# 🔳 Flujo ideal considerando algunos métodos disponibles

Las funciones fundamentales de una API comprenden la obtención, el envío, la modificación y la eliminación de información. Esto ocurre cuando una aplicación cliente o un socio envía una solicitud a la aplicación ArqSign, que a su vez genera una respuesta.

A continuación, mostramos un flujo ideal para la implementación de tres métodos de los disponibles:

<figure><img src="../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

**FASE 01:** La aplicación del cliente llama al método [<mark style="color:blue;">**POST/api/v1/processo/enviar-documento-para-assinar**</mark>](metodos-disponibles-en-la-api/post-api-v1-processo-enviar-documento-para-assinar.md) para enviar un documento a ser firmado. Con la respuesta de éxito, la API devolverá el ID del proceso generado y debes guardarlo para usar este ID como parámetro en otros métodos.

**FASE 02:**La aplicación del cliente llama al método [**GET/api/v1/processo/{idProcesso}/status-do-processo**](metodos-disponiveis-na-api/get-api-v1-processo-idprocesso-status-do-processo.md) para monitorear el estado del proceso generado en la Fase 01. Aconsejamos llamar a este método un máximo de una vez al día, no es necesario llamarlo todo el tiempo, ya que el estado de un proceso solo se considerará concluido después de la firma del documento por todos los firmantes.um processo somente será concluído após a assinatura do documento por todos os signatários.

**FASE 03:**Una vez que el proceso tenga el estado “Concluido”, puedes pasar a la fase 03, cuando llamarás al método [**GET/api/v1/processo/{idprocesso}**](metodos-disponiveis-na-api/get-api-v1-processo-idprocesso.md) para obtener los datos completos del proceso y el archivo firmado.
