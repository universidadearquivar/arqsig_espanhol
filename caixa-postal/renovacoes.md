# 🗓️ Renovaciones

{% embed url="https://app.supademo.com/demo/cmcyvechx1rhxc4kjksctqn54" %}

En el menú Renovaciones se presentan todos los documentos que fueron registrados y enviados para firma con la opción "Programar renovación \_\_\_ meses después de la conclusión de las firmas" marcada, en la pantalla [<mark style="color:blue;">Nuevo Documento > Agregar Documentos y Destinatarios > Agregar Documentos.</mark>](https://app.gitbook.com/o/Ai1YjbPQxIuvTaVzoZ4H/s/zDlPVk00J5AKVvFiB3dg/) Solo se pueden mostrar en esta pantalla documentos con el estado "Concluido".

<figure><img src="../.gitbook/assets/image (659).png" alt=""><figcaption><p>Haz clic en la imagen para ampliar.</p></figcaption></figure>

***

## Columnas de la pantalla principal - Renovaciones

<figure><img src="../.gitbook/assets/image (660).png" alt=""><figcaption><p>Haz clic en la imagen para ampliar.</p></figcaption></figure>

**Columna Nombre del Documento:** En esta columna se muestran el nombre del documento y el nombre del firmante. Si hay más de un firmante, se mostrará el nombre del primero y la cantidad de otras personas que deben firmar.

**Columna Responsable:** En esta columna se presentan el nombre y el correo electrónico de quien envió el documento (remitente). En la pantalla Renovaciones, el único nombre y correo electrónico presentados serán los del propio usuario.

**Columna Estado:** En la pantalla Renovaciones, el único estado posible para un documento es "Concluido" (todos los participantes ya han firmado el documento). Al pasar el mouse sobre el estado, se muestran información sobre los firmantes. También se muestra el código de seguridad enviado a los destinatarios (si lo hay).

<figure><img src="../.gitbook/assets/image (661).png" alt=""><figcaption></figcaption></figure>

**Columna Tamaño:** En esta columna se muestra el tamaño del archivo del documento.

**Columna Carpeta:** En esta columna se muestra la carpeta del directorio donde está almacenado el documento.

**Columna Concluido:** Información sobre la fecha y hora en que se completó el proceso de firma del documento.

Columna Renovación: Esta columna muestra la fecha y hora en que el documento debe renovarse, de acuerdo con la información ingresada en el campo "Programar renovación \_\_\_ meses después de la conclusión de las firmas", marcado en la pantalla [<mark style="color:blue;">Nuevo Documento > Agregar Documentos y Destinatarios > Agregar Documentos</mark>](../menu-superior/novo-documento.md#a.-adicionar-documentos). Se muestran tanto documentos que tienen fecha futura de renovación como aquellos que ya han pasado el plazo, pero que aún no han sido renovados.

**Columna Acciones:** Esta columna muestra botones de acción sobre el documento. Siempre se mostrará en este botón la acción prioritaria de ejecución, de acuerdo con el perfil del usuario y el estado del documento.

**Barra de filtro:** Es posible localizar uno o más documentos utilizando los filtros disponibles para la búsqueda. En la pantalla Renovaciones, la búsqueda se puede hacer por el nombre del documento, el nombre del responsable, los nombres de los firmantes, el estado del documento, la carpeta donde está hospedado el documento o la fecha de exclusión del documento.

<figure><img src="../.gitbook/assets/image (662).png" alt=""><figcaption></figcaption></figure>

***

## Acciones individuales - Renovaciones

<figure><img src="../.gitbook/assets/image (663).png" alt=""><figcaption></figcaption></figure>

#### **Renovar**

Esta acción estará disponible si el documento ha alcanzado la fecha y hora programadas para su renovación en el campo “Agendar renovación \_\_\_ meses después de la conclusión de las firmas” marcado en la pantalla [<mark style="color:blue;">Nuevo Documento > Agregar Documentos y Destinatarios > Agregar Documentos</mark>](../menu-superior/novo-documento.md#a.-adicionar-documentos). Al hacer clic en este botón, el usuario será dirigido a la pantalla “Agregar documentos y destinatarios” con la información de los destinatarios completada con la misma información del flujo anterior, para que realice nuevamente la configuración y el envío del nuevo documento a los destinatarios.

{% hint style="warning" %}
<mark style="color:orange;">**Incluso después de renovar el documento y enviarlo a los destinatarios, el documento será listado en la pantalla de Renovaciones hasta que todos los firmantes completen la firma.**</mark>&#x20;
{% endhint %}

#### **Alterar Carpeta**

Al hacer clic en esta opción, podrá cambiar la carpeta del directorio donde está almacenado el documento.

<figure><img src="../.gitbook/assets/image (664).png" alt="" width="440"><figcaption></figcaption></figure>

#### **Alterar** Renovación

Esta opción solo estará disponible si el documento aún no ha sido renovado. Al hacer clic en esta opción, será posible cambiar la fecha de renovación ingresando la cantidad de meses que debe tener el intervalo de renovación del documento. También es posible eliminar la renovación haciendo clic en "Eliminar Programación".

<figure><img src="../.gitbook/assets/image (665).png" alt=""><figcaption></figcaption></figure>

#### **Histórico**

Aquí es posible visualizar el historial del proceso de firma y sus documentos. Seleccione el botón de eventos para ver detalladamente los datos. En esta pantalla también es posible descargar los archivos originales del proceso.&#x20;

Con el botón de eventos posicionado a la derecha, observamos los datos del proceso en la pantalla.

<figure><img src="../.gitbook/assets/image (666).png" alt=""><figcaption></figcaption></figure>

Con el botón de eventos posicionado a la izquierda, es posible visualizar los ID y Hash de los documentos, en el caso de un **proceso con más de un documento no agrupados.**

<figure><img src="../.gitbook/assets/image (667).png" alt=""><figcaption></figcaption></figure>

#### **Alterar Proprietario**

Al hacer clic en esta opción, podrá cambiar el propietario del documento. Al ejecutar esta acción, no será posible realizar otras actividades de gestión del documento.

{% hint style="warning" %}
<mark style="color:orange;">**Solo pueden ser seleccionados como nuevos propietarios los usuarios registrados en la misma cuenta que el responsable.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (668).png" alt=""><figcaption></figcaption></figure>

#### Descargar Archivo

Cuando el proceso tiene un documento o es un compartimiento de solo un documento del proceso, **el sistema descarga** el documento del **proceso y el registro de firmas** en una carpeta .zip.

La carpeta zip se nombra con el nombre del proceso y el archivo de registro de firmas se nombra como **NombreDocumento\_Registro** de firma.

<figure><img src="../.gitbook/assets/image (669).png" alt=""><figcaption></figcaption></figure>

Cuando el proceso **tiene más de un documento**, el sistema muestra un modal con los documentos del proceso para que el usuario seleccione cuáles documentos desea descargar. En caso de ser un compartimiento, solo se deben listar los documentos que han sido compartidos.

<figure><img src="../.gitbook/assets/image (670).png" alt="" width="455"><figcaption></figcaption></figure>

El Registro de Firmas muestra toda la información sobre las firmas electrónicas y digitales realizadas durante el proceso, como el nombre de los firmantes, la fecha y hora de la firma, la ubicación, la IP desde donde se realizó, los datos de los certificados digitales utilizados, etc.

<figure><img src="../.gitbook/assets/image (672).png" alt="" width="478"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (673).png" alt="" width="479"><figcaption></figcaption></figure>

#### **Compartir**

Esta opción permite que el usuario cree un enlace de acceso a uno o más documentos del proceso que se podrá compartir con otras personas que no sean participantes del proceso de firma. Este enlace puede tener un plazo de validez determinado o indeterminado, y el usuario puede definir si desea permitir que las personas que accedan también visualicen los archivos adjuntos enviados por los firmantes.

Cuando el proceso tiene más de un documento no agrupado y no hay un compartimiento de documentos, el sistema abre una ventana modal para que el usuario seleccione los documentos del proceso que desea compartir.

<figure><img src="../.gitbook/assets/image (674).png" alt="" width="563"><figcaption></figcaption></figure>

Cuando el proceso con más de un documento tiene compartimiento de documentos, el sistema abre una ventana modal con los enlaces ya compartidos.

<figure><img src="../.gitbook/assets/image (675).png" alt=""><figcaption></figcaption></figure>

Al expandir las acciones del enlace de compartición, es posible visualizar nuevamente la pantalla de compartición o eliminar la compartición realizada.

<figure><img src="../.gitbook/assets/image (677).png" alt=""><figcaption></figcaption></figure>

Al compartir los documentos del proceso, el usuario tiene la posibilidad de enviarlos por correo electrónico haciendo clic en el botón "Enviar enlace por correo electrónico".

<figure><img src="../.gitbook/assets/image (678).png" alt=""><figcaption></figcaption></figure>

Agregue en el campo indicado todos los correos electrónicos que deben recibir la documentación compartida.

<figure><img src="../.gitbook/assets/image (679).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
<mark style="color:red;">**Al compartir documentos de un proceso, es importante resaltar que el destinatario del compartimiento podrá visualizar únicamente los documentos seleccionados para compartir y no todos los documentos que componen el proceso de firma.**</mark>
{% endhint %}

#### Visualización de documentos compartidos

Cuando se comparte solo un documento de un proceso con más de un documento no agrupado, al abrir el documento, se mostrará únicamente el documento compartido con el usuario.

Observe que en la lista solo se presentan los datos de los firmantes:

<figure><img src="../.gitbook/assets/image (648).png" alt=""><figcaption></figcaption></figure>

Cuando se realiza el compartimiento de más documentos del proceso, se presenta en la lista, además de los datos de los firmantes, los demás documentos del proceso:

<figure><img src="../.gitbook/assets/image (649).png" alt=""><figcaption></figcaption></figure>

**Excluir:** Utilizado para excluir el archivo, que irá a la [<mark style="color:blue;">caja de Eliminados</mark>](https://app.gitbook.com/o/Ai1YjbPQxIuvTaVzoZ4H/s/zDlPVk00J5AKVvFiB3dg/).&#x20;

<figure><img src="../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

**Renombrar:** Esta opción solo se mostrará si el usuario, además de firmante, también es el remitente del documento.&#x20;

Cuando el proceso tiene solo un documento, el sistema permite cambiar el nombre del proceso:

<figure><img src="../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

Quando processo possui mais de um documento, o sistema permite alterar o nome do processo e o nome dos documentos do processo.

<figure><img src="../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

El campo “**Renombrar documentos del proceso**” se muestra solo si el usuario que ha iniciado sesión es el remitente del proceso y el proceso contiene más de un documento/archivo.

Por defecto, este campo aparece desmarcado y, al marcarlo, el sistema lista todos los documentos del proceso habilitados para edición.

El usuario tiene la posibilidad de mover los documentos, alterando su orden. Al mover los documentos, el sistema actualiza la numeración delante de cada documento.

#### **Versionado**

Esta opción permite al usuario visualizar todas las versiones del documento que ya han sido enviadas. Al renovar un documento y concluirlo, deja de mostrarse en la pantalla de Renovaciones, pero la información sobre su envío puede ser vista en la pantalla de Versionado del Documento.

<figure><img src="../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

***

## Acciones en lote - Renovaciones

Es posible seleccionar más de un documento marcando las casillas de verificación al lado del nombre del archivo y ejecutar acciones en lote.

<figure><img src="../.gitbook/assets/renovacoes05.png" alt=""><figcaption></figcaption></figure>

#### **Mover Proceso (s)**

Al hacer clic en este ícono, será posible cambiar la carpeta donde están almacenados los documentos seleccionados.

<figure><img src="../.gitbook/assets/image (34).png" alt="" width="438"><figcaption></figcaption></figure>

#### **Alterar Proprietario**

Al hacer clic en este ícono, será posible cambiar la propiedad de los documentos seleccionados, es decir, las funciones de administración del documento serán de otro usuario. Esta acción solo podrá ser deshecha si el usuario que se define como nuevo propietario devuelve la propiedad del documento al propietario original. El cambio de propietario de un documento en lote tiene un plazo de 24 horas para ser realizado y para seguir el progreso, el usuario debe acceder al menú Mi Perfil > Pestaña Solicitudes.

{% hint style="warning" %}
<mark style="color:orange;">**Solo pueden ser seleccionados como nuevos propietarios los usuarios registrados en la misma cuenta que el responsable.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (35).png" alt="" width="380"><figcaption></figcaption></figure>

#### **Excluir**

Al hacer clic en este ícono, será posible eliminar los documentos seleccionados. Solo se podrá ejecutar esta acción en documentos con el estado "Concluido" o "Cancelado".

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

## 🗪 Preguntas y Respuestas Frecuentes

<details>

<summary>¿Cómo activar el flujo de renovación automática de Procesos?</summary>

Si ha programado la renovación de un Proceso, al cumplirse el plazo para la renovación, puede activar la renovación automática para que se cree un nuevo Proceso con las mismas configuraciones de firmantes que el original.

1. Haga clic en Renovaciones;
2. Seleccione Proceso concluido;
3. Haga clic en Renovar - La Plataforma genera automáticamente un nuevo Proceso con todos los firmantes del Proceso original;
4. Suba el archivo para la renovación. El nuevo archivo queda vinculado al(los) archivo(s) anterior(es), creando un versionado de Procesos.
5. Revise los firmantes.
6. Configure las representaciones visuales;
7. Envíe ¡y listo!

</details>

<details>

<summary>¿Cómo modificar la renovación, vencimiento de Procesos o control de reajuste?</summary>

Después de la finalización de un Proceso:

1. Haga clic en Enviados;
2. Seleccione Proceso concluido;
3. Haga clic en Historial;
4. Haga clic en Cambiar Renovación;
5. Defina el nuevo plazo en meses después de la finalización de las firmas;
6. Haga clic en Cambiar.

Cuando llegue la fecha definida para el vencimiento del Proceso, renovación o reajuste, la plataforma ArqSign enviará un correo electrónico al propietario del Proceso informando que está listo para renovación, reajuste, etc.

</details>
