# ✉️ Caja de Entrada

En la Caja de Entrada se listan todos los documentos en los que el usuario participa en el proceso de firma como signatario, es decir, como firmante a través de la Plataforma ArqSign.

El signatario de un proceso de firma también puede ser el remitente del documento, y en este caso, el documento se mostrará tanto en la Caja de Entrada como en el [<mark style="color:blue;">menú Enviados</mark>](enviados.md).

{% hint style="warning" %}
<mark style="color:orange;">**No se mostrarán en la Caja de Entrada los documentos que ya hayan expirado, es decir, cuyo plazo para firma haya finalizado.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (585).png" alt=""><figcaption></figcaption></figure>

Al hacer clic en un documento, se abrirá la pantalla de visualización del documento, que muestra el documento enviado, su estado y fecha de vencimiento. En la esquina derecha de la pantalla se presentan las informaciones de los signatarios, como datos personales, rol del signatario y estado de la firma.

<figure><img src="../.gitbook/assets/image (586).png" alt=""><figcaption></figcaption></figure>

***

## Columnas de la pantalla principal - Caja de Entrada

<figure><img src="../.gitbook/assets/image (587).png" alt=""><figcaption></figcaption></figure>

**Columna Nombre del Documento:** En esta columna se muestran el nombre del documento y el nombre del signatario. Si hay más de un signatario, se mostrará el nombre del primero y la cantidad de otras personas que deberán firmar.

**Columna Responsable:** En esta columna se presentan el nombre y el correo electrónico de quien envió el documento (remitente).

**Columna Estado:** Los posibles estados para un documento son: "Esperando" (ningún participante ha firmado el documento hasta el momento), "En proceso" (uno o más participantes ya han firmado el documento, pero aún faltan firmas), y "Concluido" (todos los participantes ya han firmado el documento). Al pasar el mouse sobre el estado, se muestran informaciones sobre qué signatarios aún tienen pendiente la firma y quiénes ya la han completado, además de los datos de estos signatarios.

<figure><img src="../.gitbook/assets/image (588).png" alt=""><figcaption></figcaption></figure>

**Columna Tamaño:** En esta columna se muestra el tamaño del archivo del documento.

**Columna Carpeta:** En esta columna se muestra la carpeta del directorio donde se almacena el documento. Si el usuario no tiene permiso de acceso a la carpeta, se mostrará "Sin carpeta".

**Columna Enviado:** Información sobre la fecha y hora en que el documento fue enviado.

**Columna Concluido:** Información sobre la fecha y hora en que el proceso de firma del documento fue completado. Si aún no ha sido concluido, esta columna quedará en blanco.

**Columna Acciones:** En esta columna se muestran botones de acción sobre el documento. Estos botones se mostrarán de acuerdo con el perfil del usuario. Siempre se mostrará en este botón la acción prioritaria para ejecutar, según el perfil del usuario y el estado del documento.

**Barra de filtro:** Es posible localizar uno o más documentos utilizando los filtros disponibles para la búsqueda. La búsqueda puede realizarse por el nombre o correo electrónico del responsable del envío, por el nombre de uno de los signatarios, por el estado del documento (en la Caja de Entrada solo se mostrarán los documentos con estado "Concluido", "Esperando" y "En proceso"), por la carpeta donde está almacenado el documento o por la fecha de conclusión de las firmas.

<figure><img src="../.gitbook/assets/image (590).png" alt=""><figcaption></figcaption></figure>

***

## Acciones individuales - Caja de Entrada

<figure><img src="../.gitbook/assets/image (591).png" alt=""><figcaption></figcaption></figure>

#### **Firmar**

Disponible solo si el documento aún no ha sido firmado por el signatario y es su turno de firmar de acuerdo con el orden establecido por el remitente, si lo hay. Al hacer clic en este botón, el usuario es dirigido a la [<mark style="color:blue;">pantalla de firma del documento</mark>](../menu-superior/assinatura-de-documentos.md).

#### **Histórial**

&#x20;Aquí es posible visualizar el historial del proceso de firma y sus documentos. Seleccione el botón de eventos para ver detalladamente los datos. En esta pantalla también es posible descargar los archivos originales del proceso.

Con el botón de eventos ubicado a la derecha, se pueden observar los datos del proceso en la pantalla.

<figure><img src="../.gitbook/assets/image (592).png" alt=""><figcaption></figcaption></figure>

Con el botón de eventos ubicado a la izquierda, es posible visualizar los ID y Hash de los documentos, en el caso de un **proceso con más de un documento no agrupado.**

<figure><img src="../.gitbook/assets/image (593).png" alt=""><figcaption></figcaption></figure>

#### **Alterar** Carpeta

Esta opción solo se mostrará si el usuario tiene acceso a la cuenta en la que está almacenado el documento. Al hacer clic en esta opción, podrá cambiar la carpeta del directorio donde se almacena el documento.

<figure><img src="../.gitbook/assets/image (594).png" alt="" width="487"><figcaption></figcaption></figure>

#### **Alterar Proprietario**

Esta opción solo se mostrará si el usuario, además de ser signatario, también es el remitente del documento. Al hacer clic en esta opción, podrá cambiar el propietario del documento. Al ejecutar esta acción, no será posible realizar otras actividades de gestión del documento.

{% hint style="warning" %}
<mark style="color:orange;">**Solo pueden seleccionarse como nuevos propietarios a usuarios registrados en la misma cuenta que el responsable.**</mark>

<mark style="color:orange;">**El Administrador Global que no sea el remitente del documento podrá cambiar la propiedad de documentos completados que estén listados en la funcionalidad Directorios o cuando inactiva a un usuario que tiene documentos a su nombre.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (596).png" alt="" width="466"><figcaption></figcaption></figure>

#### Descargar Archivo

Cuando el proceso contiene un documento o es un compartimiento de solo un documento del proceso, **el sistema descarga** el documento del **proceso y el registro de firmas** en una carpeta .zip.

La carpeta zip se nombra con el nombre del proceso y el archivo de registro de firma se nombra como NombreDocumento\_Registro de firma.

<figure><img src="../.gitbook/assets/image (597).png" alt=""><figcaption></figcaption></figure>

Cuando el proceso **contiene más de un documento**, el sistema muestra un modal con los documentos del proceso para que el usuario seleccione cuáles documentos desea descargar. Si se trata de un compartimiento, solo se deben listar los documentos que han sido compartidos.

<figure><img src="../.gitbook/assets/image (598).png" alt=""><figcaption></figcaption></figure>

El Registro de Firmas muestra toda la información sobre las firmas electrónicas y digitales realizadas durante el proceso, como el nombre de los signatarios, la fecha y hora de la firma, la ubicación, la IP desde la que se realizó, los datos de los certificados digitales utilizados, entre otros.

<figure><img src="../.gitbook/assets/image (599).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (600).png" alt=""><figcaption></figcaption></figure>

#### **Cancelar**

&#x20;Esta opción solo se mostrará si el usuario, además de firmante, es también el remitente del documento. Al hacer clic en esta opción, el documento se cancela y el proceso de firmas se interrumpe. Esta opción no se mostrará si el estado del documento es “Concluido”.

#### **Compartir**

Esta opción permite que el usuario cree un enlace de acceso a uno o más documentos del proceso que podrá ser compartido con otras personas que no sean participantes del proceso de firma. Este enlace puede tener un plazo de validez determinado o indeterminado, y el usuario puede definir si desea permitir que las personas que accedan también visualicen los archivos adjuntos enviados por los signatarios.

Cuando el proceso contiene más de un documento no agrupado y no tiene compartimiento de documentos, el sistema abre un modal para que el usuario seleccione los documentos del proceso que desea compartir.

<figure><img src="../.gitbook/assets/image (601).png" alt=""><figcaption></figcaption></figure>

Cuando el proceso con más de un documento tiene compartimiento de documentos, el sistema abre un modal con los enlaces ya compartidos.

<figure><img src="../.gitbook/assets/image (602).png" alt=""><figcaption></figcaption></figure>

Al expandir las acciones del enlace de compartimiento, es posible **visualizar** nuevamente la pantalla de compartimiento o **excluir** el compartimiento realizado.

<figure><img src="../.gitbook/assets/image (603).png" alt=""><figcaption></figcaption></figure>

Al compartir los documentos del proceso, el usuario tiene la posibilidad de enviarlos por correo electrónico haciendo clic en el botón "Enviar Enlace por correo electrónico".

<figure><img src="../.gitbook/assets/image (604).png" alt=""><figcaption></figcaption></figure>

Agregue en el campo indicado todos los correos electrónicos que deben recibir la documentación compartida.

<figure><img src="../.gitbook/assets/image (605).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
<mark style="color:red;">Al compartir documentos de un proceso, es importante destacar que el destinatario del compartimiento solo podrá ver los documentos seleccionados para el compartimiento y no todos los documentos que componen el proceso de firma.</mark>
{% endhint %}

#### Visualización de documentos compartidos

Cuando se realiza el compartimiento de solo un documento de un proceso con más de un documento no agrupado, al abrir el documento, se presentará únicamente el documento compartido con el usuario.

Observe que en la lista solo se muestran los datos de los signatarios:

<figure><img src="../.gitbook/assets/image (606).png" alt=""><figcaption></figcaption></figure>

Cuando se realiza el compartimiento de más documentos del proceso, se presentan en la lista, además de los datos de los signatarios, los demás documentos del proceso:

<figure><img src="../.gitbook/assets/image (607).png" alt=""><figcaption></figcaption></figure>

#### **Alterar** Programación de Renovación

Esta opción solo se mostrará si el usuario, además de ser signatario, también es el remitente del documento. Se utiliza para cambiar o incluir un plazo de renovación del documento establecido anteriormente en el menú [<mark style="color:blue;">Nuevo Documento > Agregar Documentos</mark>](../menu-superior/novo-documento.md#a.-adicionar-documentos).

<figure><img src="../.gitbook/assets/image (608).png" alt="" width="443"><figcaption></figcaption></figure>

#### **R**echazar Firma

Disponible solo si el documento aún no ha sido firmado por el signatario y es su turno de firmar de acuerdo con el orden establecido por el remitente, si lo hay. Se utiliza cuando, por algún motivo, el signatario no desea firmar el documento. En este caso, debe ingresar una justificación para la negativa y hacer clic en "Rechazar Firma".

<figure><img src="../.gitbook/assets/image (609).png" alt="" width="516"><figcaption></figcaption></figure>

#### **Reenviar**

Esta opción solo se mostrará si el usuario, además de ser signatario, también es el remitente del documento y si el documento está vencido, es decir, el plazo de firma terminó antes de que todos los signatarios hayan firmado. Al hacer clic en este botón, se mostrarán las informaciones de orden de envío para los destinatarios, el correo electrónico o teléfono al que se envió el documento, el código de seguridad para acceder al documento (si lo hay) y el ícono "Editar", que permite la edición de la información del destinatario.

<figure><img src="../.gitbook/assets/image (610).png" alt=""><figcaption></figcaption></figure>

#### **R**enombrar

Esta opción solo se mostrará si el usuario, además de ser signatario, también es el remitente del documento.

Cuando el proceso contiene solo un documento, el sistema permite cambiar el nombre del proceso:

<figure><img src="../.gitbook/assets/image (611).png" alt="" width="563"><figcaption></figcaption></figure>

Cuando el proceso contiene más de un documento, el sistema permite cambiar el nombre del proceso y el nombre de los documentos del proceso.

<figure><img src="../.gitbook/assets/image (612).png" alt="" width="476"><figcaption></figcaption></figure>

El campo “**Renombrar documentos del proceso**” se muestra solo si el usuario que ha iniciado sesión es el remitente del proceso y el proceso contiene más de un documento/archivo.

Por defecto, este campo se muestra desmarcado y al marcarlo, el sistema lista todos los documentos del proceso habilitados para edición.

El usuario tiene la posibilidad de mover los documentos, cambiando su orden. Al mover los documentos, el sistema actualiza la numeración frente a cada documento.

**Excluir:** Se utiliza para eliminar el archivo, que irá a la caja de [<mark style="color:blue;">Eliminados</mark>](excluidos.md).

<figure><img src="../.gitbook/assets/image (613).png" alt=""><figcaption></figcaption></figure>

***

## Acciones en lote - Caja de Entrada

Es posible seleccionar más de un documento marcando las casillas junto al nombre del archivo y ejecutar acciones en lote. Las acciones en lote solo podrán ser ejecutadas en documentos en los que el usuario, además de ser signatario, sea el remitente del documento.

<figure><img src="../.gitbook/assets/image (614).png" alt=""><figcaption></figcaption></figure>

#### **Mover  Proceso (s)**

Al hacer clic en este ícono, será posible cambiar la carpeta donde están almacenados los documentos seleccionados. Esta acción solo se podrá ejecutar en documentos en los que el usuario, además de ser signatario, sea el remitente del documento.

<figure><img src="../.gitbook/assets/image (615).png" alt="" width="470"><figcaption></figcaption></figure>

#### **Reenviar**

Al hacer clic en este ícono, será posible reenviar los documentos seleccionados a los destinatarios que aún no han firmado. Esta acción solo se podrá ejecutar en documentos en los que el usuario, además de ser signatario, sea el remitente del documento y que no tengan el estado “Concluido”.

<figure><img src="../.gitbook/assets/image (616).png" alt=""><figcaption></figcaption></figure>

#### **Cancelar Envío**

Al hacer clic en este ícono, será posible cancelar el envío de los documentos seleccionados, interrumpiendo los procesos de firma. Esta acción solo se podrá ejecutar en documentos en los que el usuario, además de ser signatario, sea el remitente del documento y que no tengan el estado “Concluido”.

<figure><img src="../.gitbook/assets/image (617).png" alt=""><figcaption></figcaption></figure>

#### **Excluir**

Al hacer clic en este ícono, será posible eliminar los documentos seleccionados. Esta acción solo se podrá ejecutar en documentos en los que el usuario, además de ser signatario, sea el remitente del documento y que tengan el estado “Concluido”.

<figure><img src="../.gitbook/assets/image (618).png" alt=""><figcaption></figcaption></figure>
