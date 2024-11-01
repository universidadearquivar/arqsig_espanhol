---
description: >-
  El objetivo de este método es permitir a los clientes, a través de la API,
  enviar procesos con uno o más documentos para firmar.
---

# ✔️ POST/api/v2/processo/enviar-documento-para-assinar

A diferencia de la aplicación ArqSign, que permite agrupar los archivos del proceso, en este servicio, al enviar un proceso con más de un documento, se considera como **una colección de archivos y estos no serán agrupados en un único archivo**. Es decir, no es posible agrupar archivos mediante el servicio de envío de documentos para firmar.

El usuario debe informar los datos del proceso y de los destinatarios participantes en el proceso de firma.

## Autenticaciones y permisos

1. Para autenticarse en la API de ArqSign, el usuario debe proporcionar la AppKey válida de la cuenta que está enviando los documentos para firmar.
2. Solo las cuentas con **estado Activo** y con **permiso de Integración ArqSign** pueden enviar procesos a través de la integración de ArqSign.
3. La cuenta debe tener créditos de Envios, SMS y/o WhatsApp, según sea necesario.
4.  Si la cuenta no tiene créditos, el sistema devolverá el mensaje:

    "Saldo de créditos de Envios o WhatsApp o SMS insuficientes."

## Solicitud: Parámetros

**Orientaciones:**

Cuando el campo requerido esté marcado como “Sí” = Siempre requerido.

Cuando el campo requerido esté marcado como “No” = Información opcional.

Cuando el campo requerido esté marcado como “Tal vez” = En algunos casos será requerido. Para saber estos casos, consulte la descripción del tópico, conforme el número de referencia de la línea en la tabla.

Cuando el campo requerido esté marcado como “No” = Información opcional.

<figure><img src="../../../.gitbook/assets/Pastel Simple Important points to build an attractive personal website infographic (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### **Ejemplo de Body Request**

```
{
   "idResponsavel": "guid",
   "nomeProcesso": "varchar(250)",
    "idPasta": "guid",
    "configuracoesAvancadas": {
        "tempoExpiracaoDocumentoDias": "smallint",
        "avisoAntesExpiracaoDocumentoDias": "smallint",
        "frequenciaLembretesDias": "smallint",
        "gerarQrCode": "bit",
        "obrigarLeitura": "bit"
    },
    "renovacaoMeses": "tinyint",
    "mensagemPadrao": {
        "titulo": "varchar(150)",
        "texto": "varchar(max)"
    },
    "usarOrdemAssinatura": "bit",
    "usarPosicaoAssinaturaAutomatica": "bit",
    "destinatarios": [
        {
            "idTipoAcao": "tinyint",
            "ordemAssinatura": "tinyint",
            "nome": "varchar(150)",
            "email": "varchar(150)",
            "telefone": "varchar(20)",
            "assinarOnline": {
                "assinarComo": "tinyint",
                "papelPessoaFisica": [
                    "varchar(50)",
                    "varchar(50)",
                    "varchar(50)"
                ],
                "papelPessoaJuridica": [
                    "varchar(50)"
                ],
                "seguranca": {
                    "codigoSeguranca": "char(4)",
                    "idMeioEnvio": "tinyint",
                    "codigoSegurancaEmail": "varchar(150)",
                    "codigoSegurancaTelefone": "varchar(20)",
                    "reenviarCodigo": "bit"
                },
                "mensagemPersonalizada": {
                    "titulo": "VarChar(150)",
                    "texto": "VarChar(max)"
                },
                "anexos": [
                    {
                        "anexoDocumentoNome": "VarChar(75)",
                        "anexoObrigatorio": "bit",
                        "anexoExibirTodosDestinatarios": "bit"
                    }
                ],
                "definirPosicaoAssinaturaManual": [
                    {
                        "documentoDeOrdem": "tinyint",
                        "pessoaFisica": {
                            "pagina": "int",
                            "altura": "decimal",
                            "largura": "decimal",
                            "posicaoX": "decimal",
                            "posicaoY": "decimal"
                        },
                        "pessoaJuridica": {
                            "pagina": "int",
                            "altura": "decimal",
                            "largura": "decimal",
                            "posicaoX": "decimal",
                            "posicaoY": "decimal"
                        }
                    }

                ],
                "idTipoAssinatura": "tinyint",
                "assinaturaEletronica": {
                    "obrigarSignatarioInformarNome": "bit",
                    "obrigarSignatarioInformarNumeroDocumento": "bit",
                    "tipoDocumentoAInformar": "tinyint",
                    "configuracaoDocumentoOutro": {
                        "nomeDocumento": "VarChar(50)",
                        "formatoDadosDocumento": "tinyint",
                        "qtdeCaracteresDocumento": "tinyint"
                    },
                    "obrigarSignatarioInformarNomeEmpresa": "bit",
                    "obrigarSignatarioInformarNumeroDocumentoEmpresa": "bit",
                    "tipoDocumentoEmpresaAInformar": "tinyint",
                    "configuracaoDocumentoEmpresaOutro": {
                        "nomeDocumento": "VarChar(50)",
                        "formatoDadosDocumento": "tinyint",
                        "qtdeCaracteresDocumento": "tinyint"
                    }
                }
            }
        }
    ],
    "documentos": [//somente pdf
        {
            "ordemDocumento": "tinyint",
            "nomeComExtensao": "varchar(150)",
            "arquivo": "String Base64"
        },
        {
            "ordemDocumento": "tinyint",
            "nomeComExtensao": "varchar(150)",
            "arquivo": "String Base64"
        }
    ]
}


```

## Descripción de los parámetros del JSON

### idResponsavel

Parámetro **obligatorio** que informa el ID del responsable del proceso. Esta información se considerará como el responsable del registro y del proceso, es decir, el “remitente” del proceso. De esta forma, si el usuario informado autentica en la aplicación, podrá visualizar todos los documentos en el menú “Enviados”.

Debe informarse el ID de un usuario activo que pertenezca a la cuenta.

### nomeProcesso

Parámetro **obligatorio** que informa el Nombre del proceso, permitiendo hasta 250 caracteres.

### idPasta

Parámetro obligatorio que informa el ID de la carpeta del proceso.&#x20;

Debe informarse un ID de carpeta que pertenezca a la cuenta.

### configuracoesAvancada

En esta parte del JSON, el usuario puede enviar las configuraciones avanzadas para el proceso en relación a tiempo de expiración, aviso de expiración, frecuencia de este aviso, generación del QRCode y obligatoriedad de lectura de los documentos del proceso.

Las configuraciones avanzadas son **opcionales** y **si no se envían** o se envían como nulas, el sistema **guardará el proceso con las configuraciones de la cuenta en cuestión.**

#### **tempoExpiracaoDocumentoDias**

Parámetro **opcional** que informa el tiempo en que el proceso estará disponible para firma, hasta que todos los firmantes firmen y el proceso se concluya.&#x20;

Se permiten valores entre {1} y {999}.

Cuando este parámetro no se envía o se envía como nulo o 0, el sistema considera las configuraciones de la cuenta.

#### **avisoAntesExpiracaoDocumentoDias**

Parámetro **opcional** que informa el tiempo para que la aplicación inicie el aviso antes de que el documento expire.\
Se permiten valores entre {1} y {99}.

Cuando este parámetro no se envía o se envía como nulo o 0, el sistema considera las configuraciones de la cuenta.

#### **frequenciaLembretesDias:**

Parámetro **opcional** que informa el tiempo para avisos de firma.&#x20;

Se permiten valores entre {1} y {999}.

Cuando este parámetro no se envía o se envía como nulo o 0, el sistema considera las configuraciones de la cuenta.

#### **gerarQrCode**

Parámetro **opcional** que informa si debe generarse el QRCode del documento firmado o no al momento de la conclusión del proceso.\
Cuando el proceso tiene más de un documento para firma, se generará un QRCode por documento. Cada documento tendrá su QRCode y su página de firma.

Se permite informar 1 = True o 0 = false.

Cuando este parámetro no se envía o se envía como nulo o 0, el sistema considera las configuraciones de la cuenta.

#### **obrigarLeitura**

Parámetro **opcional** que informa la obligatoriedad de lectura de los documentos al firmar.\
Cuando el proceso en cuestión tiene más de un documento para firmar, esta información se utilizará para obligar o no al firmante a hacer clic en cada documento antes de que el botón “Firmar” sea habilitado.\
Si el proceso solo tiene un archivo para firmar, esta información no será necesaria para el proceso de firma.\
Se permite informar 1 = True o 0 = false.

Cuando este parámetro no se envía o se envía como nulo o 0, el sistema considera las configuraciones de la cuenta.

### renovacaoMeses

Parámetro **opcional** que informa el tiempo, en meses, para definir cuándo el proceso en cuestión necesita ser renovado.

### mensagemPadrao

Parámetro **opcional** que informa el mensaje estándar que será enviado a todos los destinatarios definidos como firmantes del proceso.\
Si la colección de datos **“mensagemPadrao” no se envía**, el sistema envía las notificaciones con los valores predeterminados:\
**Título** = ArqSign: \[Nombre del documento informado en el parámetro "nome"]\
**Texto =** Usted ha recibido el/los documento(s): \[Nombre del documento informado en el parámetro "nome"] para firmas.

#### titulo

Parámetro **opcional** que informa el Título del mensaje a ser enviado a los firmantes.

**texto**

Parámetro **opcional** que informa el Texto del mensaje a ser enviado a los firmantes.

### usarOrdemAssinatura

Parámetro **obligatorio** que informa si se utilizará o no orden de firma para los firmantes.

a. Cuando el parámetro **usarOrdemAssinatura** se envía como **false**, el sistema desconsidera el valor informado en el parámetro “**ordemAssinatura**” de todos los destinatarios con acción de Firmar Online y envía el proceso a todos los destinatarios considerando como orden 1.

b. Cuando el parámetro **usarOrdemAssinatura** se envía como **true**, el sistema valida el parámetro “**ordemAssinatura**” de todos los destinatarios con acción de Firmar Online. Es decir, el parámetro “**ordemAssinatura**” de los destinatarios no puede ser cero o null.

Si el proceso tiene orden de firma, el sistema envía el proceso solo para los destinatarios de orden 1.

### usarPosicaoAssinaturaAutomatica

Parámetro **obligatorio** para indicar a la aplicación si el proceso en cuestión tendrá la página de firma al final de cada archivo. En esta página, la aplicación elige automáticamente dónde cada firma será posicionada.\
Se permite informar 1 = True o 0 = false.

a. Cuando el parámetro “**usarPosicaoAssinaturaAutomatica**” es **true**, la aplicación **incluirá una página al final de cada archivo, con la posición de la firma de cada destinatario con acción de Firmar Online**, considerando el tipo de persona para cada firmante según se describe a continuación:

* • Para los firmantes con el parámetro **assinarComo** = 1 (Persona física), significa que la aplicación ArqSign incluirá una página al final del archivo con la definición automática de la posición de la firma del tipo **Persona Física** (PF).
* • Para los firmantes con el parámetro **assinarComo** = 2 (Persona jurídica), significa que la aplicación ArqSign incluirá una página al final del archivo con la definición automática de la posición de la firma del tipo **Persona Jurídica** (PJ).
* • Para los firmantes con el parámetro **assinarComo** = 3 (Persona física y jurídica), significa que la aplicación ArqSign incluirá una página al final del archivo con la definición automática de la posición para dos firmas, una del tipo **Persona Física** (PF) y una del tipo **Persona Jurídica** (PJ).

Cuando el parámetro “**usarPosicaoAssinaturaAutomatica**” se **envía como true**, no es necesario enviar los parámetros **definirPosicaoAssinaturaManual**. Pero si en el JSON se envía para algún firmante el parámetro **definirPosicaoAssinaturaManual, la información será ignorada en este caso.**

b.Cuando el parámetro **usarPosicaoAssinaturaAutomatica** se envía como **false**, significa que el posicionamiento de las firmas **para cada firmante** deberá ser informado manualmente **para cada archivo del proceso** en cuestión. Siendo obligatorio enviar los datos del parámetro **definirPosicaoAssinaturaManual**.

{% hint style="danger" %}
<mark style="color:red;">**Importante:**</mark> <mark style="color:red;"></mark><mark style="color:red;">En el JSON, todos los destinatarios con acción de firmar en línea deben tener el posicionamiento de la representación visual de forma automática por parte de la aplicación, o el posicionamiento para todos debe enviarse manualmente en el JSON. No puede haber en el mismo proceso algunos destinatarios con posicionamiento automático y otros sin posicionamiento automático.</mark>
{% endhint %}

### destinatários

#### idTipoAcao

Parámetro **obligatorio** que define la acción del destinatario con respecto al documento. Actualmente hay dos opciones: **1 - Firmar en línea o 2 - Recibir una copia.**&#x20;

Está permitido informar 1 - Firmar en línea o 2 - Recibir una copia.

&#x20;a. Es obligatorio informar al menos un destinatario con la acción de "**Firmar en línea**" para el proceso de firmas.

#### ordemAssinatura

Parámetro que define el orden de firma del firmante en cuestión.\
\
**a.** Cuando el parámetro “**usarOrdemDeAssinatura**” se envía como **True = 1** y el destinatario en cuestión tiene el parámetro **idTipoAcao = 1 (Firmar en línea)**, entonces esta información es obligatoria.

El parámetro **ordemAssinatura** no debe enviarse en el JSON o será desconsiderado cuando:\
\- **idTipoAcao = 2 (Recibir una copia).**\
\- **usarOrdemDeAssinatura = 0 (falso)** y firmantes con **idTipoAcao = 1 (Firmar en línea)**.

**b.** La aplicación **no permite el mismo destinatario en el mismo orden de firma**. Para verificar si el destinatario es el mismo, se comprueba si el correo electrónico o el teléfono utilizado para enviar el documento se repiten en la misma orden de firma.

#### nome

Parámetro **obligatorio** que informa el nombre del destinatario que firmará el documento o recibirá una copia.

**a.** El sistema valida la obligatoriedad y el tamaño del nombre del firmante.

#### email

Parámetro que informa el correo electrónico donde el destinatario recibirá el documento.

**Formato:** Varchar(150)&#x20;

**Requerido:** Correo electrónico o Teléfono son obligatorios

**Validación**:

**a.** El sistema valida la **obligatoriedad** del correo electrónico o teléfono. \
Cuando no se envía ningún correo electrónico o teléfono, la aplicación valida los datos mostrando el mensaje: "El parámetro **email** o **teléfono** es obligatorio".

**b.** Solo se permite un correo electrónico válido.

**c.** Solo se **permite informar correo electrónico o teléfono**.\
Cuando el usuario proporciona ambos campos, el sistema devuelve el mensaje: "Solo es posible enviar el proceso a un correo electrónico o teléfono. Elija una forma de envío".

#### telefone

Parámetro que informa el teléfono donde el destinatario recibirá el documento. Al enviar el número de teléfono, significa que el documento será enviado por **WhatsApp**.

**a.** El sistema valida la **obligatoriedad** del correo electrónico o teléfono.\
Cuando no se envía ningún correo electrónico o teléfono, la aplicación valida los datos mostrando el mensaje: "El parámetro **email o teléfono** es obligatorio".

**b.** El sistema **valida** el teléfono informado.

**c.** Solo se **permite informar correo electrónico o teléfono**.\
Cuando el usuario proporciona ambos campos, el sistema devuelve el mensaje: "Solo es posible enviar el proceso a un correo electrónico o teléfono. Elija una forma de envío".

**d.** Solo es posible enviar el proceso por WhatsApp cuando el destinatario cumpla con uno de los requisitos a continuación:\
**1.** Si va a firmar el documento electrónicamente idTipoAcao = **1 (Firmar en línea) y idTipoAssinatura = 1 (Firma Electrónica).**\
**2.** Si va a recibir una copia: **idTipoAcao = 2 (Recibir una copia).**

### **assinarOnline**

Esta parte del JSON debe enviarse solo para los destinatarios con **idTipoAcao = 1 (Firmar en línea)**. Si se envía para un destinatario con **idTipoAcao = 2 (Recibir copia)**, estos datos serán ignorados.

#### **assinarComo**

Parámetro obligatorio que indica si el firmante, con el **idTipoAcao = 1 (Firmar en línea)**, firmará como persona física, persona jurídica o ambos.\
Está permitido informar 1 = Persona Física o 2 = Persona Jurídica o 3 = Persona Física y Jurídica.

#### papelPessoaFisica

Parámetro **opcional** para enviar los papeles del firmante en relación a la firma de persona física que realizará.

**a.** El parámetro **papelPessoaFisica es opcional**, pero cuando se informa, el sistema verifica **si la cuenta posee el papel del firmante informado.**\
El usuario podrá informar null o no informar este parámetro en el JSON.

Si el **papelPessoaFisica** se envía para un firmante con el parámetro “**assinarComo**” = 2 (Persona Jurídica), entonces esta información se desconsidera.

#### papelPessoaJurídica

Parámetro **opcional** para enviar los papeles del firmante en relación a la firma de persona jurídica que realizará.

**a.** El parámetro **papelPessoaJuridica es opcional**, pero cuando se informa, el sistema verifica **si la cuenta posee el papel del firmante informado.**\
El usuario podrá informar null o no informar estos parámetros en el JSON.

Si el **papelPessoaJuridica** se envía para un firmante con el parámetro “**assinarComo**” = 1 (Persona Física), entonces esta información se desconsidera.

#### seguranca

Esta parte del JSON es **opcional** y debe enviarse solo si hay necesidad de exigir al firmante un código de seguridad para iniciar el proceso de firma.

1. **codigoSeguranca**\
   Código de seguridad a exigir al firmante que va a firmar el documento. Esta información debe ser numérica con 4 caracteres.
2. **idMeioEnvio**\
   Parámetro para informar cómo se enviará el código de seguridad al firmante en cuestión.
3.  Este parámetro solo será exigido si se envía el parámetro **codigoSeguranca** y solo se permiten valores iguales a 1 = SMS (solo Brasil), 2 = WhatsApp, 3 = Correo electrónico o 4 = No enviar.

    El sistema desconsidera la información de este parámetro si **codigoSeguranca** = null.
4.  **codigoSegurancaEmail**\
    Correo electrónico donde el firmante deberá recibir el código de seguridad definido en el parámetro **codigoSeguranca**.

    **a.** El parámetro **codigoSegurancaEmail** es obligatorio cuando el parámetro **idMeioEnvio** es igual a 3.

    **b.** La aplicación valida si la información enviada es un correo electrónico.

    Si este parámetro se envía cuando idMeioEnvio ≠ 3, el sistema ignora la información.

    El sistema desconsidera la información de este parámetro si codigoSeguranca = null.
5.  **codigoSegurancaTelefone**\
    Teléfono donde el firmante deberá recibir el código de seguridad definido en el parámetro **codigoSeguranca**.

    **a.** . El parámetro **codigoSegurancaTelefone** es obligatorio cuando el parámetro **idMeioEnvio** es igual a **1** o **2**.

    Cuando idMeioEnvio = 1 (SMS), solo se aceptan números de Brasil.

    El sistema valida el teléfono informado.

    Si este parámetro se envía cuando idMeioEnvio = 3 o 4, el sistema ignora la información.

    El sistema desconsidera la información de este parámetro si **codigoSeguranca** = null.
6. **reenviarCodigo**\
   Información que define si el firmante podrá reenviar el código de seguridad a su teléfono vía SMS o WhatsApp, según la definición en el parámetro idMeioEnvio.
7.  Cuando el parámetro **reenviarCodigo** no se informa en el JSON, el servicio lo considera como false.

    Está permitido informar 1 = True ou 0 = False

    **a.** Este parámetro solo es obligatorio cuando el código de seguridad se envía por SMS o WhatsApp.

    Si este parámetro se envía cuando idMeioEnvio = 3 o 4, se desconsidera.

#### mensagemPersonalizada

Esta parte del JSON es **opcional** y deberá enviarse solamente si para el signatario en cuestión es necesario enviar un mensaje personalizado. Si se envía el título del mensaje, será necesario enviar el texto y viceversa.

1.  **titulo**\
    Texto del mensaje personalizado a ser enviado al signatario en cuestión. Los signatarios con mensaje personalizado no reciben el **mensagemPadrao.**

    **a.** El parámetro **mensagemPersonalizada** no es obligatorio, pero cuando se envía el “titulo”, la aplicación debe exigir el texto y viceversa.
2. **texto**\
   Texto del mensaje personalizado a ser enviado al signatario en cuestión. Los signatarios con mensaje personalizado no reciben el **mensagemPadrao.**
3. **a.** El parámetro **mensagemPersonalizada** no es obligatorio, pero cuando se envía el “titulo”, la aplicación debe exigir el texto y viceversa.

#### anexos

Esta parte del JSON es **opcional** y deberá enviarse solamente si para el signatario en cuestión es necesario solicitar la carga de algún archivo en el momento de la firma. Si cualquiera de los parámetros a continuación es enviado, será necesario enviar los tres.

Si cualquiera de los parámetros a continuación es enviado, será necesario enviar los tres: **anexoDocumentoNome, anexoObrigatorio y anexoExibirTodosDestinatarios.**

1.  **anexoDocumentoNome**\
    Nombre del anexo que será solicitado al signatario en el momento de la firma de los documentos.

    Es permitido informar hasta 75 caracteres.
2.  **anexoObrigatorio**\
    Información para la aplicación exigir del signatario la carga del archivo en el momento de la firma del documento.

    Es permitido informar 1 = True o 0 = false.
3.  **anexoExibirTodosDestinatarios**\
    Información para la aplicación **mostrar el anexo que fue enviado por el signatario a todos los otros destinatarios con acción de firmar o no**. Si el anexo a ser enviado exige un grado de sigilo, entonces esta información debe ser enviada como falso.

    Es permitido informar 1 = True o 0 = false.

#### definirPosicaoAssinaturaManual

Esta parte del JSON es obligatoria solamente si el parámetro **usarPosicaoAssinaturaAutomatica** es igual a **false**.\
Cuando el parámetro **usarPosicaoAssinaturaAutomatica** es enviado igual a **false**, significa que en el JSON **deberá ser enviada la posición manual de las firmas de todos los destinatarios con acción de Firmar en Línea en cada archivo del proceso**. Es decir, es obligatorio definir la posición de la firma manualmente (**definirPosicaoAssinaturaManual**) para cada destinatario en cada archivo (**documentoDeOrdem**) conforme al valor definido en el parámetro **assinarComo** (1 = Persona Física o 2 = Persona Jurídica o 3 = Persona Física y Jurídica).\
\
Cuando el parámetro **usarPosicaoAssinaturaAutomatica** es enviado como verdadero, las informaciones de posicionamiento manual de la firma de todos los signatarios **serán desconsideradas**. De esta forma, se incluirá **una página al final de cada documento con la posición de la firma de cada destinatario con acción de Firmar en Línea.**\
\
El sistema valida si el posicionamiento manual de las firmas está dentro del límite de la página informada. El sistema valida las representaciones manuales informadas para los destinatarios, no permitiendo la misma representación manual por tipo de firma en el mismo documento (**parámetro documentoDeOrdem**).

#### documentoDeOrdem

Cuando el **proceso** de firma que está siendo enviado en el JSON posee más de un archivo para firma, este campo será usado para identificar el archivo al cual el posicionamiento de la firma que está siendo descrito en los parámetros a continuación se refiere.

Si el proceso de firma posee solamente un archivo a ser firmado, este campo se vuelve innecesario y será desconsiderado cuando se envíe.\
**a.** Este parámetro es obligatorio siempre que en el proceso exista más de un archivo a ser firmado.\
**b.** El sistema valida si existe el documento de la orden informada en el parámetro “**documentoDeOrdem**”.

#### pessoaFisica

Los parámetros a continuación indicarán la posición de la firma de persona física para el signatario en cuestión, en el archivo identificado en **documentoDeOrdem** y serán obligatorios cuando los parámetros **usarPosicaoAssinaturaAutomatica** = **false** y **assinarComo** = **1 (PF) o 3 (PF y PJ).**

Cuando el parámetro **assinarComo = 2 (PJ)**, estos datos serán desconsiderados. Los parámetros a continuación indicarán la posición de la firma de persona física para el signatario en cuestión, para el archivo identificado en **documentoDeOrdem**.

1.  **pagina**\
    Esta información es la página del archivo donde la posición de la firma será insertada. Es obligatoria cuando **usarPosicaoAssinaturaAutomatica** = **false** y **assinarComo = 1 (PF) o 3 (PF y PJ).**

    **a.** Esta información no puede ser cero ni nula.

    **b.** La aplicación valida si la página informada existe en el archivo en cuestión.
2.  **altura**\
    Altura en milímetros del tamaño de la caja donde la firma será aplicada. Es **obligatoria** cuando **usarPosicaoAssinaturaAutomatica** = **false** y **assinarComo = 1 (PF) o 3 (PF y PJ**).

    Es permitido informar valor decimal.

    **a.** Esta información no puede ser nula.
3.  **largura**\
    Anchura en milímetros del tamaño de la caja donde la firma será aplicada. Es **obligatoria** cuando **usarPosicaoAssinaturaAutomatica** = **false** y **assinarComo = 1 (PF) o 3 (PF y PJ)**.

    Es permitido informar valor decimal.

    **a.** Esta información no puede ser nula.
4.  **posicaoX**\
    **Descripción:** Posición en milímetros de la orilla izquierda de la página hasta la orilla izquierda de la caja de firma.

    Es **obligatoria** cuando **usarPosicaoAssinaturaAutomatica** = **false** y **assinarComo = 1 (PF) o 3 (PF y PJ).**

    Es permitido informar valor decimal.

    **a.** Esta información no puede ser nula.
5.  **posicaoY**\
    **Descripción:** Posición en milímetros de la orilla superior de la página hasta la orilla superior de la caja de firma.

    Es **obligatoria** cuando **usarPosicaoAssinaturaAutomatica** = **false** y **assinarComo = 1 (PF) o 3 (PF y PJ).**

    Es permitido informar valor decimal.

    **a.** Esta información no puede ser nula.

#### pessoaJuridica

Los parámetros a continuación indicarán la posición de la firma de persona jurídica para el signatario en cuestión, en el archivo identificado en **documentoDeOrdem** y serán obligatorios cuando los parámetros **usarPosicaoAssinaturaAutomatica** = **false** y **assinarComo = 2 (PJ) o 3 (PF y PJ).**

Cuando el parámetro **assinarComo = 1 (PF)**, estos datos serán desconsiderados.

1.  **pagina**\
    Esta información es la página del archivo donde la posición de la firma será insertada. Es **obligatoria** cuando **usarPosicaoAssinaturaAutomatica** = **false** y **assinarComo = 2 (PJ) o 3 (PF y PJ).**

    **a.** Esta información no puede ser cero ni nula.

    **b.** La aplicación valida si la página informada existe en el archivo en cuestión.
2.  **altura**\
    Altura en milímetros del tamaño de la caja donde la firma será aplicada. Es **obligatoria** cuando **usarPosicaoAssinaturaAutomatica** = **false** y **assinarComo = 2 (PJ) o 3 (PF y PJ).**

    Es permitido informar valor decimal.

    **a.** Esta información no puede ser cero ni nula.
3.  **largura**\
    Ancho en milímetros del tamaño de la caja donde la firma será aplicada. Es **obligatoria** cuando **usarPosicaoAssinaturaAutomatica** = **false** y **assinarComo = 2 (PJ) o 3 (PF y PJ).**

    Es permitido informar valor decimal.

    **a**. Esta información no puede ser cero ni nula.
4.  **posicaoX**\
    Posição em milímetros da borda esquerda da página até a borda esquerda da caixa de assinatura. É **obrigatória** quando **usarPosicaoAssinaturaAutomatica = false** e **assinarComo = 2 (PJ) ou 3 (PF e PJ).**

    É permitido informar valor decimal.

    **a**. Esta informação não pode ser zero nem nula.
5.  **posicaoY**\
    **Descrição:** Posição em milímetros da borda superior da página até a borda superior da caixa de assinatura. . É obrigatória quando **usarPosicaoAssinaturaAutomatica = false** e **assinarComo = 2 (PJ) ou 3 (PF e PJ).**

    É permitido informar valor decimal.

    **a.** Esta informação não pode ser zero nem nula.

#### idTipoAssinatura

Definição do tipo de assinatura que será exigida ao signatário que pode ser: **1 = Assinatura Eletrônica, 3 = Certificado Digital ICP Brasil** ou **4 = Certificado Digital Outros.**\
**a.** Esta informação é obrigatória para todos os signatários com parâmetro idTipoAcao = 1 (Assinar Online).\
**b.** A aplicação permite somente os valores 1,3 ou 4.

#### assinaturaEletronica

Esta parte do JSON somente é **obrigatória** para os signatários com **idTipoAssinatura = 1** (Assinatura Eletrônica).

*   **obrigarSignatarioInformarNome**\
    Informação para a aplicação obrigar o signatário em questão informar seu nome.

    É permitido informar 1 = True ou 0 = False.

    **a.** Esta informação é obrigatória para todos os signatários com idTipoAssinatura = 1 (Assinatura Eletrônica).
*   **obrigarSignatarioInformarNumeroDocumento**\
    Informação para a aplicação obrigar o signatário em questão informar o número de seu documento.

    É permitido informar 1 = True ou 0 = False.

    **a.** Esta informação é obrigatória para todos os signatários com idTipoAssinatura = 1 (Assinatura Eletrônica).
*   **tipoDocumentoAInformar**\
    Tipo de documento que o signatário deverá informar no momento da assinatura, permitindo os valores: **1 = CPF**, **2 = CNH**, **3 = RH** ou **4 = Outro**.

    **a.** Esta informação é obrigatória para todos os signatários com idTipoAssinatura = 1 (Assinatura Eletrônica).

    **b.** Quando informado, o sistema valida o parâmetro **tipoDocumentoAInformar** permitindo somente os valores:  1 = CPF, 2 = CNH, 3 = RH ou 4 = Outro.
* **configuracaoDocumentoOutro**\
  Esta parte do JSON somente **é obrigatória** quando o **tipoDocumentoAInformar** for igual a **4 = Outro**. Nesta parte é possível definir os parâmetros do documento que será solicitado ao signatário a informação, no ato da assinatura.
  1.  **nomeDocumento**\
      Nome do documento que será exibido ao signatário no momento da assinatura dos documentos.

      É permitido informar valores com até 50 caracteres
  2. **formatoDadosDocumento**\
     Formato de dados que será exigido no campo de documento, permitindo o valor 1 = Texto ou 2 = Numérico.
  3. **qtdeCaracteresDocumento**\
     Quantidade de caracteres que serão exigidos no campo documento.
*   **obrigarSignatarioInformarNomeEmpresa**\
    Informação para a aplicação obrigar o signatário em questão informar o nome da empresa (pessoa jurídica).

    É permitido informar 1 = True ou 0 = False.

    **a.** Esta informação é obrigatória para os signatários quando parâmetros idTipoAssinatura  = 1 (Assinatura Eletrônica) e assinarComo seja igual a 2 = Pessoa Jurídica ou 3 = Pessoa Física e Jurídica.
*   **obrigarSignatarioInformarNumeroDocumentoEmpresa**\
    Informação para a aplicação obrigar o signatário em questão informar o documento da empresa (pessoa jurídica).

    É permitido informar 1 = True ou 0 = False.

    **a.** Esta informação é obrigatória para os signatários quando parâmetros idTipoAssinatura  = 1 (Assinatura Eletrônica) e assinarComo seja igual a 2 = Pessoa Jurídica ou 3 = Pessoa Física e Jurídica.
*   **tipoDocumentoEmpresaAInformar**\
    Tipo de documento que o signatário deverá informar para a empresa.

    É permitido informar 4 = Outro ou 5 = CNPJ.

    **a.** Esta informação é obrigatória para os signatários quando parâmetros idTipoAssinatura  = 1 (Assinatura Eletrônica) e assinarComo seja igual a 2 = Pessoa Jurídica ou 3 = Pessoa Física e Jurídica.

    **b.** Quando informado, o sistema validr o parâmetro **tipoDocumentoEmpresaAInformar** permitindo somente os valores:  4 = Outro ou 5 = CNPJ.
*   **configuracaoDocumentoEmpresaOutro**\
    Esta parte do JSON somente é **obrigatória quando** o **tipoDocumentoEmpresaAInformar** **for igual a 4 = Outro.**

    Nesta parte é possível definir os parâmetros do documento que será solicitado ao signatário a informação, no ato da assinatura.

    1.  **nomeDocumento**\
        Nome do documento que será exibido ao signatário como documento da empresa, permitindo informar até 50 caracteres.

        **a.** Esta informação é obrigatória para todos os signatários com tipoDocumentoEmpresaAInformar = 4 (Outro).
    2.  **formatoDadosDocumento**\
        Formato de dados que será exigido no campo de documento da empresa, permitindo informar 1 = Texto ou 2 = Numérico

        a. Esta informação é obrigatória para todos os signatários com tipoDocumentoEmpresaAInformar = 4 (Outro).
    3.  **qtdeCaracteresDocumento**\
        Quantidade de caracteres que serão exigidos no campo documento.

        a. Esta informação é obrigatória para todos os signatários com tipoDocumentoEmpresaAInformar = 4 (Outro). &#x20;

### documentos

**a.** Esta parte do JSON é **obrigatória, sendo necessário enviar pelo menos um arquivo.**

**b.** É permitido enviar até 25 arquivos por processo.

**c.** A soma do tamanho destes arquivos não pode ultrapassar a **100MB**.

**d.** Somente é permitido arquivo do tipo PDF.

#### ordemDocumento

Quando estiver sendo enviado mais de um arquivo no processo, será necessário definir a ordem com que estes arquivos serão listados na tela para o signatário assinar. Esta ordem também será usada para relacionar o posicionamento da assinatura do signatário no arquivo em questão. Ver parâmetro **documentoDeOrdem.**\
**a.** Para processo com mais de um arquivo o parâmetro **ordemDocumento** é obrigatório em cada documento.\
**b.** Não é permitido arquivos com mesma ordem.\
**c.** Quando estiver sendo enviado mais de um arquivo, eles serão considerados como uma coleção de arquivos para o processo em questão, **não serão mergeados,** ou seja, agrupados em um único arquivo.\
Não é possível agrupar arquivos pelo serviço de envio de processo de documentos para assinar.

#### nomeComExtensao

Parâmetro **obrigatório** para informar o Nome do arquivo com sua extensão, permitindo até 150 caracteres.\
**a.** A aplicação **não permite** arquivos com nomes iguais em um mesmo processo.

#### arquivo

Parâmetro **obrigatório** para informar o arquivo PDF no formato base64.\
**a.** É obrigatório enviar pelo menos um arquivo. Ele precisa ser enviado no formato PDF.



## Retorno Validações

### Erro: 400 - Bad Request

Este erro é retornado quando não for possível interpretar a requisição e/ou o servidor tenta processar a solicitação, mas algum parâmetro da solicitação não é válido, por exemplo, um recurso formatado incorretamente ou uma tentativa de requisição com dados faltantes. As informações sobre a solicitação são fornecidas no corpo da resposta e incluem um código de erro e uma mensagem de erro.

**a.** **Item obrigatório**: Esta mensagem é exibida no singular ou plural quando um ou mais itens obrigatórios não tiver sido enviado na chamada da API.

**O(s) item(ns) listado(s) é(são) obrigatório(s): “nome dos itens separados por vírgula”.**

**b. Formato incorreto:** Esta mensagem é exibida no singular ou plural quando um ou mais itens estiverem sido enviados com formato incorreto.

&#x20;**O(s) item(ns) listado(s) está(ão) com o formato incorreto: “nome dos itens separados por vírgula”.**

**c. Ids inexistente:** Esta mensagem é exibida no singular ou plural quando um ou mais Id enviado não existir.

&#x20;**O(s) id(s) listado(s) não existe(m): “nome dos itens que são Ids de tabela, separados por vírgula”.**

**d. Algum parâmetro está incorreto ou é inexistente:** Esta mensagem é exibida quando a chamada é feita com algum parâmetro escrito errado ou quando é enviado uma informação que não existe no método.

**Algum parâmetro está incorreto ou é inexistente.**

### Erro:  401 - Unauthorized

Este erro é retornado quando

* A chave de autenticação da API ArqSign está incorreta ou não foi informada corretamente.
* Conta está com status diferente de Ativo.

### Erro: 404 - Not Found

Este erro é retornado quando o recurso solicitado ou o _endpoint_ não foi localizado.

### Erro: 422 - Unprocessable

Este erro é retornado quando a requisição foi recebida com sucesso, porém contém parâmetros inválidos.

### Erro: 500 - Server Error

Este erro é retornado quando:

* Ocorre um erro interno no servidor.
* Ocorre uma falha na plataforma ArqSign.
* Formato do parâmetro incorreto.        &#x20;
* Formato do JSON incorreto.



## Retorno Sucesso

Ao executar o envio do processo com sucesso, o sistema retorna o id do processo e o(s) id(s) do(s) documento(s) do processo.

Code 200 – OK

### Retorno - Exemplo Body Response

```
{
    "IdProcesso": "guid",
    "documentos": [
        {
            "id": "guid",
            "nome": "string"
        },
        {
            "id": "guid",
            "nome": "string"
        }
    ]
}

```

#### idProcesso

O sistema retorna o id do processo criado.

#### documentos

Neste objeto o sistema retorna os  id’s e o nomes dos documentos do processo.\
Um processo por ter uma ou mais documentos.

#### idDocumento

O sistema retorna o id do documento do processo.

#### nomeDocumento

O sistema retorna o nome do documento do processo criado.
