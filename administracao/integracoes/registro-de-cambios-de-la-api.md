---
icon: rectangle-history
---

# Registro de Cambios de la API

## 2024

<details>

<summary>2.5.0 - 26/11/2024</summary>

El flujo de integración ideal se ha actualizado de acuerdo con los nuevos métodos disponibles en la actualización 2.4.0, lanzada el 13/11/2024.

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

<summary></summary>



</details>
