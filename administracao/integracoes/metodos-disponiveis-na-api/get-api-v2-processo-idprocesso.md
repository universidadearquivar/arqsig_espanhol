---
description: >-
  El objetivo del método es permitir a los clientes, a través de la API, buscar
  un proceso con sus respectivos datos, firmantes y documentos.
---

# ✔️ GET/api/v2/processo/{idProcesso}

## Solicitud

<figure><img src="../../../.gitbook/assets/image (762).png" alt=""><figcaption></figcaption></figure>

## Autenticaciones y Validaciones

1. Para autenticar en la API de ArqSign, el usuario debe proporcionar una AppKey válida de la cuenta que está buscando el proceso.
2. Solo una cuenta con **estado Activo** y con permiso de Integración ArqSign puede buscar **procesos mediante integración ArqSign.**
3. El sistema valida si el **IdProceso** pertenece a la cuenta de la **AppKey**.

## Retorno de Validaciones

### Error: 400 - Bad Request

Este error se devuelve cuando no se puede interpretar la solicitud y/o el servidor intenta procesarla, pero algún parámetro de la solicitud no es válido, como un recurso con formato incorrecto o una solicitud con datos faltantes. La información sobre la solicitud se proporciona en el cuerpo de la respuesta, incluyendo un código y un mensaje de error.

**a. Ítem obligatorio:** Se muestra en singular o plural cuando uno o más ítems obligatorios no han sido enviados en la llamada de la API.

**Mensaje**: **El/Los ítem(s) listado(s) es/son obligatorio(s): “nombre de los ítems separados por coma”.**

**b. Formato incorrecto**: Se muestra en singular o plural cuando uno o más ítems han sido enviados con formato incorrecto.

**Mensaje: El/Los ítem(s) listado(s) tiene(n) un formato incorrecto: “nombre de los ítems separados por coma”.**

**c. Ids inexistentes**: Se muestra en singular o plural cuando uno o más Id enviados no existen.

**Mensaje**: **El/Los id(s) listado(s) no existe(n): “nombre de los ítems que son Ids de tabla, separados por coma”.**

**d. Documento eliminado: Se muestra cuando el proceso está eliminado.**

**Mensaje: Proceso eliminado.**

**e.Algún parámetro es incorrecto o inexistente**: Se muestra cuando la llamada se realiza con algún parámetro mal escrito o se envía información que no existe en el método.

**Mensaje: Algún parámetro es incorrecto o inexistente.**

### Error: 401 – Unauthorized

Este error se devuelve cuando la clave de autenticación de la API ArqSign es incorrecta o no se ha proporcionado correctamente.

### Error: 404 - Not Found

Este error se devuelve cuando no se encuentra el recurso solicitado o el endpoint.

### Error: 422 - Unprocessable

Este error se devuelve cuando la solicitud se ha recibido correctamente, pero contiene parámetros inválidos.

### Error: 500 - Server Error

Este error se devuelve cuando:

* Ocurre un error interno en el servidor;
* Hay una falla en la plataforma ArqSign;
* Formato de JSON incorrecto.

## Retorno de éxito

Status 200 - Success

El sistema debe devolver los datos del proceso, datos de los firmantes, archivo del proceso y registro de firma.

* Datos del proceso
* Datos de los firmantes
* Documentos del proceso con su respectivo registro de firma.

<figure><img src="../../../.gitbook/assets/GET v2 (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### Datos del proceso

Esta sección del JSON devuelve los datos del proceso de firma.

#### 1. nomeProcesso

El sistema devuelve el nombre del proceso.

#### 2. idPasta

El sistema devuelve el id de la carpeta del proceso.

#### 3. caminhodaPasta

El sistema devuelve la ruta de la carpeta del proceso.\
Ej.: Archivar \Administración \ Contratos

#### 4. idResponsavel

El sistema devuelve el id del responsable (remitente) del proceso.

#### 5. nomeResponsavel

El sistema devuelve el nombre del responsable del proceso.

#### 6. status

El sistema devuelve el estado del proceso **(Creado, En espera, En proceso, Completado o Cancelado).**

#### 7. dataCadastro

El sistema devuelve la fecha de registro del proceso.

#### 8. dataEnvio

El sistema devuelve la fecha de envío del proceso. El proceso tendrá fecha de envío (**dataEnvio**) cuando el estado sea diferente de **Creado**.

#### 9. dataConclusao

El sistema devuelve la fecha de finalización del proceso. El proceso tendrá fecha de finalización (**dataConclusao**) cuando el estado sea igual a **Completado**.

#### 10. dataRenovacao

El sistema devuelve la fecha de renovación del proceso. El proceso tendrá fecha de renovación (**dataRenovacao**) cuando haya configuración de renovación y el documento esté en estado **Completado**.

&#x20;O sistema deve calcular a data de renovação conforme a configuração de renovação e a data de conclusão do documento. **(dataRenovacao = dataConclusao + renovacaoMeses)**

#### 11. dataCancelamento

El sistema devuelve la fecha de cancelación del proceso. El proceso tendrá fecha de cancelación **(dataCancelamento)** cuando el estado sea igual a **Cancelado**.

#### 12. usuarioCancelamento

El sistema devuelve el nombre del usuario que canceló el proceso. El documento mostrará el nombre del usuario que lo canceló **(usuarioCancelamento)** cuando haya una fecha de cancelación **(dataCancelamento)** y el estado sea igual a **Cancelado**.

#### 13. dataReenvio

El sistema devuelve la fecha de reenvío del proceso. El proceso tendrá una fecha de reenvío cuando el remitente vuelva a enviar el proceso a los firmantes pendientes.

#### 14. dataExpiracao:

El sistema devuelve la fecha de expiración del proceso.

El cálculo se basa en la configuración de expiración y en la fecha de envío/reenvío del documento.\
Si **dataReenvio** es null, entonces **dataExpiracao = dataEnvio + ExpiracaoDias.**\
Si **dataReenvio** es diferente de null, entonces **dataExpiracao = dataReenvio + expiracaoDias.**

#### 15. expiracaoDias

El sistema devuelve los días de expiración del proceso.

#### 16. avisoExpiracaoDias

El sistema devuelve los días para el aviso de expiración del proceso.

#### 17. lembrete:

El sistema indica si el proceso tiene un recordatorio de firma.

&#x20;El parámetro (**recordatorio**) informa si el proceso tiene o no recordatorio de firma.\
1 - true = tiene recordatorio de firma.\
0 - false = no tiene recordatorio de firma.

#### &#x20;18. frequenciaLembrete

El sistema devuelve la frecuencia del recordatorio de firma de los documentos del proceso.



### Datos de los Firmantes

Esta sección del JSON devuelve los datos de los firmantes participantes en el proceso de firma.

#### 19. firmantes

#### 19.1. ordemAssinatura

El sistema devuelve el orden de firma del firmante en cuestión.&#x20;

**19.2. id**

El sistema devuelve el id del destinatario del proceso.

**19.3. nome**

El sistema devuelve el nombre del firmante.

**19.4. email**

El sistema devuelve el correo electrónico del firmante cuando el proceso fue enviado por **correo electrónico.**

**19.5. telefone**

El sistema devuelve el teléfono del firmante cuando el proceso fue enviado por **WhatsApp**.

**19.6. aguardandoEnvio**

El sistema devuelve información de espera de envío del proceso, que puede ser true o false. Este parámetro tendrá el valor true cuando el proceso de firma tenga un orden de firmas y el firmante anterior al firmante en cuestión no haya completado la firma. De esta manera, el firmante está esperando el envío del documento para su firma.

**19.7. falhaEnvio**

El sistema indica un fallo en el envío, ya sea true o false. Este valor será true cuando haya un fallo en el envío del proceso al destinatario en cuestión.

**19.8. tipoAcao**

El sistema devuelve el tipo de acción del firmante en el proceso, que puede ser **Firmar en línea** o **Recibir una copia**.

**19.9. copiaEnviada**

El sistema devuelve información de copia enviada cuando el firmante tiene la acción de **recibir una copia**. Este parámetro tendrá el valor true cuando se haya enviado la copia del proceso o false cuando no se haya enviado la copia.

**19.10. remetente**

El sistema devuelve información sobre si el firmante es también el remitente del proceso. Este parámetro tendrá el valor true cuando el firmante sea el remitente del proceso o false cuando el firmante no sea el remitente del proceso.\
Nota: El remitente del proceso también puede participar en el proceso de firma como firmante.

**19.11. assinaturaRecusada**

El sistema devuelve información sobre firma rechazada cuando un firmante rechaza la firma del(os) documento(s). Este parámetro tendrá el valor true cuando el firmante haya rechazado la firma del(os) documento(s) o false cuando el firmante no haya rechazado la firma del(os) documento(s) del proceso.

**19.12. motivoRecusa**

El sistema devuelve información sobre el motivo del rechazo de la firma del(os) documento(s) del proceso. Cuando el parámetro **assinaturaRecusada** sea igual a **true**, el parámetro **motivoRecusa** debe contener el motivo del rechazo informado por el firmante y el estado del proceso debe ser "**Cancelado**".

**19.13. seguranca**

El sistema devuelve datos del código de seguridad solo si el firmante tiene estas configuraciones para acceder al(os) documento(s) del proceso.

**19.13.1. codigoSeguranca**

&#x20;El sistema devuelve el código de seguridad generado al enviar el proceso para firmas.

**19.13.2. codigoSegurancaEmail**

El sistema devuelve el correo electrónico cuando el código de seguridad fue enviado por **correo electrónico.**

**19.13.3. codigoSegurancaTelefone**

El sistema devuelve el teléfono cuando el código de seguridad fue enviado por **WhatsApp** o **SMS**.

**19.14. papelSignatario**

El sistema devuelve el(los) papel(es) solo si el firmante tiene estas configuraciones.

**19.14.1. pessoaFisica**

El sistema devuelve esta información cuando el firmante tiene papel(es) como persona física.

**19.14.2. pessoaJuridica**

El sistema devuelve esta información cuando el firmante tiene papel(es) como persona jurídica.

**19.15. dadosAssinatura**

El sistema devuelve datos de firma del firmante.

**19.15.1. tipoAssinatura**

El sistema devuelve el tipo de firma que el firmante ejecutó o ejecutará. Este parámetro puede tener el valor: **Firma Electrónica** o **Certificado Digital - ICP Brasil, o Certificado Digital - Otros**. Cuando el **tipo de acción** del firmante sea igual a Recibir una copia, el parámetro **tipoAssinatura** será **null**.

**19.15.2. dataAssinatura**

El sistema devuelve la fecha en que el firmante firmó el documento. Este parámetro tendrá valor null cuando el firmante no firmó el(os) documento(s) del proceso.

**19.15.3. ip**

El sistema devuelve la IP del firmante que firmó el documento. Este parámetro tendrá valor null cuando el firmante no firmó el(os) documento(s) del proceso.

**19.15.5. geoLocalizacao**

El sistema devuelve la geolocalización del firmante que firmó el documento. Este parámetro tendrá valor null cuando el firmante no firmó el(os) documento(s) del proceso o cuando el firmante no permitió capturar su ubicación.

**19.16. dadosCertificado**

El sistema devuelve los datos del certificado utilizado para firmar el(os) documento(s) del proceso.

Estos parámetros tendrán valor null cuando el firmante no firmó el(os) documento(s) del proceso.

**19.16.1. nome**

El sistema devuelve el nombre del certificado.

**19.16.2. emissor**

El sistema devuelve el emisor del certificado.

**19.16.3. validadeInicio**

El sistema devuelve el inicio de la validez del certificado.

**19.16.4. validadeFim**

El sistema devuelve el final de la validez del certificado.

**19.17. dadosPessoaFisica**

Estos datos serán devueltos cuando firmantes con tipo de firma electrónica informen los datos de persona física. Estos parámetros tendrán valor null cuando:

* El tipo de firma sea con certificado digital (ICP-Brasil o Otros), o
* El tipo de firma electrónica y el firmante no haya informado los datos de persona física, o
* El firmante no haya firmado el(os) documento(s) del proceso.

**19.17.1. nomePessoaFisica**

El sistema devuelve el nombre informado por el firmante al firmar el(os) documento(s) del proceso.

**19.17.2. tipoDocumentoPessoaFisica**

El sistema devuelve el tipo del documento de persona física del firmante. Este tendrá el valor definido en el envío de documento que puede ser **CPF, CNH, RG** u **Otro**.\
Cuando el tipo del documento de persona física sea definido como **Otro**, el sistema debe mostrar el nombre del tipo de documento definido por el usuario/remitente del proceso.

**19.17.3. numeroDocumetoPessoaFisica**

El sistema devuelve el número del documento de persona física informado por el firmante al firmar el(os) documento(s) del proceso.

**19.18. dadosPessoaJuridica**

Estos datos serán devueltos cuando firmantes con tipo de firma electrónica informen los datos de persona jurídica. Estos parámetros tendrán valor null cuando:

* El tipo de firma sea con certificado digital (ICP-Brasil u Otros), o
* El tipo de firma electrónica y el firmante no haya informado los datos de persona jurídica, o
* El firmante no haya firmado el(os) documento(s) del proceso.

**19.18.1.nomeEmpresa**

El sistema devuelve el nombre de la empresa informado por el firmante.

**19.18.2. tipoDocumentoEmpresa**

El sistema devuelve el tipo del documento de persona jurídica del firmante al firmar el(os) documento(s) del proceso. Este tendrá el valor definido en el envío de documento que puede ser **CNPJ** u **Otro**. Cuando el tipo del documento de persona jurídica sea definido como **Otro**, el sistema debe mostrar el nombre del tipo de documento definido por el usuario.

**19.18.3. numeroDocumentoEmpresa**

El sistema devuelve el número del documento de la empresa informado por el firmante al firmar el(os) documento(s) del proceso.

**19.19. anexos**

El sistema devuelve los datos de anexos cuando el firmante que firmó el(os) documento(s) realice carga de anexos, conforme a la configuración del proceso. Estos parámetros tendrán valor null cuando no haya anexos para el firmante.

**19.19.1. id**

El sistema devuelve el id del anexo insertado por el firmante.

**19.19.2. anexoDocumentoNome**

El sistema devuelve el nombre del anexo del firmante.

### Dados dos documentos do processo

Un proceso de firma puede contener uno o más documentos para ser firmados.

**20. documentos**

El sistema devuelve el(os) documento(s) del proceso de firma en el orden definido en el parámetro **"ordemDocumento"**, con su respectivo registro de firmas.

**20.1. ordemDocumento**&#x20;

El sistema devuelve el orden del documento definido en el momento en que el proceso fue enviado.

**20.2. nomeDocumento**

El sistema devuelve el nombre del documento.

**20.3. base64Documento**

El sistema devuelve el base64 del archivo.

**20.4. registroAssinaturas**

El sistema devuelve, para cada documento del proceso, el respectivo registro de firmas.

**20.4.1. nome**

El sistema devuelve el nombre del registro de firmas del documento. El nombre del registro de firma debe contener el nombre del documento más la cadena “\_registro de firmas”.\
Ejemplo: Contrato de Alquiler\_Registro de firmas.pdf

**20.4.2. base64**

El sistema devuelve el base64 del archivo del registro de firmas del documento.

### Retorno - Ejemplo Body Response

```

{
    "nomeProcesso": "string",
    "idPasta": "guid",
    "caminhoDaPasta": "string",
    "idResponsavel": "guid",
    "nomeResponsavel": "string",
    "status": "string",
    "dataCadastro": "datetime",
    "dataEnvio": "datetime",
    "dataConclusao": "datetime",
    "dataRenovacao": "datetime",
    "dataCancelamento": "datetime",
    "usuarioCancelamento": "string",
    "dataReenvio": "datetime",
    "dataExpiracao": "datetime",
    "expiracaoDias": "smallint",
    "avisoExpiracaoDias": "smallint",
    "lembrete": "true",
    "frequenciaLembrete": "smallint",
    "signatarios": [
        {
            "ordemAssinatura": "tinyint",
            "id": "guid",
            "nome": "string",
            "email": "string",
            "telefone": "string",
            "aguardandoEnvio": "string",
            "falhaEnvio": "string",
            "tipoAcao": "string",
            "papelSignatario": {
                "pessoaFisica": [
                    "varchar(50)",
                    "varchar(50)",
                    "varchar(50)"
                ],
                "pessoaJuridica": [
                    "varchar(50)"
                ]
            },
            "copiaEnviada": "string",
            "remetente": "string",
            "assinaturaRecusada": "string",
            "motivoRecusa": "string",
            "seguranca": {
                "codigoSeguranca": "string",
                "codigoSegurancaEmail": "string",
                "codigoSegurancaTelefone": "string"
            },
            "dadosAssinatura": {
                "tipoAssinatura": "string",
                "dataAssinatura": "datetime",
                "ip": "string",
                "geoLocalizacao": "string",
                "dadosCertificado": {
                    "nome": "string",
                    "emissor": "string",
                    "validadeInicio": "string",
                    "validadeFim": "string"
                },
                "dadosPessoaFisica": {
                    "nomePessoaFisica": "string",
                    "tipoDocumentoPessoaFisica": "string",
                    "numeroDocumetoPessoaFisica": "string"
                },
                "dadosPessoaJuridica": {
                    "nomeEmpresa": "string",
                    "tipoDocumentoEmpresa": "string",
                    "numeroDocumentoEmpresa": "string"
                },
                "anexos": [
                    {
                        "id": "guid",
                        "anexoDocumentoNome": "string"
                    }
                ]
            }
        }
    ],
    "documentos": [
        {
            "ordemDocumento": "tinyint",
            "nomeDocumento": "string",
            "base64Documento": "string base64",
            "registroAssinaturas": {
                "nome": "string",
                "base64": "string base64"
            }
        },
        {
            "ordemDocumento": "tinyint",
            "nomeDocumento": "string",
            "base64Documento": "string base64",
            "registroAssinaturas": {
                "nome": "string",
                "base64": "string base64"
            }
        }
    ]
}
```

