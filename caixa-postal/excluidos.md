# 🗑️ Excluídos

En el menú Eliminados se muestran todos los documentos eliminados por el usuario. Pueden ser documentos ya concluidos, cancelados o solo creados.

{% hint style="warning" %}
<mark style="color:orange;">**No es posible visualizar el documento en la pantalla Eliminados. Para ver el archivo, es necesario restaurar el documento y acceder a él en su buzón de origen, que puede ser la**</mark> [<mark style="color:blue;">**Caja de Entrada**</mark>](https://app.gitbook.com/o/Ai1YjbPQxIuvTaVzoZ4H/s/zDlPVk00J5AKVvFiB3dg/) <mark style="color:orange;">**o la**</mark> [<mark style="color:blue;">**caja Enviados**</mark>](enviados.md)<mark style="color:orange;">**.**</mark>
{% endhint %}

***

<figure><img src="../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

## Columnas de la pantalla principal - Excluídos

<figure><img src="../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

**Columna Nombre del Documento**: Muestra el nombre del documento y el nombre del firmante. Si hay más de un firmante, se muestra el nombre del primero y la cantidad de otras personas que deben firmar.

**Columna Responsable**: Presenta el nombre y el correo electrónico de quien envió el documento (remitente).

**Columna Estado**: Los estados posibles para un documento son: “Concluido” (todos los participantes firmaron el documento), “Cancelado” (el envío fue cancelado y el proceso de firma interrumpido) y “Creado” (el documento fue creado en la plataforma, pero su configuración y envío a los destinatarios aún no fueron completados). Al pasar el cursor sobre el estado, se muestra información sobre los firmantes que aún tienen firmas pendientes y los que ya firmaron, además de los datos de estos firmantes. También se muestra el código de seguridad enviado a los destinatarios (si existe).

<figure><img src="../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

**Columna Tamaño**: Muestra el tamaño del archivo del documento.&#x20;

**Columna Carpeta**: Muestra la carpeta del directorio donde se almacena el documento. Si el usuario no tiene permiso de acceso a la carpeta, se mostrará "Sin carpeta".

**Columna Concluido**: Proporciona información sobre la fecha y hora en que se completó el proceso de firma del documento. Si aún no se ha completado, esta columna permanecerá en blanco.&#x20;

**Columna Excluido**: Muestra la fecha y hora en que el documento fue eliminado.&#x20;

**Columna Acciones**: Esta columna muestra botones de acción sobre el documento. Siempre se mostrará en este botón la acción prioritaria de ejecución, según el perfil del usuario y el estado del documento.

**Barra de filtro**: Permite localizar uno o más documentos utilizando los filtros disponibles para búsqueda. En la pantalla Excluidos, la búsqueda se puede realizar por el nombre del documento, el nombre del responsable, los nombres de los firmantes, el estado del documento, la carpeta donde está almacenado el documento o la fecha de eliminación del documento.

<figure><img src="../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

## Acciones individuales - Excluídos

<figure><img src="../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

#### **Restaurar**

Al hacer clic en esta opción, el documento regresa a la bandeja de entrada donde estaba antes de la eliminación. Solo se pueden restaurar documentos eliminados hace menos de un año.

{% hint style="info" %}
<mark style="color:blue;">**Los documentos con el estado “Concluido” regresarán a la Bandeja de Entrada si el usuario es solo participante del proceso de firma o a la caja Enviados si es propietario del documento.**</mark>

<mark style="color:blue;">**Los documentos con el estado “Cancelado” siempre regresarán a la caja Enviados, ya que son propiedad del usuario.**</mark>
{% endhint %}

{% hint style="danger" %}
<mark style="color:red;">**Los documentos con el estado “Creado” no pueden ser restaurados.**</mark>
{% endhint %}

#### Descargar Archivo

Cuando el proceso tiene un documento o es un intercambio de solo un documento del proceso, **el sistema descarga** el documento del **proceso y el registro de firmas** en una carpeta .zip.

La carpeta zip se nombra con el nombre del proceso y el archivo de registro de firma se nombra como **NombreDocumento\_Registro** de firma.

<figure><img src="../.gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

Cuando el proceso **tiene más de un documento**, el sistema muestra un modal con los documentos del proceso para que el usuario seleccione cuáles documentos desea descargar. Si se trata de un intercambio, solo se deben listar los documentos que han sido compartidos.

<figure><img src="../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

El Registro de Firmas muestra toda la información sobre las firmas electrónicas y digitales realizadas durante el proceso, como el nombre de los firmantes, la fecha y hora de la firma, la ubicación, la dirección IP desde donde se realizó, los datos de los certificados digitales utilizados, etc.

<figure><img src="../.gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (48).png" alt=""><figcaption></figcaption></figure>

#### **Histórico**

Aquí es posible visualizar el historial del proceso de firma y sus documentos. Seleccione el botón de eventos para ver los datos en detalle. En esta pantalla también es posible descargar los archivos originales del proceso.&#x20;

Con el botón de eventos posicionado a la derecha, observamos los datos del proceso en la pantalla.

Com o botão de eventos posicionado para a esquerda, é possível visualizar os Id's e Hash's dos documentos, no caso de um **processo com mais de um documento não agrupados**.

<figure><img src="../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>

***

## Acciones en lote - Excluídos

Es posible seleccionar más de un documento marcando las casillas al lado del nombre del archivo y ejecutar acciones en lote.

**Restaurar:** En la pantalla de Eliminados, la única acción en lote posible es restaurar documentos, devolviéndolos a la bandeja de entrada en la que estaban antes de la eliminación. Solo se pueden restaurar documentos eliminados hace menos de un año.

{% hint style="info" %}
<mark style="color:blue;">**Los documentos con el estado "Concluido" volverán a la Bandeja de Entrada si el usuario es solo participante del proceso de firma o a la bandeja Enviados si es el propietario del documento.**</mark>

<mark style="color:blue;">**Los documentos con el estado "Cancelado" siempre regresarán a la bandeja Enviados, ya que son propiedad del usuario.**</mark>
{% endhint %}

{% hint style="danger" %}
<mark style="color:red;">**Los documentos con el estado "Creado" no pueden ser restaurados.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (52).png" alt=""><figcaption><p>Haz clic en la imagen para ampliar.</p></figcaption></figure>
