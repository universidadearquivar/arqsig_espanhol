---
icon: arrow-progress
---

# Flujo de Integración Ideal

El flujo de integración ideal de ArqSIGN debe combinar el uso de la API de ArqSIGN y los Webhooks de ArqSIGN.

Para lograr una automatización óptima, es esencial configurar dos Webhooks: uno para monitoreo y otro para finalización.

## Webhook de Monitoreo

El propósito del webhook de monitoreo es mantener su sistema actualizado sobre acciones clave relacionadas con el documento, así como indicar momentos críticos para llamar a otras API de ArqSIGN.

En la respuesta del webhook de monitoreo, se recomienda no incluir ningún dato del documento. Dado que el proceso aún no está completado, no es necesario transmitir archivos potencialmente grandes.

### Disparadores

* Un proceso firmado por un signatario
* Un proceso con falla de envío
* Un proceso rechazado por un signatario
* Un proceso cancelado por el remitente
* Un proceso expirado

### Retorno

* Datos del proceso
* Signatarios

## **Webhook de Finalización**

El propósito del webhook de finalización es enviar el documento firmado a su sistema una vez que todos los signatarios hayan firmado. En esta etapa, el sistema puede enviar el archivo en Base64 o el enlace tanto al archivo firmado como a su registro de firma. Idealmente, el webhook envía las URL de estos archivos a su endpoint, permitiendo que su aplicación maneje la descarga. Si esto no es factible, el webhook puede configurarse para enviar el archivo en Base64.

### Retorno

* Datos del proceso
* Signatarios
* Documentos
  * Archivos del proceso: Enlace para descargar el archivo
  * Enlaces compartidos del documento
  * Registro de firma: Enlace para descargar el archivo

Con los dos Webhooks configurados, puede implementar el siguiente flujo de integración.

## Flujo de Integración

Haga clic en las imágenes para ampliarlas

<figure><img src="../../.gitbook/assets/image (777).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (778).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (779).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (780).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (781).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (782).png" alt=""><figcaption></figcaption></figure>

### Flujo de Trabajo Detallado

1. **Envío de Documentos a los Signatarios**

En esta etapa, el cliente debe implementar la llamada al método POST responsable de enviar el documento a ser firmado en la plataforma ArqSIGN.

**Método:**

> * **Nombre:** Enviar Proceso de Firma V2
> * **URL:** POST [https://api-rest.arqsign.com/api/v2/processo/enviar-documento-para-assinar](https://api-rest.arqsign.com/api/v2/processo/enviar-documento-para-assinar)
> * **Documentación:** [https://developers.arqsign.com/api-details#api=api-rest-arqsign\&operation=6734bb1a4640eeaf71857525](https://developers.arqsign.com/api-details#api=api-rest-arqsign\&operation=6734bb1a4640eeaf71857525)

2. **Monitoreo: Falla**

Si hay alguna falla en la entrega de documentos a ser firmados por un signatario, la aplicación ArqSIGN activará el Webhook, que llamará al servicio (URL) del cliente según lo configurado.

Después de recibir esta respuesta del Webhook, el cliente puede implementar la llamada al método PATCH responsable de reenviar el proceso. Este método también puede usarse para editar el método de entrega a los signatarios con fallas en la entrega.

**Método:**

> * **Nombre:** Editar y Reenviar el Proceso a Signatarios Pendientes V2
> * **URL:** PATCH https://api-rest.arqsign.com/api/v2/processo/{idProcesso}/reenviar-processo
> * **Documentación:** [https://developers.arqsign.com/api-details#api=api-rest-arqsign\&operation=6734bb1a21b37c983bbe8bbe](https://developers.arqsign.com/api-details#api=api-rest-arqsign\&operation=6734bb1a21b37c983bbe8bbe)

3. **Monitoreo: Firmado por un Signatario**

Cuando un signatario firma el documento, la aplicación ArqSIGN activará el Webhook, que llamará al servicio (URL) del cliente según lo configurado.

Con los datos retornados por el Webhook, el cliente puede actualizar su sistema para mantener la información sincronizada.

4. **Monitoreo: Rechazo o Cancelación**

El proceso puede ser cancelado de tres maneras:

* Cuando un signatario se niega a firmar el documento;
* Cuando la persona responsable del envío del documento cancela el proceso a través de la aplicación ArqSIGN;
* Cuando el cliente llama al método PATCH API Proceso/Cancelar-Proceso para cancelar el proceso.

Cuando ocurre la cancelación, el Webhook llamará al endpoint del cliente como fue configurado, proporcionando información sobre si el proceso fue cancelado o si un signatario se negó a firmar. Si el signatario se niega a firmar, la aplicación le exigirá proporcionar una justificación, que también será enviada por el Webhook.

En este punto, el cliente puede manejar la respuesta y decidir si reinicia el proceso llamando al método POST para enviar un nuevo documento para firmar (Paso 1).

5. **Monitoreo: Expiración**

Cuando el documento expira, la aplicación ArqSIGN activará el Webhook, que llamará al endpoint del cliente como fue configurado.

Después de recibir esta respuesta del Webhook, el cliente puede implementar la llamada al método PATCH responsable de reenviar el proceso. Este método actualizará el token de firma para los signatarios que aún no hayan firmado el documento.

**Método:**

> * **Nombre:** Editar y Reenviar el Proceso a Signatarios Pendientes V2
> * **URL:** PATCH https://api-rest.arqsign.com/api/v2/processo/{idProcesso}/reenviar-processo
> * **Documentación:** [https://developers.arqsign.com/api-details#api=api-rest-arqsign\&operation=6734bb1a21b37c983bbe8bbe](https://developers.arqsign.com/api-details#api=api-rest-arqsign\&operation=6734bb1a21b37c983bbe8bbe)

6. **Conclusión**

Cuando el último signatario firma el documento, la aplicación ArqSIGN activará el Webhook, que llamará al endpoint del cliente como fue configurado.

Después de recibir esta respuesta del Webhook, el cliente puede almacenar el documento firmado y su registro de firma en su sistema.

Tenga en cuenta que, al configurar dos webhooks según nuestra recomendación, el documento firmado y completado solo será transmitido en esta etapa a través del Webhook de Conclusión.
