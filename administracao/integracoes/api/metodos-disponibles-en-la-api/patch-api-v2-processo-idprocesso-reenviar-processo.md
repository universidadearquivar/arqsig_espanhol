# ✔️ PATCH/api/v2/processo/{idProcesso}/reenviar-processo

Este servicio permite a los Clientes, a través de API, **reenvíar el proceso** a los **destinatarios pendientes de firma** en el orden de firma actual, permitiendo editar los datos de los destinatarios pendientes de firma.

## Requisición - Orientaciones

Cuando el campo requerido esté como “Sí” = Siempre requerido

Cuando el campo requerido esté como “No” = Información opcional

Cuando el campo requerido esté como “Tal vez” = En algunos casos será requerido. Para conocer estos casos, consulte la descripción del tema, de acuerdo con el número de referencia de la línea en la tabla.

<div align="left"><figure><img src="../../../../.gitbook/assets/image (440).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure></div>

## Ejemplo Body Request

**Ejemplo Body - Sin edición**

```
[]

```

Ejemplo Body - Con edición

```
[
    {
        "idProcessoDestinatario": "Guid",
        "idFormaEnvioProcesso": "bit",
        "nome": "string",
        "email": "string",
        "telefone": "string",
        "idMeioEnvioCodigoSeguranca": "bit",
        "emailSeguranca": "string",
        "telefoneSeguranca": "string",
        "permitirReenviarCodigo": "bit",
        "dadosAssinatura": {
            "signatario": {
                "nome": "string",
                "numeroDocumento": "string",
                "validar": "bit"
                "DescartarDadosAnteriores": "bit"
            },
            "empresa": {
                "nome": "string",
                "numeroDocumento": "string",
                "validar": "bit"
                "DescartarDadosAnteriores": "bit"
            }
        }
    }
]

```

## Validaciones

### Validaciones Generales - Autenticación

Para autenticarse en la API de ArqSign, se debe proporcionar el AppKey de la cuenta que está reenviando el proceso. Esta cuenta debe estar activa y con el debido permiso para el uso de la integración Arqsign.

### Validaciones Generales - Descripción de los parámetros JSON

**01. idProcessoDestinatario**

**Descripción:** Parámetro que indica el Id del destinatario al que se reenviará el proceso.

**Formato:** Guid

**Requerido:** <mark style="color:red;">Sí, cuando hay datos para edición.</mark>

**Validación:** El reenvío del proceso solo está permitido para destinatarios con acción de Firmar Online que tengan pendiente la acción de firma en los documentos. No se permite el envío del proceso a destinatarios con acción de Recibir Copia.

***

**02. IdFormaEnvioProcesso**

**Descripción:** Parámetro que indica la forma de reenvío del proceso

**Formato:** Bit - 1 - E-mail o 2 - Whatsapp

**Requerido:** <mark style="color:blue;">No</mark>

***

**03. nome**

**Descripción:** Parámetro que indica el nombre del destinatario.

**Formato:** String

**Requerido:** <mark style="color:blue;">No</mark>

***

**04. email**

**Descripción:** Parámetro que indica el correo electrónico para reenviar el proceso.

**Formato:** String

**Requerido:** <mark style="color:red;">Sí, cuando el parámetro idFormaEnvio es igual a 1.</mark>

&#x20;**Validación:** El correo electrónico proporcionado debe tener un formato válido.

***

**05. telefone**

**Descripción:** Parámetro que indica el teléfono para reenviar el proceso.

**Formato:** String

**Requerido:** <mark style="color:red;">Sí, cuando el parámetro idFormaEnvio es igual a 2.</mark>

**Validación**: Solo es posible reenviar el proceso por WhatsApp (idFormaEnvioProcesso = 2) cuando el tipo de firma del destinatario es electrónica.

***

**06. idMeioEnvioCodigoSeguranca**

**Descripción:** Los datos del Código de Seguridad solo pueden editarse para destinatarios que tengan la configuración de código de seguridad, sin permitir la inserción de un código de seguridad para destinatarios que no fueron configurados inicialmente para utilizarlo. Solo se permite cambiar la forma de entrega del código de seguridad para los destinatarios que tengan esta configuración en el proceso.                 &#x20;

**Formato:** Bit, 1- SMS (Solo Brasil), 2 – Whatsapp, 3 – Email o 4 - No enviar

**Requerido:** <mark style="color:blue;">No</mark>

***

**07. emailSeguranca**

**Descripción:** Parámetro que indica el correo electrónico para el envío del código de seguridad.

**Formato:** String

**Requerido:** <mark style="color:red;">Sí, cuando el parámetro idMeioEnvioCodigoSeguranca es igual a 3.</mark>

***

**08.** **telefoneSeguranca**

**Descripción:** Parámetro que indica el teléfono para el envío del código de seguridad.

**Formato:** String

**Requerido:** <mark style="color:red;">Sí, cuando el parámetro idMeioEnvioCodigoSeguranca es igual a 1 o 2.</mark>

***

**09. permitirReenviarCodigo**

**Descripción:** Permitir el reenvío del código de seguridad.

**Formato:** Bit, 1 = true o 0 = False

**Requerido:** <mark style="color:blue;">No</mark>

***

**10.dadosAssinatura**

Esta parte del JSON es opcional y **permite editar los datos de firma de los destinatarios** con **idTipoAssinatura igual a 1 = electrónica** que tengan estos datos configurados, los cuales pueden ser utilizados para el llenado de campos o la validación del documento en el momento en que el destinatario firme los documentos del proceso como persona física y/o jurídica.

Cuando se envían datos de firma para **destinatarios que no fueron configurados inicialmente con estos datos**, estos serán desconsiderados.

**10.1 Signatario:** Parámetros para editar el nombre y el documento del signatario que serán utilizados para el llenado de campos en pantalla o la validación del documento del signatario.

**a. nome**

**Descripción:** Parámetro que indica el documento del signatario que será cambiado al reenviar el proceso.

**Formato:** Varchar(250)

**Requerido:** <mark style="color:blue;">No</mark>

**b. numeroDocumento**

**Descrición:** Parámetro que indica el documento del signatario que será cambiado al reenviar el proceso.

**Formato:** String

**Requerido:** <mark style="color:blue;">No</mark>

**c. validarDocumento**

**Descripción:** Parámetro que indica si el número del documento del destinatario modificado en el parámetro numeroDocumento del objeto signatario será utilizado para validación o no.

**Formato:** Bit: 1 – True o 0 - False

**Requerido:** <mark style="color:blue;">No</mark>

**Los datos indicados en este parámetro serán desconsiderados cuando** el parámetro **numeroDocumento** del objeto **signatario** sea nulo o no se envíe.

**Cuando este parámetro no se envíe o se envíe** con **null** o con **valor 0**, significa que los datos indicados en el parámetro **numeroDocumento** serán utilizados solo para el llenado automático en el momento de la firma como persona física..

**Cuando este parámetro se envíe con valor 1**, significa que los datos indicados en el parámetro **numeroDocumento** serán utilizados para validación en el momento de la firma como persona física.

**d. DescartarDadosAnteriores**

**Descripción:** Parámetro que indica si los datos no indicados en el objeto signatario serán descartados.

**Formato:** Bit: 1 – True o 0 - False

**Requerido:** <mark style="color:blue;">No</mark>

**Los datos indicados en este parámetro serán desconsiderados cuando** los parámetros **nombre** y **numeroDocumento** del objeto signatario sean **enviados**.

**Cuando este parámetro no se envíe o se envíe** con **null** o con **valor 0**, significa que ningún parámetro del objeto **signatario** será descartado.

**Cuando este parámetro se envíe con valor 1**, significa que los datos no indicados del objeto **signatario** deben ser eliminados del proceso.

**10.2 empresa:** Parámetros para editar el nombre y el documento de la empresa que serán utilizados para el llenado de campos en pantalla o la validación del documento del signatario.

{% hint style="warning" %}
**Atención**: **Los datos de empresa serán desconsiderados** cuando el signatario esté configurado para firmar únicamente como **persona física**.
{% endhint %}

**a. nome**

Descripción: Parámetro que informa el nombre de la empresa que se modificará al reenviar el proceso.

**Formato:** Varchar(250)

**Requerido:** <mark style="color:blue;">No</mark>

**b. numeroDocumento**

Descripción: Parámetro que informa el documento de la empresa que se modificará al reenviar el proceso.

**Formato:** String

**Requerido:** <mark style="color:blue;">No</mark>

**Validación: Cuando este parámetro NO sea informado o sea nulo** y el parámetro **DescartarDatosAnteriores sea enviado con valor 1**, la información del documento será eliminada del proceso.

**c. validarDocumento**

**Descripción:** Parámetro que indica si el número de documento de la empresa modificado en el parámetro numeroDocumento del objeto empresa se utilizará para validación o no.

**Formato:** Bit: 1 – True o 0 - False

**Requerido:** <mark style="color:blue;">No</mark>

**Los datos informados en este parámetro deben ser desconsiderados cuando el** parámetro **numeroDocumento** del objeto empresa sea **nulo**.

**Cuando este parámetro no sea enviado, sea enviado** con valor **null** o con **valor 0**, significa que los datos informados en el parámetro **numeroDocumento** serán utilizados solo para el **llenado automático** en el momento de la firma como persona jurídica.

**Cuando este parámetro sea enviado con valor 1**, significa que los datos informados en el parámetro **numeroDocumento** serán utilizados para la **validación** en el momento de la firma como persona física.

**d. DescartarDadosAnteriores**

**Descripción:** Parámetro que indica si los datos no informados en el objeto empresa serán descartados.

**Formato:** Bit: 1 – True o 0 - False

**Requerido:** <mark style="color:blue;">No</mark>

**Los datos informados en este parámetro serán desconsiderados cuando los** parámetros nombre y **numeroDocumento** del objeto **empresa** sean enviados.

**Cuando este parámetro no sea enviado**, sea enviado con valor **null** o con **valor 0**, significa que ningún parámetro del objeto **empresa** será descartado.

**Cuando este parámetro sea enviado con valor 1**, significa que los datos no informados del objeto **empresa** serán eliminados del proceso.

***

## Retorno de Validaciones

### Error: 400 - Bad Request

Este error se devuelve cuando no se puede interpretar la solicitud y/o el servidor intenta procesarla, pero algún parámetro no es válido, por ejemplo, un recurso con formato incorrecto o una solicitud con datos faltantes. La información sobre la solicitud se proporciona en el cuerpo de la respuesta e incluye un código de error y un mensaje de error.

**a. Ítem obligatorio:** Este mensaje se mostrará en singular o plural cuando uno o más ítems obligatorios no hayan sido enviados en la llamada a la API: **El(los) ítem(s) listado(s) es(son) obligatorio(s): “nombres de los ítems separados por comas”.**

&#x20;**b. Formato incorrecto:** Este mensaje se mostrará en singular o plural cuando uno o más ítems hayan sido enviados con formato incorrecto: **El(los) ítem(s) listado(s) está(án) con formato incorrecto: “nombres de los ítems separados por comas”.**

**c. Ids inexistentes:** Este mensaje se mostrará en singular o plural cuando uno o más Ids enviados no existan: **El(los) id(s) listado(s) no existe(n): “nombres de los ítems que son Ids de tabla, separados por comas”.**

**d. Algún parámetro está incorrecto o es inexistente:** Este mensaje se mostrará cuando la llamada se realice con algún parámetro escrito incorrectamente o cuando se envíe una información que no existe en el método: **Algún parámetro está incorrecto o es inexistente.**

### Erro: 401 – Unauthorized

Este error se devuelve cuando:

• La clave de autenticación de la API ArqSign es incorrecta o no fue informada correctamente.

• La cuenta tiene un estado diferente de Activo.

### Erro: 404 - Not Found

Este error se devuelve cuando el recurso solicitado o el endpoint no fue localizado.

### Erro: 422 - Unprocessable

Este error se devuelve cuando la solicitud fue recibida con éxito, pero contiene parámetros inválidos.

### Erro: 500 - Server Error

Este error se devuelve cuando:

• Ocurre un error interno en el servidor.

• Ocurre una falla en la plataforma ArqSign.

• Formato del parámetro incorrecto.

• Formato del JSON incorrecto.

***

## Retorno Éxito

**Code 200** – OK

Al ejecutar el reenvío del proceso con éxito, el sistema **devolverá los datos de los participantes del proceso pendientes de firma de los documentos.**

{% hint style="warning" %}
<mark style="color:orange;">**Atención: Incluso si el destinatario no ha sido informado para reenvío, los datos de este también se devolverán si está pendiente de firma.**</mark>
{% endhint %}

**Por ejemplo:**

En un proceso que tiene 3 firmantes pendientes de firma.

Al reenviar el proceso sin editar datos, se devolverán los datos de los 3 firmantes pendientes de firma.

Al reenviar el proceso editando los datos de un firmante, se devolverán los datos de los 3 firmantes pendientes de firma.

### &#x20;Retorno - Ejemplo de Cuerpo de Respuesta

```
[
    {
        "idProcessoDestinatario": "guid",
        "ordem": 1, //numérico  
        "formaEnvioProcesso": "string",
        "nome": "string",
        "anexos": [
            {
                "idConfiguracaoAnexo": "guid",
                "nomeAnexo": "string"
            }
        ]
    },
    {
        "idProcessoDestinatario": "guid",
        "ordem": 1, //numérico  
        "formaEnvioProcesso": "string",
        "nome": "string",
        "anexos": null
    }
]

```

**a. idProcessoDestinatario**&#x20;

La API devuelve el id del proceso destinatario.

**b. ordem**

La API devuelve el orden de firma del destinatario.

**c. formaEnvioProcesso**

&#x20;La API devuelve la forma de envío del proceso para el destinatario, ya sea por e-mail o teléfono del destinatario.

&#x20;**d. Nome**

&#x20;La API devuelve el nombre del destinatario.

&#x20;**e. Anexo**&#x20;

La API devuelve las configuraciones de anexo del destinatario, si las hay.
