---
icon: rectangle-history
---

# Registro de Cambios de la API

## 2024

<details>

<summary>2.5.0 - 26/11/2024</summary>

El [flujo de integración ideal](page.md) se ha actualizado de acuerdo con los nuevos métodos disponibles en la actualización 2.4.0, lanzada el 13/11/2024.

</details>

<details>

<summary>2.4.0 - 13/11/2024</summary>

La API para recuperar datos de procesos ha sido ajustada:\
**GET/api/v2/processo/{idProcesso}**\
Este servicio permite a los clientes, a través de la API, recuperar un proceso con sus respectivos datos, signatarios y documentos del proceso.

Nuevos métodos también fueron habilitados:

* **POST/api/v1/processo/{idProcesso}/buscar-anexos-signatarios**\
  Permite recuperar los anexos de los signatarios especificando uno o más dentro del proceso.
* **GET/api/v1/processo/{idArquivoProcesso}/registro-assinaturas**\
  Permite recuperar el registro de firma en base64 de un archivo del proceso.
* **POST/api/v1/diretorio/buscar-pastas**\
  Permite recuperar datos de carpetas dentro de la cuenta.
* **POST/api/v1/usuarios/buscar-usuarios**\
  Permite recuperar los datos de usuarios de la cuenta.
* **GET/api/v1/conta/papeis-signatarios**\
  Permite recuperar los roles de signatarios en la cuenta.
* **POST/api/v1/conta/buscar-consumo-itens-assinatura**\
  Permite recuperar la cantidad de elementos relacionados con firmas (envíos, WhatsApp, SMS) utilizados dentro de un período específico.
* **GET/api/v1/conta/dados-assinatura**\
  Permite recuperar los detalles de una cuenta ArqSIGN.
* **PATCH/api/v1/confwebhook/{idConfWebHook}/alterar-status**\
  Permite cambiar el estado de las configuraciones de webhook.
* **POST/api/v1/confwebhook**\
  Permite registrar configuraciones de webhook.

</details>

<details>

<summary>2.3.1 - 11/11/2024</summary>

La versión 1 (V1) de los siguientes métodos ha sido descontinuada:

* **POST/api/v1/processo/enviar-documento-para-assinar**
* **GET/api/v1/processo/{idprocesso}**
* **PATCH/api/v1/processo/{idProcesso}/reenviar-processo**\
  Para más detalles, haga clic aquí.

</details>

<details>

<summary>2.3.0 - 31/10/2024</summary>

El menú **Webhook** ha sido creado en Integraciones. Su propósito es permitir a los clientes monitorear el progreso de los procesos de firma de documentos. Dependiendo de la configuración del webhook, el usuario recibirá datos de ejecución del proceso a través de eventos/disparadores.

</details>

<details>

<summary>06/09/2024</summary>

Se ha creado una nueva ruta para la API de ArqSIGN.\
La ruta [**https://api.arqsign.com/**](https://api.arqsign.com/) será descontinuada el **31/10/2024**, y todos los usuarios deben actualizar sus llamadas API a la nueva ruta: [**https://api-rest.arqsign.com/**](https://api-rest.arqsign.com/).\
La documentación oficial de la API de ArqSIGN ahora está disponible en: [**https://developers.arqsign.com/**](https://developers.arqsign.com/).\
Para más detalles, haga clic aquí.

</details>

<details>

<summary>2.2.0 - 04/09/2024</summary>

Se ha creado la versión dos (V2) del siguiente método:

* **PATCH api/v2/processo/reenviar-processo/{idProcesso}**\
  Esta versión ha sido completamente reestructurada para permitir no solo la reenvío simple y directo de un proceso, sino también la edición de datos como el tipo de entrega por correo electrónico o WhatsApp, método de entrega del código de seguridad, nombre del signatario y datos obligatorios requeridos para la validación o autocompletado, dependiendo de la cuenta o tipo de firma.

</details>

<details>

<summary>2.1.0 - 05/08/2024</summary>

El menú **API** ha sido creado en Integraciones. Su propósito es proporcionar al cliente la(s) clave(s) de acceso que serán utilizadas para la gestión y control de solicitudes API.

</details>

<details>

<summary>2.0.0 - 18/07/2024</summary>

Se ha creado la versión dos (V2) de los siguientes métodos:

* **POST api/v2/processo/enviar-documento-para-assinar**\
  Se han agregado los parámetros **gerarQrCode** y **obrigarLeitura**, junto con la opción de enviar múltiples documentos **.pdf** en el proceso.
* **GET /api/v2/processo/{idProcesso}**\
  La nueva versión del servicio de recuperación de procesos devuelve todos los documentos dentro del proceso especificado, lo cual no es posible utilizando la versión 1 del servicio.

</details>

<details>

<summary>1.17.0 - 07/02/2024</summary>

**Firmar Documento:** El sistema encontró un error al intentar firmar un documento enviado a través de la API.\
El sistema mostró la representación visual en una posición incorrecta para documentos enviados a través de la API con posicionamiento manual.

</details>

## 2023

<details>

<summary>1.15.6 – 13/12/2023</summary>

En la pantalla del menú de Integraciones de la Plataforma ArqSIGN:

1. Se eliminó el enlace de Entrenamiento.
2. El término "Manual del Usuario" se cambió a "Documentación de la API".
3. El enlace de la Documentación de la API se actualizó a: [https://arquivar.gitbook.io/manual-arqsign/administracao/integracoes](https://arquivar.gitbook.io/manual-arqsign/administracao/integracoes).

</details>

<details>

<summary>1.15.3 – 13/11/2023</summary>

API > Validar Email CTG: El sistema devolvía un error 404 para ciertos dominios.

</details>

<details>

<summary>1.15.2 - 02/11/2023</summary>

API de comercio electrónico - Compra de créditos: Se ajustó el servicio de compra de créditos (/api/v1/compras/comprar-creditos) para recibir datos fiscales y dirección de cuenta.

</details>

<details>

<summary>1.14.0 - 03/10/2023</summary>

API > Enviar documento para firma: El sistema no ignoró la posición manual cuando se proporcionó el parámetro de página automática.

</details>

<details>

<summary>1.13.5 - 19/09/2023</summary>

El sistema mostró la contraseña del certificado en el payload del endpoint api/v1/certificados/validar-certificado-selecionado.

</details>

<details>

<summary>1.13.4 - 18/08/2023</summary>

API de ArqSign > Datos del Proceso: El sistema mostró la información de rechazo de la firma para todos los firmantes en lugar de solo para el firmante que rechazó el documento.

</details>

<details>

<summary>1.13.3 - 02/08/2023</summary>

API > Notificación: La aplicación mostró el nombre de la cuenta en lugar del nombre del documento en la notificación de firma.

</details>

<details>

<summary>1.13.0 - 27/06/2023</summary>

Integraciones: Se añadieron enlaces al manual de la API de ArqSIGN y al entrenamiento.

</details>

<details>

<summary>1.12.3 - 26/05/2023</summary>

API > Enviar Documento para Firma: El sistema no envió el documento con la definición de página automática.

</details>

<details>

<summary>1.12.2 - 25/05/2023</summary>

API: El sistema no aplicó la representación visual para los destinatarios que requerían representación en una página automática.

</details>

<details>

<summary>1.11.1 - 02/05/2023</summary>

API > Enviar Documento para Firmar:

* El sistema envió documentos a través de la API sin la representación visual para el tipo PJ cuando se requería el nombre de la empresa y la configuración de documentos PJ era obligatoria.&#x20;
* El sistema validó la posición de la firma para los destinatarios cuya acción era recibir una copia.&#x20;
* El sistema generó la marca de la firma en la página automática para los destinatarios que recibían una copia.

</details>

<details>

<summary>1.9.8 - 04/04/2023</summary>

Correcciones en las descripciones de los servicios de API.

</details>

<details>

<summary>1.9.7 - 30/03/2023</summary>

\[API] Enviar Documento para Firma: La aplicación no validaba cuando se enviaban parámetros tanto de posición automática como manual para la representación visual, retornando un estado 200.

Firma de Documento:&#x20;

* Al firmar un documento a través de WhatsApp enviado mediante la API, el sistema mostraba información incorrecta junto a la representación visual, mostrando el número de teléfono del signatario en el campo de correo electrónico.
* Al firmar un documento con firma electrónica enviado mediante la API, el sistema no mostraba la información del certificado vinculada a la firma.

</details>

<details>

<summary>1.9.4 - 14/03/2023</summary>

Firma de Documento: Se corrigió el bucle generado durante la firma con un Certificado Digital para un documento enviado mediante la API.

</details>

<details>

<summary>1.9.3 - 23/02/2023</summary>

API > Enviar Documento para Firma: El sistema no validó el método de entrega para guardar el contacto del signatario.

</details>

## 2022

<details>

<summary>1.8.1 – 16/11/2022</summary>

API > Enviar Documento: El sistema permitía enviar un documento utilizando el mismo correo electrónico en el mismo orden de firma.

</details>

<details>

<summary>1.6.4 - 03/06/2022</summary>

Ajuste en la API de Compra: Al recibir los datos de compra desde el comercio electrónico y cuando el país era diferente de Brasil, el sistema requería "Tipo de Persona", CPF/CNPJ y el Código Postal. Después del ajuste, estos campos ya no son obligatorios cuando el país no es Brasil.

</details>

<details>

<summary>1.3.0 - 04/01/2022</summary>

Se incluyeron validaciones de seguridad adicionales en la API llamada por el comercio electrónico en ArqSign.

</details>
