# ✔️ POST/api/v1/processo/enviar-documento-para-assinar

El objetivo de este método es permitir que el usuario envíe un documento para ser firmado a través de la plataforma ArqSIGN. En esta versión, todos los documentos enviados para firma se agrupan en un mismo PDF.

{% hint style="danger" %}
<mark style="color:red;">Este método tiene una versión actualizada disponible para su uso.</mark>

<mark style="color:red;">Si va a utilizar el método por primera vez, lo ideal es comenzar utilizando la versión más reciente, disponible en</mark> [<mark style="color:red;">**POST/api/v2/processo/enviar-documento-para-assinar**</mark>](../../metodos-disponiveis-na-api/post-api-v2-processo-enviar-documento-para-assinar.md)<mark style="color:red;">.</mark>

<mark style="color:red;">Para aquellos que ya utilizan el método en la versión 1, la funcionalidad permanece igual, aunque esta versión no contará con nuevas funcionalidades. Dependerá del cliente evaluar el uso y decidir si mantiene la utilización de la versión 1 o migra a la versión 2.</mark>

<mark style="color:red;">Consulte aquí un</mark> [<mark style="color:red;">**comparativo de información**</mark>](./#comparativo-json-v1xv2) <mark style="color:red;">que le ayudará en el proceso de migración.</mark>
{% endhint %}

## Requisición

### Ejemplo de JSON de Requisição

```
{
  "configuracoesAvancadas": {
    "tempoExpiracaoDocumentoDias": 1,
    "avisoAntesExpiracaoDocumentoDias": 1,
    "frequenciaLembretesDias": 1
  },
  "mensagemPadrao": {
    "titulo": "1",
    "texto": "1"
  },
  "destinatarios": [
    {
      "seguranca": null,
      "mensagemPersonalizada": {
        "titulo": "",
        "texto": null
      },
      "destinatariosEntradaDto": {
        "infComplNomeSignatarioObrigatorio": true,
        "infComplDocumentoSignatarioObrigatorio": true,
        "infComplRazaoSocialObrigatorio": false,
        "infComplIdentificadorObrigatorio": false,
        "idInfComplTipoDocumentoSignatarioPF": 1,
        "infComplDocumentoNomePF": "1",
        "idInfComplTipoDadosIndentificadorPF": 1,
        "infComplQtdeCaracteresPF": null,
        "idInfComplTipoDocumentoSignatarioPJ": 5,
        "infComplDocumentoNomePJ": "",
        "idInfComplTipoDadosIndentificadorPJ": null,
        "infComplQtdeCaracteresPJ": null
      },
      "anexos": [],
      "ordem": 1,
      "nome": "Nome destinatario aqui",
      "idTipoAssinatura": 1,
      "idTipoAcao": 1,
      "idFormaEnvio": 1,
      "email": "Email destinatario aqui",
      "telefone": null,
      "definirPosicaoAssinaturaAutomatica": 1
    },
    {
      "seguranca": null,
      "mensagemPersonalizada": {
        "titulo": "",
        "texto": null
      },
      "destinatariosEntradaDto": {
        "infComplNomeSignatarioObrigatorio": true,
        "infComplDocumentoSignatarioObrigatorio": true,
        "infComplRazaoSocialObrigatorio": false,
        "infComplIdentificadorObrigatorio": false,
        "idInfComplTipoDocumentoSignatarioPF": 1,
        "infComplDocumentoNomePF": "1",
        "idInfComplTipoDadosIndentificadorPF": 1,
        "infComplQtdeCaracteresPF": null,
        "idInfComplTipoDocumentoSignatarioPJ": 5,
        "infComplDocumentoNomePJ": "",
        "idInfComplTipoDadosIndentificadorPJ": null,
        "infComplQtdeCaracteresPJ": null
      },
      "anexos": [],
      "ordem": 1,
      "nome": "Nome destinatario aqui",
      "idTipoAssinatura": 1,
      "idTipoAcao": 1,
      "idFormaEnvio": 1,
      "email": "email destinatario aqui",
      "telefone": null,
      "definirPosicaoAssinaturaAutomatica": 1
    },
    {
      "seguranca": null,
      "mensagemPersonalizada": {
        "titulo": "",
        "texto": null
      },
      "destinatariosEntradaDto": {
        "infComplNomeSignatarioObrigatorio": true,
        "infComplDocumentoSignatarioObrigatorio": true,
        "infComplRazaoSocialObrigatorio": false,
        "infComplIdentificadorObrigatorio": false,
        "idInfComplTipoDocumentoSignatarioPF": 1,
        "infComplDocumentoNomePF": "1",
        "idInfComplTipoDadosIndentificadorPF": 1,
        "infComplQtdeCaracteresPF": null,
        "idInfComplTipoDocumentoSignatarioPJ": 5,
        "infComplDocumentoNomePJ": "",
        "idInfComplTipoDadosIndentificadorPJ": null,
        "infComplQtdeCaracteresPJ": null
      },
      "anexos": [],
      "ordem": 2,
      "nome": "Nome destinatario aqui",
      "idTipoAssinatura": 1,
      "idTipoAcao": 1,
      "idFormaEnvio": 1,
      "email": "Email destinatario aqui",
      "telefone": null,
      "definirPosicaoAssinaturaAutomatica": 1
    },
    {
      "seguranca": null,
      "mensagemPersonalizada": {
        "titulo": "",
        "texto": null
      },
      "destinatariosEntradaDto": {
        "infComplNomeSignatarioObrigatorio": true,
        "infComplDocumentoSignatarioObrigatorio": true,
        "infComplRazaoSocialObrigatorio": false,
        "infComplIdentificadorObrigatorio": false,
        "idInfComplTipoDocumentoSignatarioPF": 1,
        "infComplDocumentoNomePF": "1",
        "idInfComplTipoDadosIndentificadorPF": 1,
        "infComplQtdeCaracteresPF": null,
        "idInfComplTipoDocumentoSignatarioPJ": 5,
        "infComplDocumentoNomePJ": "",
        "idInfComplTipoDadosIndentificadorPJ": null,
        "infComplQtdeCaracteresPJ": null
      },
      "anexos": [],
      "ordem": 3,
      "nome": "nome destinatario aqui",
      "idTipoAssinatura": 1,
      "idTipoAcao": 1,
      "idFormaEnvio": 1,
      "email": "Email destinatario aqui",
      "telefone": null,
      "definirPosicaoAssinaturaAutomatica": 1
    },
    {
      "seguranca": null,
      "mensagemPersonalizada": {
        "titulo": "",
        "texto": null
      },
      "destinatariosEntradaDto": {
        "infComplNomeSignatarioObrigatorio": true,
        "infComplDocumentoSignatarioObrigatorio": true,
        "infComplRazaoSocialObrigatorio": false,
        "infComplIdentificadorObrigatorio": false,
        "idInfComplTipoDocumentoSignatarioPF": 1,
        "infComplDocumentoNomePF": "1",
        "idInfComplTipoDadosIndentificadorPF": 1,
        "infComplQtdeCaracteresPF": null,
        "idInfComplTipoDocumentoSignatarioPJ": 5,
        "infComplDocumentoNomePJ": "",
        "idInfComplTipoDadosIndentificadorPJ": null,
        "infComplQtdeCaracteresPJ": null
      },
      "anexos": [],
      "ordem": 5,
      "nome": "Nome do destinatÃƒÂ¡rio aqui",
      "idTipoAssinatura": 1,
      "idTipoAcao": 1,
      "idFormaEnvio": 1,
      "email": "Email destinatario aqui",
      "telefone": null,
      "definirPosicaoAssinaturaAutomatica": 1
    },
    {
      "seguranca": null,
      "mensagemPersonalizada": {
        "titulo": "",
        "texto": null
      },
      "destinatariosEntradaDto": {
        "infComplNomeSignatarioObrigatorio": true,
        "infComplDocumentoSignatarioObrigatorio": true,
        "infComplRazaoSocialObrigatorio": false,
        "infComplIdentificadorObrigatorio": false,
        "idInfComplTipoDocumentoSignatarioPF": 1,
        "infComplDocumentoNomePF": "1",
        "idInfComplTipoDadosIndentificadorPF": 1,
        "infComplQtdeCaracteresPF": null,
        "idInfComplTipoDocumentoSignatarioPJ": 5,
        "infComplDocumentoNomePJ": "",
        "idInfComplTipoDadosIndentificadorPJ": null,
        "infComplQtdeCaracteresPJ": null
      },
      "anexos": [],
      "ordem": 5,
      "nome": "Nome destinatario aqui",
      "idTipoAssinatura": 1,
      "idTipoAcao": 1,
      "idFormaEnvio": 1,
      "email": "Email destinatario aqui",
      "telefone": null,
      "definirPosicaoAssinaturaAutomatica": 1
    }
  ],
  "documentos": [
    {
      "arquivo": "Base64 aqui",
      "nomeComExtensao": "nomedoc.pdf"
    }
  ],
  "IdPasta" : "Id Pasta aqui",
  "renovacaoMeses": 1,
  "assinarOrdemDestinatarios": true,
  "nome": "nome arquivo aqui",
  "idResponsavel": "IdResponsavel aqui" 
}
```

<figure><img src="../../../../.gitbook/assets/POST.png" alt=""><figcaption></figcaption></figure>

### Detallamiento del Header y Body

**General:** Los parámetros no obligatorios que se enumeran a continuación deben estar en el JSON, y si no son necesarios para el documento, enviarlos con el valor null al lado:

&#x20;    \-> Ref. 03 “ConfiguracoesAvancadas”

&#x20;    \-> Ref. 05 “RenovacoesMeses”

&#x20;    \-> Ref. 08 “MensagemPadrão”

&#x20;    \-> Ref. 10.08 “Seguranca”

&#x20;    \-> Ref. 10.09 “mensagemPersonalizada”

&#x20;    \-> Ref. 10.10 “destinatariosEntradaDto”

&#x20;    \-> Ref. 10.11 “Anexos”

&#x20;    \-> Ref. 10.12 “definirPosicaoAssinaturaAutomatica”

&#x20;    \-> Ref. 10.13 “definirPosicaoAssinaturaManual”

**Ref. 01:** “AppKey” es la clave de autorización para autenticar en la API. Esta clave debe ser válida y estar vinculada a una cuenta activa de ArqSIGN.a.

**Ref. 03:** “ConfiguracoesAvancadas” - Las configuraciones avanzadas son un valor opcional para enviar un documento a ser firmado. Cuando esta configuración no se envía, la aplicación utiliza los valores predeterminados configurados en la cuenta.

**Ref. 03.01:** “tempoExpiracaoDocumentoDias” - es el tiempo de expiración en días para que el documento sea firmado por los firmantes. Después de este tiempo, si el documento no es firmado, expira y queda indisponible para firma.

**Ref. 03.02:** “avisoAntesExpiracaoDocumentoDias” -es el tiempo en días que la aplicación utilizará como referencia para comenzar a notificar al usuario antes de la expiración del documento.

**Ref. 03.03:** “frequenciaLembreteDias” - es la frecuencia para el envío de recordatorios a los firmantes para recordarles que firmen el documento.

**Ref. 04:** “idPasta” - es el ID de la carpeta donde el documento será almacenado dentro de la aplicación ArqSIGN.

**Ref. 05:** “renovacaoMeses” - es el tiempo en meses contados a partir de la fecha de firma del documento, que el mismo debe ser renovado, generando recordatorios de renovación para el responsable del documento.

**Ref. 06:** “assinarOrdemDestinatarios” – cuando “true”, significa que los firmantes deberán firmar el documento siguiendo un orden definido en el campo “ordem”. Cuando “false” significa que los firmantes no deberán firmar siguiendo un orden.

**Ref. 07:** “nome” - es el nombre del proceso de firma. Este nombre es la referencia de búsqueda del documento dentro de la aplicación.

**Ref. 08:** “mensagemPadrao” - es el mensaje que se enviará en la notificación a todos los firmantes que recibirán el documento para ser firmado por correo electrónico y que no tienen configuración de “mensagemPersonalizada”.

**Ref. 08. 01:** “titulo” - en este campo debe informarse el texto que será enviado como asunto del mensaje.

**Ref. 08.02:** “texto” - en este campo debe informarse el texto que será enviado como cuerpo del mensaje.

**Ref. 09:** “idResponsavel” - es el ID de un usuario activo vinculado a la cuenta en la plataforma ArqSIGN que será considerado responsable del documento que se está enviando a través de la API. Este usuario recibirá notificaciones de conclusión, rechazo de firma y recordatorios de renovación del documento, si existen.

**Ref. 10:** “Destinatarios” - en esta parte del JSON deben definirse todos los destinatarios para el documento en cuestión. Los destinatarios pueden ser personas que firmarán el documento o que recibirán una copia al final del proceso después de la firma de todos los firmantes.

**Ref. 10.01:** “ordem” – en este campo debe enviarse el orden en que el firmante firmará el documento. Este campo debe tener valor, si el campo Ref. 06 “assinarOrdemDestinatario” ha sido enviado como true. Los destinatarios configurados para recibir una copia (destinatarios del proceso que no firmarán el documento) tendrán el orden desconsiderado.

**Ref. 10.02:** “nome” – en este campo debe enviarse el nombre del destinatario.

**Ref. 10.03:** “idTipoAção” – en este campo debe definirse lo que el destinatario deberá ejecutar en el documento.

&#x20;    \-> 1 = Firmar en línea.

&#x20;    \-> 2 = Recibir una copia.

**Ref. 10.04:** “idTipoAssinatura” – en este campo debe definirse el tipo de firma del destinatario. Cuando “idTipoAção” = 1 (Firmar en línea), enviar el código de 1 a 4. Cuando “idTipoAção” = 2 (Recibir una copia), enviar el código 5.

&#x20;     \-> 1 = Firma Electrónica.

&#x20;     \-> 2 = Certificado Digital – ICP Brasil.

&#x20;     \-> 4 = Certificado Digital – Outros.

&#x20;     \-> 5 = Sin Firma.

**Ref. 10.05:** “idFormaEnvio” – en este campo debe enviarse cómo el destinatario deberá recibir el documento.

&#x20;    \-> 1 = Correo Electrónico

&#x20;    \-> 2 = WhatsApp

**Ref. 10.06:** “email” - si “idFormaEnvio” es 1 (correo electrónico), en este campo debe enviarse el correo electrónico al que el destinatario recibirá el documento.

**Ref. 10.07:** “telefone” - caso o “idFormaEnvio” seja 2 (whatsapp), en este campo debe enviarse el teléfono al que el destinatario recibirá el documento.

**Ref. 10.08:** “seguranca” - en esta parte del JSON se puede enviar un código de seguridad que el usuario debe informar al momento de firmar el documento. Vea a continuación qué información debe enviarse para que esto ocurra:

**Ref. 10.08.01:** “idMeioEnvio” - en este campo debe informarse cómo debe enviarse el código de seguridad al destinatario. Las opciones son:

&#x20;    \-> 1 = SMS **(Sólo para teléfonos de Brasil)**

&#x20;    \-> 2 = WhatsApp

&#x20;    \-> 3 = Correo Electrónico

&#x20;    \-> 4 = No enviar (Esta opción debe elegirse cuando quien está enviando el documento al destinatario informará el código de seguridad de otra forma, sin usar los medios de notificación de la plataforma ArqSIGN).

**Ref. 10.08.02:** “codigoSeguranca” - en este campo debe informarse el código de seguridad para el destinatario en cuestión.

**Ref. 10.08.03:** “codigoSegurancaEmail” - si se ha enviado en el campo “idMeioEnvio” la opción 3 = Email, se debe informar el email al cual la plataforma ArqSIGN enviará el código de seguridad.

**Ref. 10.08.04:** “codigoSegurancaTelefone” - si se ha enviado en el campo “idMeioEnvio” la opción 1 = SMS o 2 = WhatsApp, se debe informar el teléfono al cual la plataforma ArqSIGN enviará el código de seguridad.

**Ref. 10.08.05:** “reenviarCodigo” - si se ha enviado en el campo “idMeioEnvio” la opción 1 = SMS o 2 = WhatsApp, se debe informar en este campo si el destinatario, al recibir el documento para firmar, podrá solicitar el reenvío del código. Este reenvío se computará en los créditos de SMS y WhatsApp de la cuenta. Para permitir el reenvío del código, envíe la información 1 = True, para no permitir el reenvío, envíe la información 0 = False.

**Ref. 10.09:** “mensagemPersonalizada” - en esta parte del JSON se puede enviar un mensaje personalizado para el firmante en cuestión, si recibe el documento para firmar por correo electrónico.

**Ref. 10.09.01:** “titulo” - en este campo debe informarse el texto que será enviado como asunto del mensaje.

**Ref. 10.09.02:** “texto” - en este campo debe informarse el texto que será enviado como cuerpo del mensaje.

**Ref. 10.10:** “destinatariosEntradaDto” - en esta parte del JSON se deben enviar las configuraciones de datos que serán solicitados al firmante en el momento de la firma.

**Ref. 10.10.01:** “infComplNomeSignatarioObrigatorio” - envíe 1 = true para obligar al firmante a informar su nombre completo, envíe 0 = false para no obligar al firmante a informar su nombre completo.

**Ref. 10.10.02:** “infComplDocumentoSignatarioObrigatorio” - envíe 1 = true para obligar al firmante a informar un documento de identificación de PF, envíe 0 = false para no obligar al firmante a informar un documento de identificación de PF.

**Ref. 10.10.03:** “infComplRazaoSocialObrigatorio” - envíe 1 = true para obligar al firmante a informar el nombre de la empresa, envíe 0 = false para no obligar al firmante a informar el nombre de la empresa.

**Ref. 10.10.04:** “infComplIdentificadorObrigatorio” - envie 1 = true para obrigar o signatário a informar um documento de identificação de PJ, envie 0 = false para não obrigar o signatário a informar um documento de identificação de PJ.

**Ref. 10.10.05:** “idInfComplTipoDocumentoSignatarioPF” - neste campo deve ser informado o tipo de documento a ser informado como PF, as opções são:

&#x20;    \-> 1 = CPF

&#x20;    \-> 2 = CNH

&#x20;    \-> 3 = RG

&#x20;    \-> 4 = Outro

**Ref.10.10.06:** “infComplDocumentoNomePF” - quando no JSON, o campo “idInfComplTipoDocumentoSignatarioPF” estiver com o valor 4 = Outro, é necessário enviar neste campo um nome que irá identificar esta opção “Outro” para o signatário no momento da assinatura.

**Ref.10.10.07:** “idInfComplTipoDadosIndentificadorPF” - quando no JSON, o campo “idInfComplTipoDocumentoSignatarioPF” estiver com o valor 4 = Outro, é necessário enviar neste campo a informação se o documento de PF deve ser do tipo 1 = Texto ou 2 = Numérico.

**Ref.10.10.08:** “infComplQtdeCaracteresPF” - quando no JSON, o campo “idInfComplTipoDocumentoSignatarioPF” estiver com o valor 4 = Outro, é necessário enviar neste campo a quantidade de caracteres para a aplicação validar o documento de PF.

**Ref. 10.10.09:** “idInfComplTipoDocumentoSignatarioPJ” - neste campo deve ser informado o tipo de documento a ser informado como PJ, as opções são:

&#x20;    \-> 4 = Outro

&#x20;    \-> 5 = CNPJ

**Ref.10.10.10:** “infComplDocumentoNomePJ” - quando no JSON, o campo “idInfComplTipoDocumentoSignatarioPJ” estiver com o valor 4 = Outro, é necessário enviar neste campo um nome que irá identificar esta opção “Outro” para o signatário no momento da assinatura.

**Ref.10.10.11:** “idInfComplTipoDadosIndentificadorPJ” - quando no JSON, o campo “idInfComplTipoDocumentoSignatarioPJ” estiver com o valor 4 = Outro, é necessário enviar neste campo a informação se o documento de PJ deve ser do tipo 1 = Texto ou 2 = Numérico.

**Ref.10.10.12:** “infComplQtdeCaracteresPJ” - quando no JSON, o campo “idInfComplTipoDocumentoSignatarioPJ” estiver com o valor 4 = Outro, é necessário enviar neste campo a quantidade de caracteres para a aplicação validar o documento de PJ.

**Ref. 10.11:** “Anexos” - nesta parte do JSON devem ser enviadas as configurações de arquivos a serem solicitados aos signatários no momento da assinatura.

**Ref. 10.11.01:** “anexoDocumentoNome” – envie neste campo o nome do arquivo que deseja que o signatário faça o upload. Exemplo: Frente da Identidade, Selfie etc.

**Ref. 10.11.02:** “anexoObrigatorio” - envie 1 = true para obrigar o signatário a fazer o upload deste anexo, ou 0 = false para não obrigar.

**Ref. 10.11.03:** “anexoExibirTodosDestinatarios” - envie 1 = true para após a conclusão do processo de assinatura, este anexo estar disponível para todos os signatários ou envie 0 = false para este anexo estar disponível somente para você que enviou o documento para ser assinado e para quem fez o upload do anexo.

**Ref. 10.12:** “definirPosicaoAssinaturaAutomatica” - neste campo deve ser enviada a informação se a plataforma deverá ou não definir de forma automática o posicionamento da assinatura para o signatário.

{% hint style="warning" %}
<mark style="color:orange;">**No JSON, todos os destinatários com a ação de “Assinar Online” precisam ter o posicionamento da representação visual de forma automática ou manual. Para inserir o posicionamento automático da assinatura, a aplicação irá inserir uma página em branco ao final do arquivo com os locais onde todos os signatários assinarão. Desta forma, ao enviar um documento a ser assinado via API, deve-se deixar a aplicação definir o posicionamento da assinatura para todos os signatários ou para nenhum. Não é possível uma opção híbrida, um signatário se envia o posicionamento da assinatura e outro a aplicação escolhe automaticamente.**</mark>

<mark style="color:orange;">**Então neste campo teremos as seguintes opções:**</mark>

* <mark style="color:orange;">**Null: ao enviar este parâmetro como null, significa que a aplicação não irá definir o posicionamento da assinatura para os signatários de forma automática, ou seja, será necessário enviar os dados de posicionamento no JSON (definirPosicaoAssinaturaManual).**</mark>
* <mark style="color:orange;">**1 = PF: ao enviar este parâmetro com valor 1, significa que a aplicação ArqSign irá incluir uma página no final do arquivo com a definição automática da posição da assinatura do tipo Pessoa Física (PF).**</mark>
* <mark style="color:orange;">**2 = PJ: ao enviar este parâmetro com valor 2, significa que a aplicação ArqSign irá incluir uma página no final do arquivo com a definição automática da posição da assinatura do tipo Pessoa Jurídica (PJ).**</mark>
* <mark style="color:orange;">**3 = PF e PJ: ao enviar este parâmetro com valor 3, significa que a aplicação ArqSign irá incluir uma página no final do arquivo com a definição automática da posição para duas assinaturas, uma do tipo Pessoa Física (PF) e uma do tipo Pessoa Jurídica (PJ).**</mark>
{% endhint %}

**Ref. 10.13:** “definirPosicaoAssinaturaManual” - nesta parte do JSON devem ser enviados os dados de posicionamento da assinatura no documento. Esta parte deve ser enviada obrigatoriamente se no campo “definirPosicaoAssinaturaAutomatica”, tiver sido enviada a informação “Null”.

**Ref. 10.13.01:** “pessoaFisica” - se este signatário for assinar como pessoa física, envie nesta parte o posicionamento da assinatura em questão.

**Ref. 10.13.01.01:** “pagina” - envie o número da página onde a assinatura deve ser posicionada.

**Ref. 10.13.01.02:** “Altura” - envie a altura em milímetros do tamanho da caixa onde a assinatura será aplicada.

**Ref. 10.13.01.03:** “Largura” - envie a largura em milímetros do tamanho da caixa onde a assinatura será aplicada.

**Ref. 10.13.01.04:** “PosicaoX” - envie a posição em milímetros da borda esquerda da página até a borda esquerda da caixa da assinatura.

**Ref. 10.13.01.05:** “PosicaoY” - envie a posição em milímetros da borda superior da página até a borda superior da caixa da assinatura.

**Ref. 10.13.02:** “pessoaJuridica” - se este signatário for assinar como pessoa jurídica, envie nesta parte o posicionamento da assinatura em questão.

**Ref. 10.13.02.01:** “pagina” - envie o número da página onde a assinatura deve ser posicionada.

**Ref. 10.13.02.02:** “Altura” - envie a altura em milímetros do tamanho da caixa onde a assinatura será aplicada.

**Ref. 10.13.02.03:** “Largura” - envie a largura em milímetros do tamanho da caixa onde a assinatura será aplicada.

**Ref. 10.13.02.04:** “PosicaoX” - envie a posição em milímetros da borda esquerda da página até a borda esquerda da caixa da assinatura.

**Ref. 10.13.02.05:** “PosicaoY” - envie a posição em milímetros da borda superior da página até a borda superior da caixa da assinatura. Na figura abaixo está a representação visual das medidas que precisam ser identificadas no seu modelo de documento (Altura, Largura, PosicaoX e PosicaoY).&#x20;

<figure><img src="../../../../.gitbook/assets/api05.png" alt=""><figcaption></figcaption></figure>

Para saber como tirar estas medidas, assista ao vídeo abaixo:

{% embed url="https://www.youtube.com/watch?v=8GPh7jtpHHY" %}

**Ref. 11:** “Documento” - nesta parte do JSON deve ser enviado o arquivo a ser assinado. O arquivo deve ser no formato PDF limitado a 100 MB.

**Ref. 11.01:** “arquivo” - envie neste campo o arquivo em Base64.

**Ref. 11.02:** “nomeComExtensao” - envie o nome do arquivo com sua extensão.

***

## Retorno <a href="#toc112750306" id="toc112750306"></a>

<figure><img src="../../../../.gitbook/assets/api06.png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### Detalhamento do Retorno

**Ref. 01 – Código 201:** Como retorno de sucesso, a aplicação retornará o código 201 e o GUID gerado para o processo. O Guid deve ser armazenado na aplicação do Cliente de forma a possibilitar a usar os métodos de GET​/api​/v1​/processo​/{idprocesso} e GET​/api​/v1​/processo​/{idProcesso}​/status-do-processo

**Ref. 02 – Código 400:** _Mensagem de item obrigatório_: Esta mensagem será exibida no singular ou plural quando um ou mais itens obrigatórios não tiver sido enviado na chamada da API.

**Ref. 03 – Código 400:** _Mensagem de formato incorreto:_ Esta mensagem será exibida no singular ou plural quando um ou mais itens estiverem sido enviados com formato incorreto.

**Ref. 04 – Código 400:** _Mensagem de Ids inexistente:_ Esta mensagem será exibida no singular ou plural quando um ou mais Id enviado não existir.

**Ref. 05 – Código 400:** _Mensagem de parâmetro incorreto ou é inexistente:_ Quando a chamada é feita com algum parâmetro escrito errado ou parâmetro que não existe no método.

**Ref. 06 – Código 400:** _Mensagem de saldo insuficiente:_ Esta mensagem será exibida quando a conta não possuir saldo suficiente para o envio por E-mail ou WhatsApp ou SMS.

**Ref. 07 – Código 400:** _Mensagem de arquivo no formato inválido:_ Esta mensagem será exibida quando o usuário informar um arquivo com extensão diferente de PDF.

**Ref. 08 – Código 400:** _Mensagem de tamanho do arquivo:_ Esta mensagem será exibida quando o usuário informar um arquivo com tamanho maior que 100MB.

**Ref. 09 - Código 400:** _Mensagem de conta bloqueada:_ Esta mensagem será exibida quando a conta estiver bloqueada.

**Ref. 10 - Código 401:** _Mensagem de usuário da API não autorizado:_ AppKey inválida ou não localizada.

***

## Comparativo JSON V1xV2

### Forma de envio&#x20;

Na **v1** era necessário informar no parâmetro “**idFormaEnvio**”, qual seria a forma de envio no processo. Agora na **V2** este parâmetro não existe. Portanto essa informação fica subentendida no sistema, quando se informa um e-mail ou telefone.

<mark style="color:red;">**V1**</mark>

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (454).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

</div>

<mark style="color:green;">**V2**</mark>

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (455).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

</div>



### Usar página automática&#x20;

o nome do parâmetro mudou.

<mark style="color:red;">**V1**</mark>&#x20;

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (456).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

</div>

<mark style="color:green;">**V2**</mark>

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (457).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

</div>

### Definição da posição de assinatura manual

Na **V2**, deve ser configurado dados de posição da assinatura manual para cada documento do processo. Portanto foi adicionado o parâmetro “**documentoDeOrdem**” dentro do objeto “**definirPosicaoAssinaturaManual**”.

<mark style="color:red;">**V1**</mark>

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (458).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

</div>

<mark style="color:green;">**V2**</mark>

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (459).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

</div>

### Tipo de Assinatura

Na **V1** o Tipo de Assinatura, é informado através do parâmetro “**idTipoAssinatura**” dentro do objeto de signatário.

Já na **V2**, este parâmetro se tornou uma propriedade independente (não fica dentro de nenhum objeto).

<mark style="color:red;">**V1**</mark>

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (460).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

</div>

<mark style="color:green;">**V2**</mark>

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (461).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

</div>

### Dados complementares&#x20;

Na **V1** os dados complementares de Pessoa Física e Jurídica eram informados dentro do objeto de Signatário por meio do parâmetro “**destinatariosEntradaDto**”. E na **V2** esses dados também se tornaram independentes e são informados no objeto "**assinaturaEletronica**".

<mark style="color:red;">**V1**</mark>

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (462).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

</div>

<mark style="color:green;">**V2**</mark>

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (463).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

</div>

### Documento por processo

Na **V1** é possível enviar apenas 1 documento por processo.

E na **V2** é possível enviar vários documentos em um único processo.

<mark style="color:red;">**V1**</mark>

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (464).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

</div>

<mark style="color:green;">**V2**</mark>

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (465).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

</div>

### Retorno da requisição

O retorno da requisição também mudou. Na **V2** é são retornados os dados de Id do processo, Id’s dos documentos e seus respectivos nomes.

<mark style="color:red;">**V1**</mark>

É retornado apenas o ID do Processo.

<mark style="color:green;">**V2**</mark>

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (466).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

</div>
