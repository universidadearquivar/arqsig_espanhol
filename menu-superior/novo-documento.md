# ➕ Nuevo Documento

En la pantalla **Nuevo Documento**, el usuario podrá registrar uno o más documentos que serán enviados a los firmantes para su firma.

## Etapa 1: Agregar Documentos y Destinatarios

### A. Agregar Documentos (Cargar archivos)

Para incluir los documentos que deberán ser firmados, arrastre los archivos deseados hasta el campo de inclusión de documentos o selecciónelos para cargar desde un directorio de su dispositivo.

Se pueden incluir más de un archivo en el mismo proceso de firma. En este caso, la opción "Agrupar los archivos en un único documento" estará disponible y podrá ser seleccionada o deseleccionada.

<figure><img src="../.gitbook/assets/image (124).png" alt=""><figcaption></figcaption></figure>

Cuando este campo esté **marcado**, ArqSign mostrará los archivos agrupados en el área de listado, donde se permite alterar el orden de los documentos, haciendo clic y arrastrándolos a la posición deseada. En este caso, no se permite cambiar el nombre de cada uno de los archivos, solo el nombre del proceso.

<figure><img src="../.gitbook/assets/image (114).png" alt=""><figcaption></figcaption></figure>

Para eliminar un archivo, haga clic en el ícono de la papelera disponible para cada uno de los archivos en la pantalla.

Cuando este campo esté deseleccionado, ArqSign mostrará los archivos desagrupados en el área de listado, permitiendo que se alteren tanto el orden como el nombre de los archivos.

<figure><img src="../.gitbook/assets/image (115).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Se permiten archivos de las siguientes extensiones:**</mark>

<mark style="color:orange;">**Documento: .doc, .docx, .pdf, .txt.**</mark>

<mark style="color:orange;">**Imagen: .jpg, .jpeg, .png, .tif, .tiff**</mark>

<mark style="color:orange;">**Presentación: .ppt, .pptx**</mark>&#x20;

<mark style="color:orange;">**Hoja de cálculo: .csv, .xls, .xlsx**</mark>

<mark style="color:orange;">**Cada archivo puede tener hasta 35 MB o hasta 2000 páginas, no pudiendo superar 100 MB en total.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (116).png" alt=""><figcaption></figcaption></figure>

En el campo **“Nombre del Proceso de Firma”,** es posible editar el nombre del proceso que abarca los archivos agrupados; modifíquelo según sea necesario.

En el campo “Carpeta del Documento”, seleccione la carpeta en la que se alojará el documento. Las carpetas en las que se podrán almacenar los documentos deben ser creadas en el menú [<mark style="color:blue;">**Directorios > Documentos**</mark>](../diretorios/documentos/). Por defecto, se crea una carpeta con el nombre del usuario, que debe ser seleccionada si no existe ninguna otra.

<figure><img src="../.gitbook/assets/image (117).png" alt=""><figcaption></figcaption></figure>

Por último, para programar la renovación de los documentos que se están registrando de forma automática, seleccione la casilla del campo **“Programar renovación \_\_\_ meses después de la conclusión de las firmas”**, indicando la cantidad de meses en los que desea ser avisado sobre la renovación del proceso. Una vez que las firmas del primer envío se hayan completado, el sistema comenzará a contar el plazo determinado y, cuando se alcance el período de renovación, el responsable de los documentos (remitente) recibirá una notificación informando que los documentos del proceso están listos para ser renovados.

<figure><img src="../.gitbook/assets/image (118).png" alt=""><figcaption></figcaption></figure>

### Configuraciones Avanzadas

Las configuraciones avanzadas son ajustes relativos al documento. Se pueden ajustar tanto para todos los documentos, es decir, establecer un estándar configurado para cada vez que sea necesario solicitar firmas, como configurar opciones relacionadas con un documento específico en particular. Para acceder a la lista completa de las opciones que se pueden configurar en los documentos, acceda al menú [<mark style="color:blue;">Administración > Cuenta > Configuraciones</mark>](../administracao/administracao/conta.md#aba-configuracoes). A continuación, conozca todas las opciones generales configurables:

* **Tiempo para la expiración del documento después del envío:** En este campo, el usuario debe indicar el plazo (en días) de expiración del documento, es decir, el límite para que los destinatarios lo firmen.

{% hint style="warning" %}
<mark style="color:orange;">Si este campo no se modifica, se completará con el valor predeterminado. El valor predeterminado del sistema es de 120 días, pero este valor puede ser cambiado en el menú</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**Administración > Cuenta > Configuraciones**</mark><mark style="color:orange;">.</mark>
{% endhint %}

* **Aviso antes de la expiración:** En este campo se debe indicar el plazo (en días) en el que el sistema deberá enviar a los destinatarios que aún no han firmado un aviso sobre la expiración del documento.
* **Activar recordatorios:** Al activar esta opción, el sistema enviará a los destinatarios recordatorios para que realicen la firma del documento. Estos recordatorios se enviarán solo a los firmantes que aún no han firmado el documento. Por defecto, esta opción estará marcada.
* **Enviar recordatorios a los destinatarios cada:** En este campo se debe especificar cada cuánto tiempo (en días) el sistema deberá enviar los recordatorios de firma a los destinatarios que aún no han firmado.
* **Obligar al firmante a leer los documentos antes de firmar:** Esta configuración obliga a la lectura de los documentos del proceso. Esta información estará marcada o desmarcada, según la configuración de la cuenta.
* **Generar QRCode de acceso del documento en el Registro de Firmas:** Al activar esta opción, se generará un QRCode en el documento de registro de firmas. Por defecto, esta opción estará desmarcada.

Al pasar el mouse sobre la opción de "Configuraciones avanzadas", se presenta un Tooltip con una vista previa de las configuraciones realizadas.

<figure><img src="../.gitbook/assets/image (776).png" alt=""><figcaption></figcaption></figure>

Para editar puntualmente las configuraciones de un archivo determinado, haga clic en **Ajustes Avanzadas**, como se muestra en la imagen a continuación.

<figure><img src="../.gitbook/assets/image (123).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (127).png" alt=""><figcaption></figcaption></figure>

### B. Destinatarios

En el campo “Destinatarios”, complete los campos relacionados con los firmantes que recibirán el documento y participarán en el proceso de firma. Es necesario realizar las configuraciones descritas a continuación para cada uno de los destinatarios.

<figure><img src="../.gitbook/assets/image (129).png" alt=""><figcaption></figcaption></figure>

Es posible agregar un destinatario guardado a partir de la lista de contactos, haciendo clic en el ícono **“Agregar destinatario de mis contactos”**.

{% hint style="info" %}
<mark style="color:blue;">**Importante:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">la lista de contactos debe ser creada anteriormente en el menú</mark> [<mark style="color:blue;">**Mi Perfil**</mark>](meu-perfil.md)<mark style="color:blue;">.</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (131).png" alt=""><figcaption></figcaption></figure>

Al hacer clic en este botón, se muestra la lista. Para agregar los destinatarios deseados, seleccione los que desee marcando la casilla junto al nombre y haga clic en “Agregar Destinatarios”.

<figure><img src="../.gitbook/assets/image (132).png" alt="" width="365"><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

Al marcar la casilla **“Firmar en el orden a continuación”**, el documento será enviado a los destinatarios en el orden definido en el campo **“Orden”**, que aparecerá en la parte superior de **“Datos del Destinatario”**. Al establecer esta opción, un usuario solo recibirá el documento cuando el anterior complete su acción de firma.

{% hint style="warning" %}
<mark style="color:orange;">**Si el usuario anterior solo tuvo una acción de visualización, el siguiente firmante recibirá el documento cuando el último firmante anterior a él complete la firma.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (134).png" alt=""><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

**Nombre del Destinatario:** Indique el nombre del destinatario.

**Enviar por:** Seleccione si el documento será enviado por correo electrónico o WhatsApp al destinatario.

{% hint style="warning" %}
<mark style="color:orange;">**La opción de envío por WhatsApp solo será exhibida si la cuenta del usuario tiene créditos de mensajes de WhatsApp.**</mark>
{% endhint %}

Dependiendo de la opción elegida anteriormente, indique el correo electrónico o el número de teléfono del destinatario para el envío del documento.

<figure><img src="../.gitbook/assets/image (136).png" alt=""><figcaption></figcaption></figure>

**Este destinatario irá:** Indique si el destinatario firmará el documento en línea como Persona Física, Jurídica o ambas, o si solo recibirá una copia del documento al final del proceso de firmas.

<figure><img src="../.gitbook/assets/image (137).png" alt="" width="375"><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

Si se ha determinado que el destinatario firmará como persona física o jurídica, es necesario definir su rol de firmante en el proceso. Seleccione entre uno o más roles listados o agregue un “Rol del Firmante” personalizado haciendo clic en “Agregar rol”.

<figure><img src="../.gitbook/assets/image (138).png" alt="" width="306"><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

Los roles del firmante presentados aquí se crean previamente en el menú [<mark style="color:blue;">Administración > Cuenta > Pestaña Configuraciones > Rol del Firmante</mark>](https://app.gitbook.com/o/Ai1YjbPQxIuvTaVzoZ4H/s/zDlPVk00J5AKVvFiB3dg/)**.** De manera predeterminada, la plataforma muestra los roles de “Contratada”, “Contratante”, “Fiador” y “Arrendatario”, pero es posible editar o eliminar estos roles, además de crear otros si es necesario.

<figure><img src="../.gitbook/assets/image (139).png" alt="" width="338"><figcaption></figcaption></figure>

**Tipo de Firma:** Seleccione si el destinatario deberá utilizar firma electrónica o un certificado digital para firmar el documento.

<figure><img src="../.gitbook/assets/image (140).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">**FIRMA ELECTRÓNICA VS FIRMA DIGITAL (ICP Brasil y Otros ICP)**</mark>

<mark style="color:blue;">La firma electrónica no necesita un certificado digital y se utiliza principalmente para firmar contratos y documentos entre entidades privadas (B2B, B2C).</mark>

<mark style="color:blue;">La firma digital, por otro lado, requiere un certificado digital y es más utilizada para la emisión de facturas y transacciones con el gobierno.</mark>

<mark style="color:blue;">En la Plataforma ArqSign, al configurar un flujo de firmas, puedes determinar qué tipo de firma debe ejecutarse para cada destinatario eligiendo entre:</mark>

<mark style="color:blue;">a)</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Firma electrónica**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">(ArqSign produce firmas electrónicas avanzadas con validez jurídica de acuerdo con la MP 2.200-2 de 24/08/2001 y la Ley 14.063 de 23/11/2020). Siempre que un firmante utiliza la firma electrónica, ArqSign aplica un certificado digital propio de la plataforma, capturando el</mark> <mark style="color:blue;"></mark>_<mark style="color:blue;">Hash</mark>_ <mark style="color:blue;"></mark><mark style="color:blue;">(identificación única) del archivo, verificando su integridad y anexando al certificado la identificación del firmante.</mark>

<mark style="color:blue;">b)</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Firma digital – ICP-Brasil u Otros**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">(ArqSign produce firmas digitales cualificadas de acuerdo con la MP 2.200-2 de 24/08/2001 y la Ley 14.063 de 23/11/2020). Cuando el usuario ya posee un certificado digital y desea utilizarlo para firmar a través de ArqSign, este certificado se usa para verificar la integridad de la firma y identificar al usuario como firmante en el documento.</mark>
{% endhint %}

**Representación Visual Firma**: Seleccione cuál debe ser la representación visual utilizada por el destinatario en el momento de la firma. Al optar por la primera opción (Estándar, Dibujo o Imagen), podrá utilizar cualquiera de las representaciones; en el caso de las demás opciones, la utilización quedará restringida a la representación seleccionada en este momento.

<figure><img src="../.gitbook/assets/image (141).png" alt="" width="375"><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

Al marcar la opción **“Guardar este destinatario en mi lista de contactos”**, los datos proporcionados del destinatario se guardarán automáticamente en la lista de contactos del usuario.

<figure><img src="../.gitbook/assets/image (142).png" alt=""><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

**Ícono “Código de Seguridad”**: Al hacer clic en este ícono, se creará un código numérico que se enviará al destinatario para que pueda acceder al documento. El código puede ser generado automáticamente por el sistema o informado manualmente por el usuario.

<figure><img src="../.gitbook/assets/image (143).png" alt=""><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

Después de generar el código, elija si se enviará por correo electrónico, WhatsApp o SMS e informe el correo electrónico o número de teléfono para el envío. También es posible no enviar el código, dejando a cargo del usuario informarlo al destinatario de la forma que prefiera. Para eliminar el código creado, simplemente haga clic en “Eliminar Código de Seguridad”.

<figure><img src="../.gitbook/assets/image (144).png" alt=""><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

Si se selecciona la opción de envío por WhatsApp, es posible permitir que el destinatario solicite el reenvío del código, marcando la casilla de verificación **“Permitir que este destinatario pueda solicitar el reenvío del código de seguridad”**.

{% hint style="warning" %}
<mark style="color:orange;">**Cada reenvío del código de seguridad solicitado por el destinatario consumirá un crédito de WhatsApp de la cuenta del usuario que está enviando el documento.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (146).png" alt=""><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

**Ícono Mensaje Privado**: Al hacer clic en este ícono, será posible insertar un mensaje que se enviará al destinatario junto con el documento. Para ello, complete los campos “Asunto” y “Mensaje”. Si desea eliminar el mensaje, haga clic en **“Eliminar Mensaje Privado”**.

<figure><img src="../.gitbook/assets/image (147).png" alt=""><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

Los elementos **Código de Seguridad** y **Mensaje Privado** son expandibles y, cuando están recogidos, cuentan con el ícono de edición, señalizando al usuario que pueden ser modificados.

<figure><img src="../.gitbook/assets/image (148).png" alt=""><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

Para insertar otros destinatarios, haga clic en el botón “Agregar Nuevo Destinatario”. Si desea incluirse a sí mismo como destinatario, haga clic en **“Añadirme como destinatario”**. Los campos de nombre y correo electrónico se completarán automáticamente con la información registrada en su perfil de usuario, y el campo “Enviar por” se llenará con la opción “Correo electrónico”.

<figure><img src="../.gitbook/assets/image (149).png" alt=""><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

### C. Mensaje Predeterminado

En el campo “Mensaje Predeterminado”, se puede mantener el mensaje predeterminado creado por la plataforma o seleccionar en la lista su mensaje predeterminado, creado en "[<mark style="color:blue;">Mi Perfil</mark>](meu-perfil.md#mensagem-padrao)", que se enviará a todos los destinatarios, completando los campos “Asunto” y “Mensaje”.

{% hint style="warning" %}
<mark style="color:orange;">**En el caso de destinatarios que tengan los campos de Mensaje Personalizado completados, se enviará el mensaje informado en sustitución del mensaje predeterminado.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (150).png" alt=""><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

Después de concluir estas configuraciones, haga clic en “Siguiente” para continuar a la próxima etapa, “Concluir Más Tarde” para guardar el flujo como borrador o “Descartar” para cancelar el registro.

<figure><img src="../.gitbook/assets/image (151).png" alt=""><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

***

## Etapa 2: Configurar Campos

En la siguiente etapa se mostrarán los documentos que se han insertado en la etapa anterior en formato PDF, y se deberán configurar los campos de firma, información de llenado y adjuntos.

**Proceso con un documento o más documentos agrupados**

Cuando el proceso tiene uno o más documentos agrupados, el sistema muestra el nombre del proceso.

<figure><img src="../.gitbook/assets/image (152).png" alt=""><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

**Proceso con más de un documento no agrupado**

Cuando el proceso tiene uno o más documentos no agrupados, el sistema muestra:



* En la parte superior de la pantalla, el **nombre del documento** que se está exhibiendo;
* En la esquina izquierda de la pantalla, **la lista de documentos del proceso** ordenados según la configuración de orden definida en la [<mark style="color:blue;">Etapa 01</mark>](novo-documento.md#etapa-1-adicionar-documentos-e-destinatarios), indicando si el documento está siendo visualizado o no. Al hacer clic en el documento, el sistema lo mostrará en la pantalla.

<figure><img src="../.gitbook/assets/image (153).png" alt=""><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

### C**ampos de Firma**

#### R**epresentación de la firma**

Al hacer clic en el documento, el sistema muestra el modal de configuración de la representación visual, listando a los signatarios pendientes de configuración de la representación de la firma ordenados alfabéticamente o según el orden de firma definido en la [<mark style="color:blue;">etapa 01</mark>](novo-documento.md#etapa-1-adicionar-documentos-e-destinatarios).

Para cada documento listado, el sistema muestra la(s) respectiva(s) representación(es) para cada signatario(s) según el tipo de firma definida en la [<mark style="color:blue;">etapa 01</mark>](novo-documento.md#etapa-1-adicionar-documentos-e-destinatarios) (campo "Este Destinatario irá"), permitiendo al usuario configurar la representación para cada signatario(s) con la acción de firmar en línea en cada documento.

<figure><img src="../.gitbook/assets/image (154).png" alt=""><figcaption></figcaption></figure>

Al incluir la configuración de la representación visual, la aplicación muestra la representación en el documento en la posición que el usuario insertó, permitiendo ajustar el tamaño y/o eliminar la representación de la firma que está insertada en el documento.

<figure><img src="../.gitbook/assets/Animação (1).gif" alt=""><figcaption></figcaption></figure>

Si en la [<mark style="color:blue;">Etapa 1</mark>](novo-documento.md#b.-destinatarios) se ha definido que el destinatario firmará como persona física y jurídica, se mostrarán dos cuadros con el nombre del destinatario en el mismo color. Los cuadros de cada uno de los destinatarios se mostrarán en colores diferentes para señalar visualmente dónde cada uno deberá firmar.

**Modal de representación visual de firma para proceso con un documento o más documentos agrupados**\
Cuando el proceso tiene un documento o más documentos agrupados, el sistema lista las representaciones de los destinatarios, según el tipo de persona (PF y/o PJ), mostrando una barra de desplazamiento en la modal.

<figure><img src="../.gitbook/assets/image (155).png" alt=""><figcaption></figcaption></figure>

**Modal de representación visual de firma para procesos con más de un documento no agrupados**

Cuando el proceso tiene **más de un documento**, el sistema muestra un **"carrusel"**, permitiendo la navegación entre los documentos y los firmantes.

<figure><img src="../.gitbook/assets/image (486).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (488).png" alt="" width="283"><figcaption></figcaption></figure>

Al concluir la configuración de la firma de todos los firmantes en el documento, el sistema señala el documento como configuración de la representación concluida, marcando el ícono de verificación en verde en la esquina izquierda de la pantalla.

Al concluir la configuración de la firma del firmante en todos los documentos, el sistema señala a este firmante como configuración de la representación concluida, marcando el ícono de verificación en verde frente al nombre de cada firmante.Parte inferior do formulário

<figure><img src="../.gitbook/assets/image (489).png" alt=""><figcaption></figcaption></figure>

### D**atos de Firma y Adjuntos**

En la esquina superior derecha de la pantalla, se muestra el campo "**Configuraciones para**", donde se presenta el nombre del destinatario que está seleccionado para la configuración. Cada destinatario tiene un color asignado automáticamente por la plataforma, y al lado de este ícono, aparece un símbolo de "check", que cambia de color y se vuelve verde para señalar que la **Información Complementaria de Firma** ha sido incluida o permanece en gris cuando no ha sido incluida.

<figure><img src="../.gitbook/assets/image (490).png" alt=""><figcaption></figcaption></figure>

Si no hay un orden de firmas configurado en la Etapa 1, el ítem "Configuraciones para" muestra la lista de los firmantes ordenados alfabéticamente. Si ya hay un orden de firmas configurado, la lista de los firmantes estará agrupada por orden de firmas y ordenada alfabéticamente.

<figure><img src="../.gitbook/assets/image (491).png" alt="" width="286"><figcaption></figcaption></figure>

### **Envío Simplificado**

En caso de que el usuario no desee insertar las firmas manualmente en el documento, se puede seleccionar la opción **Envío Simplificado**.

<figure><img src="../.gitbook/assets/image (492).png" alt=""><figcaption></figcaption></figure>

El **Envío Simplificado** permite al usuario enviar el proceso sin el ajuste manual de la posición de la firma; de este modo, la plataforma inserta automáticamente una página al final del documento con las representaciones de las firmas, considerando las configuraciones definidas anteriormente en la inserción de los documentos y las siguientes reglas:

{% hint style="info" %}
* **Se el campo "Agrupar los archivos en único documento" de la** [<mark style="color:blue;">**Etapa 1**</mark>](https://app.gitbook.com/o/Ai1YjbPQxIuvTaVzoZ4H/s/zDlPVk00J5AKVvFiB3dg/) **está desmarcado:**

La plataforma **inserta una página al final de cada documento** con la posición de la firma de cada destinatario con la acción de Firmar en Línea, de acuerdo con el tipo de firma de cada uno (Persona Física y/o Persona Jurídica) configurada en el campo "Este Destinatario irá".

* **Se el campo "Agrupar los archivos en único documento" de la** [<mark style="color:blue;">**Etapa 1**</mark>](novo-documento.md#etapa-1-adicionar-documentos-e-destinatarios) **está marcado:**&#x20;

La plataforma **inserta una página al final del documento** con la posición de la firma de cada destinatario con la acción de Firmar en Línea, de acuerdo con el tipo de firma de cada uno (Persona Física y/o Persona Jurídica) configurada en el campo "Este Destinatario irá".
{% endhint %}

{% hint style="danger" %}
<mark style="color:red;">Caso el usuario haya optado anteriormente por la opción de</mark> <mark style="color:red;"></mark><mark style="color:red;">**configurar la firma manualmente**</mark> <mark style="color:red;"></mark><mark style="color:red;">en algún documento del proceso, el sistema muestra un mensaje de confirmación de envío simplificado. Al confirmar, los campos insertados manualmente serán eliminados y todas las firmas se posicionarán en la página automática generada por la plataforma.</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (493).png" alt=""><figcaption></figcaption></figure>

### Información Complementaria de Firma

El campo "**Configuraciones para**" muestra el nombre de los destinatarios seleccionados para la configuración con el ícono del color definido por la plataforma para el destinatario, señalizando si la configuración de los datos complementarios y/o anexos ha sido incluida o no.

<figure><img src="../.gitbook/assets/image (494).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (497).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">• Si</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**no hay**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">un orden de firmas configurado, la plataforma lista a los firmantes ordenados alfabéticamente.</mark>

<mark style="color:blue;">• Si</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**hay**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">un orden de firmas configurado, la plataforma lista a los firmantes agrupados por orden de firmas y alfabéticamente.</mark>
{% endhint %}

Dependiendo del tipo de firma definido para el destinatario en la [<mark style="color:blue;">Etapa 1</mark>](novo-documento.md#b.-destinatarios), se mostrarán los campos **“Información Complementaria de Firma”**. Estos campos solo se mostrarán si en la[ <mark style="color:blue;">Etapa 1, en el campo “Tipo de Firma”</mark>](novo-documento.md#b.-destinatarios), se ha elegido la opción “Firma Electrónica”.

Si la firma es como Persona Física, es posible exigir al destinatario datos como nombre y documento, marcando la opción “Nombre de la Persona Física” como llenado obligatorio y seleccionando uno de los documentos de la lista “Documento de la Persona Física”.

<figure><img src="../.gitbook/assets/image (498).png" alt="" width="225"><figcaption></figcaption></figure>

Para exigir un documento, seleccione la opción deseada entre CPF, CNH, C.I. u otros.

<figure><img src="../.gitbook/assets/image (499).png" alt="" width="256"><figcaption></figcaption></figure>

ADespués de seleccionar el tipo de documento que se exigirá al destinatario en la firma, informe el número del documento. En el momento de la firma, el destinatario deberá informar exactamente el número definido en este momento si se seleccionó la opción **"Llenado Obligatorio"**. Al seleccionar la opción **"Usar el valor informado en el campo para validar el CPF completado por el firmante durante la firma"**, automáticamente el campo será de llenado obligatorio y será validado por la plataforma para continuar con la firma.

En el momento de la firma, si el destinatario utiliza un número diferente al informado por el remitente en la configuración, se mostrará el siguiente error en la pantalla:

<figure><img src="../.gitbook/assets/image (500).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
<mark style="color:orange;">Los procesos configurados con esta validación de llenado de campo no se listan para</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**"Firma en Lote"**</mark><mark style="color:orange;">. Los documentos de estos procesos estarán disponibles para firma en la</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**"Bandeja de Entrada"**</mark><mark style="color:orange;">.</mark>
{% endhint %}

Si se selecciona esta última opción "otros", será necesario informar el nombre del documento, si es del tipo texto o numérico y la cantidad de caracteres.

<figure><img src="../.gitbook/assets/image (501).png" alt=""><figcaption></figcaption></figure>

Si la firma es como Persona Jurídica, es posible exigir al destinatario la razón social de la empresa y algún documento, marcando las opciones “Razón Social de la Persona Jurídica” y “Documento de la Persona Jurídica” como de llenado obligatorio.

<figure><img src="../.gitbook/assets/image (502).png" alt=""><figcaption></figcaption></figure>

Después de seleccionar el tipo de documento que se exigirá al destinatario en la firma, informe el número del documento. En el momento de la firma, el destinatario deberá informar exactamente el número definido en este momento si se selecciona la opción **"Llenado Obligatorio"**. Al seleccionar la opción **"Usar el valor informado en el campo para validar el CNPJ completado por el firmante durante la firma"**, automáticamente el campo será de llenado obligatorio y será validado por la plataforma para continuar con la firma.

En el momento de la firma, si el destinatario utiliza un número diferente al informado por el remitente en la configuración, se mostrará el siguiente error en la pantalla:

<figure><img src="../.gitbook/assets/image (503).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">Los procesos configurados con esta validación de llenado de campo no se listan para</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**"Firma en Lote"**</mark><mark style="color:orange;">. Los documentos de estos procesos estarán disponibles para firma en la</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**"Bandeja de Entrada".**</mark>
{% endhint %}

Para exigir un documento, seleccione la opción deseada entre CNPJ u otros. Si se selecciona la opción "otros", será necesario informar el nombre del documento, si es del tipo texto o numérico, y la cantidad de caracteres.

<figure><img src="../.gitbook/assets/image (504).png" alt="" width="282"><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>

### Anexos

En el campo “Anexos” en el lado izquierdo de la pantalla, se mostrarán configuraciones que permitirán a los destinatarios adjuntar otros archivos al documento en el momento de la firma. Para ello, marque la opción **“Solicitar adjuntar documentos”**.

Informe el nombre del anexo que se solicitará y defina si será de llenado obligatorio y si todos los destinatarios participantes en el flujo de firma podrán visualizar el archivo adjuntado por el destinatario.

Es posible solicitar más de un anexo haciendo clic en el ícono **“Añadir”.**

<figure><img src="../.gitbook/assets/image (505).png" alt=""><figcaption></figcaption></figure>

Al hacer clic en “Descartar”, el flujo será excluido. Al hacer clic en “Concluir Más Tarde”, el flujo se guardará en la carpeta de Borradores. Para editar el documento o los destinatarios, haga clic en “Volver a la Etapa Anterior”. Finalizada la configuración de la Etapa 2, haga clic en “Enviar” para enviar el documento para la firma de los destinatarios.

<figure><img src="../.gitbook/assets/image (506).png" alt=""><figcaption><p>Haga clic en la imagen para ampliar.</p></figcaption></figure>
