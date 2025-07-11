# 📩 Expedidos

## Visualizar Proceso

En la caja Enviados se presentan todos los documentos enviados por el usuario a los firmantes, incluidos aquellos en los que él mismo es firmante.

<figure><img src="../.gitbook/assets/image (619).png" alt=""><figcaption></figcaption></figure>

{% embed url="https://app.supademo.com/demo/cmcyraln11nj7c4kjet0nzlu1" %}

Al hacer clic en un documento, se abrirá la pantalla de visualización del documento, que muestra el documento enviado, su estado y fecha de vencimiento. En la esquina derecha de la pantalla se presentan las informaciones de los firmantes, como datos personales, rol de firmante y estado de la firma.

<figure><img src="../.gitbook/assets/image (620).png" alt=""><figcaption></figcaption></figure>

Cuando el proceso tiene más de un documento no agrupado, el sistema lista los documentos en el orden definido para los documentos del proceso, permitiendo la navegación entre ellos y mostrando en la pantalla el documento seleccionado por el usuario.

#### Vista del usuario conectado

<figure><img src="../.gitbook/assets/image (621).png" alt=""><figcaption></figcaption></figure>

#### Vista del usuario no conectado

<figure><img src="../.gitbook/assets/image (622).png" alt=""><figcaption></figcaption></figure>

Por padrão, os dados do signatário são apresentados abertos na tela, basta fechar a lista e continuar com a navegação no documento.

## Columnas de la pantalla principal - Enviados

<figure><img src="../.gitbook/assets/image (623).png" alt=""><figcaption></figcaption></figure>

**Columna Nombre del Documento**: En esta columna se muestran el nombre del documento y el nombre del firmante. Si hay más de un firmante, se mostrará el nombre del primero y la cantidad de otras personas que deben firmar.

**Columna Responsable**: En esta columna se presentan el nombre y correo electrónico de quien envió el documento (remitente). En la pantalla Enviados, el único nombre y correo electrónico que se mostrarán serán los del propio usuario.

**Columna Estado**: Los posibles estados para un documento son: "Esperando" (ningún participante ha firmado el documento hasta el momento), "En proceso" (uno o más participantes ya han firmado el documento, pero aún faltan firmas), "Completado" (todos los participantes ya han firmado el documento) y "Cancelado" (el envío del documento fue cancelado y el proceso de firma fue interrumpido). Al pasar el mouse sobre el estado, se muestra información sobre cuáles firmantes aún tienen la firma pendiente y cuáles ya han concluido, además de los datos de estos firmantes. También se muestra el código de seguridad enviado a los destinatarios (si lo hay).

<figure><img src="../.gitbook/assets/image (624).png" alt=""><figcaption></figcaption></figure>

**Columna Tamaño**: En esta columna se muestra el tamaño del archivo del documento.

**Columna Carpeta**: En esta columna se muestra la carpeta del directorio donde está almacenado el documento. Si el usuario no tiene permiso de acceso a la carpeta, se mostrará "Sin carpeta".

**Columna Enviado**: Información sobre la fecha y hora en que se envió el documento.

**Columna Completado**: Información sobre la fecha y hora en que se completó el proceso de firma del documento. Si aún no se ha completado, esta columna permanecerá en blanco.

**Columna Acciones**: Esta columna muestra los botones de acción sobre el documento. Estos botones se mostrarán según el perfil del usuario. Siempre se mostrará en este botón la acción prioritaria a ejecutar, de acuerdo con el perfil del usuario y el estado del documento.

**Barra de filtro**: Es posible localizar uno o más documentos utilizando los filtros de búsqueda disponibles. La búsqueda se puede realizar por el nombre o correo electrónico del responsable del envío, por el nombre de uno de los firmantes, por el estado del documento (en la caja Enviados se mostrarán los documentos con estado "Completado", "Esperando", "En proceso" y "Cancelado"), por la carpeta donde está almacenado el documento o por la fecha de finalización de las firmas.

<figure><img src="../.gitbook/assets/image (625).png" alt=""><figcaption></figcaption></figure>

***

## A**cciones individuales - Enviados**

<figure><img src="../.gitbook/assets/image (626).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">Es importante resaltar que las "Acciones" mostradas en la pantalla dependen del "Estado" del proceso de firma.</mark>
{% endhint %}

#### **Reenviar**

Es posible reenviar documentos que aún no han sido firmados por todos los firmantes. En los casos de documentos cuyo plazo de firma ha expirado y que no han sido firmados por todos los firmantes, se muestra el mensaje "Vencido antes de la conclusión de las firmas".&#x20;

En este caso, es posible reenviar el documento solo a aquellos firmantes que aún no han firmado. Al hacer clic en "reenviar" se mostrarán las informaciones sobre el orden de envío para los destinatarios, correo electrónico o teléfono al cual se envió el documento, y el código de seguridad para acceder al documento (si aplica).

<figure><img src="../.gitbook/assets/image (627).png" alt=""><figcaption></figcaption></figure>



En el ícono "Editar", es posible realizar la edición de la información del destinatario, así como la información definida para la validación del documento en las [<mark style="color:blue;">**configuraciones del destinatario**</mark>](https://app.gitbook.com/o/Ai1YjbPQxIuvTaVzoZ4H/s/zDlPVk00J5AKVvFiB3dg/).

<figure><img src="../.gitbook/assets/image (628).png" alt="" width="545"><figcaption></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">Los datos de validación del documento solo podrán ser editados en esta pantalla si fueron configurados previamente. La "Edición" no permite la inclusión de datos para validación.</mark>
{% endhint %}

{% hint style="warning" %}
<mark style="color:orange;">**Los procesos de firma enviados a través de ArqGED-ArqFlow solo podrán ser reenviados mediante una nueva acción en ArqGED-ArqFlow.**</mark>

<mark style="color:orange;">**De esta manera, en la columna Acciones, no habrá la opción "Reenviar".**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (806).png" alt=""><figcaption></figcaption></figure>

Tampoco habrá la opción "Reenviar" al abrir el proceso en la plataforma ArqSign.

<figure><img src="../.gitbook/assets/Screenshot_7 (1).jpg" alt=""><figcaption></figcaption></figure>

#### **Alterar** Carpeta

Esta opción solo se mostrará si el usuario tiene acceso a la carpeta en la que está almacenado el documento. Al hacer clic en esta opción, podrá cambiar la carpeta del directorio donde se almacena el documento.

<figure><img src="../.gitbook/assets/image (629).png" alt="" width="439"><figcaption></figcaption></figure>

#### **Alterar Proprietario**

Al hacer clic en esta opción, el usuario podrá cambiar el propietario del documento. Al ejecutar esta acción, no será posible realizar otras actividades de gestión del documento.

{% hint style="warning" %}
<mark style="color:orange;">**Solo se pueden seleccionar como nuevo propietario a los usuarios registrados en la misma cuenta que el responsable.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (630).png" alt=""><figcaption></figcaption></figure>

#### Descargar Archivo

Cuando el proceso tiene un documento o es un compartido de solo un documento del proceso, **el sistema descarga** el documento del **proceso y el registro de firmas** en una carpeta .zip.

La carpeta zip se nombra con el nombre del proceso y el archivo de registro de firma se nombra como **NombreDocumento\_Registro** de firma.

<figure><img src="../.gitbook/assets/image (655).png" alt=""><figcaption></figcaption></figure>

Cuando el proceso **tenga más de un documento**, el sistema mostrará un modal con los documentos del proceso para que el usuario seleccione cuáles desea descargar. En caso de ser un intercambio, solo se deben listar los documentos que han sido compartidos.

<figure><img src="../.gitbook/assets/image (632).png" alt=""><figcaption></figcaption></figure>

El Registro de Firmas muestra toda la información sobre las firmas electrónicas y digitales realizadas durante el proceso, como el nombre de los signatarios, la fecha y hora de la firma, la ubicación, la IP desde la que se realizó, los datos de los certificados digitales utilizados, entre otros.

<figure><img src="../.gitbook/assets/image (633).png" alt="" width="449"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (634).png" alt="" width="447"><figcaption></figcaption></figure>

#### **Cancelar**

Al hacer clic en esta opción, el documento se cancela y el proceso de firmas se interrumpe.

<figure><img src="../.gitbook/assets/image (635).png" alt=""><figcaption></figcaption></figure>

#### **Histórico**

Se utiliza para visualizar información sobre el documento y el historial de los eventos relacionados con él. También es posible descargar los archivos originales del proceso, antes de que se hayan completado las firmas. Esta opción solo estará disponible para documentos con el estado "Concluido".

&#x20;Con el botón de **eventos posicionado a la derecha**, se observan los datos del proceso en la pantalla.

<figure><img src="../.gitbook/assets/image (636).png" alt=""><figcaption></figcaption></figure>

Con el botón de **eventos posicionado a la izquierda**, es posible visualizar los ID y Hash de los documentos, en el caso de un **proceso con más de un documento no agrupados**.

<figure><img src="../.gitbook/assets/image (637).png" alt=""><figcaption></figcaption></figure>

#### **Alterar** Renovación

Esta opción solo estará disponible si el documento tiene el estado “Concluido”. Al hacer clic en esta opción, es posible incluir o modificar la fecha de renovación del documento, determinada anteriormente en el campo “Programar renovación \_\_\_ meses después de la conclusión de las firmas”, marcado en la pantalla Nuevo Documento > Agregar Documentos y Destinatarios > Agregar Documentos. Para incluir o modificar la cantidad de meses de intervalo entre las renovaciones, edite el campo “Cantidad Meses Renovación”.

<figure><img src="../.gitbook/assets/image (638).png" alt=""><figcaption></figcaption></figure>

#### **C**orregir

Se mostrará este botón cuando la información de contacto (correo electrónico o teléfono) para el envío del documento de uno o más firmantes esté incorrecta. En este caso, será necesario corregir la información incorrecta para que el sistema reenvíe el documento.

#### Eliminar

Utilizado para eliminar el flujo. Los flujos eliminados irán a la caja de [<mark style="color:blue;">Eliminados</mark>](https://app.gitbook.com/o/Ai1YjbPQxIuvTaVzoZ4H/s/zDlPVk00J5AKVvFiB3dg/).

<figure><img src="../.gitbook/assets/image (639).png" alt="" width="264"><figcaption></figcaption></figure>

#### **R**enombrar

Esta opción solo se mostrará si el usuario, además de firmante, también es el remitente del documento.&#x20;

Cuando el proceso tiene solo un documento, el sistema permite cambiar el nombre del proceso:

<figure><img src="../.gitbook/assets/image (808).png" alt="" width="375"><figcaption></figcaption></figure>

Cuando el proceso tiene más de un documento, el sistema permite cambiar el nombre del proceso y el nombre de los documentos del proceso.

<figure><img src="../.gitbook/assets/image (809).png" alt="" width="374"><figcaption></figcaption></figure>

El campo "**Renombrar documentos del proceso**" se muestra solo si el usuario conectado es el remitente del proceso y el proceso tiene más de un documento/archivo.

Por defecto, este campo se muestra desmarcado y al marcarlo, el sistema lista todos los documentos del proceso habilitados para edición.

El usuario tiene la posibilidad de mover los documentos, cambiando su orden. Al mover los documentos, el sistema actualiza la numeración al frente de cada documento.

#### **Compartir**

Esta opción permite que el usuario cree un enlace de acceso a uno o más documentos del proceso que podrá ser compartido con otras personas que no sean participantes del proceso de firma. Este enlace puede tener un plazo de validez determinado o indefinido y el usuario puede definir si desea permitir que las personas que accedan también visualicen los anexos enviados por los signatarios.

Cuando el proceso con más de un documento no agrupado no tiene compartición de documentos, el sistema abre el modal para que el usuario seleccione los documentos del proceso que desea compartir.

<figure><img src="../.gitbook/assets/image (642).png" alt="" width="563"><figcaption></figcaption></figure>

Cuando el proceso con más de un documento tiene compartición de documentos, el sistema abre el modal con los enlaces ya compartidos.

<figure><img src="../.gitbook/assets/image (643).png" alt="" width="563"><figcaption></figcaption></figure>

Al expandir las acciones del enlace de compartición, es posible **visualizar** nuevamente la pantalla de compartición o **eliminar** la compartición realizada.

<figure><img src="../.gitbook/assets/image (644).png" alt=""><figcaption></figcaption></figure>

Al compartir los documentos del proceso, el usuario tiene la posibilidad de enviarlos por correo electrónico haciendo clic en el botón "Enviar enlace por correo electrónico".

<figure><img src="../.gitbook/assets/image (645).png" alt=""><figcaption></figcaption></figure>

Agregue en el campo indicado todos los correos electrónicos que deben recibir la documentación compartida.

<figure><img src="../.gitbook/assets/image (646).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
<mark style="color:red;">Al compartir documentos de un proceso, es importante resaltar que el destinatario del compartido podrá visualizar únicamente los documentos seleccionados para el intercambio y no todos los documentos que componen el proceso de firma.</mark>
{% endhint %}

#### Visualización de documentos compartidos

Cuando se realiza el intercambio de un solo documento de un proceso con más de un documento no agrupado, al abrir el documento, se presentará únicamente el documento compartido con el usuario.

Observe que en la lista solo se presentan los datos de los firmantes:

<figure><img src="../.gitbook/assets/image (648).png" alt=""><figcaption></figcaption></figure>

Quando realizado o compartilhamento de mais documentos do processo, é apresentado na lista, além dos dados dos signatários, os demais documentos do processo:

<figure><img src="../.gitbook/assets/image (649).png" alt=""><figcaption></figcaption></figure>

***

## Acciones en lote - Enviados

É possível selecionar mais de um documento marcando o _checkbox_ ao lado do nome do arquivo e selecionando um dos ícones de execução de ações em lote.

<figure><img src="../.gitbook/assets/enviados05.png" alt=""><figcaption><p>Haz clic en la imagen para ampliar.</p></figcaption></figure>

#### **Mover Proceso (s)**

Al hacer clic en este ícono, será posible cambiar la carpeta donde se almacenan los documentos seleccionados. No se podrá ejecutar esta acción en documentos con el estado "Esperando".   &#x20;

<figure><img src="../.gitbook/assets/image (629).png" alt="" width="439"><figcaption></figcaption></figure>

#### **Alterar Proprietario**

&#x20;Al hacer clic en este ícono, será posible cambiar la propiedad de los documentos seleccionados, es decir, las funciones de administración del documento serán de otro usuario. Esta acción solo podrá deshacerse si el usuario que se defina como nuevo propietario devuelve la propiedad del documento al propietario original o la transfiere a otro usuario. El cambio de propietario de un documento en lote tiene un plazo de 24 horas para ser realizado, y para seguir el progreso, el usuario debe acceder al menú [<mark style="color:blue;">Mi Perfil > Pestaña Solicitudes</mark>](../menu-superior/meu-perfil.md#aba-solicitacoes).

{% hint style="warning" %}
<mark style="color:orange;">**Solo pueden ser seleccionados como nuevos propietarios usuarios registrados en la misma cuenta del responsable.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (630).png" alt=""><figcaption></figcaption></figure>

#### **Visualizar Documento**

&#x20;Al hacer clic en este ícono, será posible visualizar el documento o los documentos del proceso de firma. Esta opción debe utilizarse al seleccionar un proceso a la vez.

#### **Reenviar**

Al hacer clic en este ícono, será posible reenviar los documentos seleccionados a los destinatarios que aún no han firmado. Solo se podrá ejecutar esta acción en documentos que no tengan el estado “Concluido”.

<figure><img src="../.gitbook/assets/image (650).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Para la acción de reenvío en lote, el sistema no habilita el ícono de reenviar si al menos un proceso seleccionado está marcado como "Enviado vía ArqFlow".**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (810).png" alt=""><figcaption></figcaption></figure>

#### **Cancelar Envío**

Al hacer clic en este ícono, será posible cancelar el envío de los documentos seleccionados, interrumpiendo los procesos de firma. Solo se podrá ejecutar esta acción en documentos que no tengan el estado “Concluido”.

<figure><img src="../.gitbook/assets/image (651).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (1).png" alt="" width="328"><figcaption></figcaption></figure>

#### **E**liminar

Al hacer clic en este ícono, será posible eliminar los documentos seleccionados. Solo se podrá ejecutar esta acción en documentos con el estado “Concluido” o “Cancelado”.

<figure><img src="../.gitbook/assets/image (653).png" alt="" width="263"><figcaption></figcaption></figure>

#### **Falhas na entrega de emails**

Cuando haya una falla en el envío del proceso, el sistema señalará el proceso con la falla de envío.

Cuando haya una falla en el envío del código de seguridad para algún destinatario del proceso, el sistema señalará al destinatario con la falla de envío del código de seguridad.

<figure><img src="../.gitbook/assets/image (811).png" alt=""><figcaption></figcaption></figure>

## 🗪 Preguntas y Respuestas Frecuentes

<details>

<summary>¿Cómo compartir un Proceso firmado en la Plataforma ArqSign?</summary>

* Inicia sesión en tu cuenta ArqSign a través del enlace: [https://app.arqsign.com/auth/login](https://app.arqsign.com/auth/login)
* Haz clic en **'Enviados'**;
* Localiza el Proceso que deseas compartir;
* Esta opción permite que el usuario cree un enlace de acceso a uno o más documentos del proceso, el cual puede ser compartido con personas que no sean participantes del proceso de firma. Este enlace puede tener una vigencia determinada o indefinida, y el usuario puede definir si desea permitir que las personas que accedan también visualicen los anexos enviados por los firmantes.

- Cuando el Proceso tiene más de un documento **no agrupado** y **no tiene compartición activa**, el sistema abrirá una ventana para que el usuario seleccione qué documentos desea compartir.
- Cuando el Proceso tiene más de un documento **ya compartido**, el sistema mostrará la ventana con los enlaces que ya fueron generados.
- Al expandir las acciones del enlace compartido, es posible visualizar nuevamente la pantalla de compartición o eliminar el enlace generado.
- Al compartir los documentos del proceso, el usuario también tiene la posibilidad de enviarlos por correo electrónico haciendo clic en el botón **"Enviar enlace por correo"**.\
  Agrega en el campo correspondiente todos los correos electrónicos que deben recibir la documentación compartida.

</details>

<details>

<summary>¿Cómo cambiar el propietario de un Proceso?</summary>

Si eres el remitente de un Proceso con estado "Pendiente", "En proceso" o "Completado", puedes cambiar el propietario a otro usuario activo de la cuenta. De esta forma, las notificaciones automáticas del flujo pasarán a ser enviadas al nuevo propietario.

Para realizar este cambio, sigue uno de los siguientes métodos:

#### Opción 1:&#x20;

1. Localiza el flujo en el menú Enviados;
2. Haz clic en el menú desplegable ubicado en la esquina derecha;
3. Haz clic en Cambiar propietario;
4. Ingresa el nuevo propietario y guarda.

Si se transfiere solo un Proceso, el cambio se realiza de inmediato.

Si se transfieren dos o más Procesos, el sistema requiere 24 horas para completar la solicitud.

#### **Opción 2:**&#x20;

1. Al inactivar un usuario que posee Procesos en su cuenta, puedes transferirlos a otro usuario responsable;
2. Al hacer clic en 'Inactivar', aparecerá un cuadro de confirmación;
3. En ese cuadro, confirma que deseas transferir los Procesos;
4. Selecciona el nuevo propietario;
5. Elige los Procesos que deseas transferir por estado: 'Todos' o 'En firma o con renovación programada';
6. Haz clic en 'Cambiar';
7. El usuario será inactivado y los Procesos serán transferidos en un plazo de 24 horas;
8. Si el usuario no tiene Procesos en la cuenta, este procedimiento no es necesario;
9. La transferencia de Procesos solo puede hacerse a un usuario activo.
10. Para verificar el progreso de las solicitudes de transferencia, accede a:\
    "Mi perfil" → "Solicitudes".

Si deseas transferir la propiedad de los Procesos de un usuario que ya fue inactivado, consulta el paso a paso en: "¿Cómo inactivar un usuario y cambiar la propiedad de sus Procesos?"

</details>

<details>

<summary>¿Cómo verificar la versionado de los Procesos guardados en la plataforma?</summary>

Con cada renovación de Procesos a través de la herramienta de renovación de la Plataforma ArqSign, se realiza un vínculo de los nuevos Procesos con los anteriores.\
Para acceder a este recurso siga los siguientes pasos:

1. Menú "Enviados".
2. Ubique el Proceso que desea consultar.
3. En el botón "Historial", haga clic en el desplegable.
4. Elija la opción "Versionado".

Analice la información.

</details>

<details>

<summary>¿Cómo cancelar procesos enviados?</summary>

La cancelación de un Proceso o flujo puede realizarse mientras aún no se haya concluido. Para ello, siga el siguiente paso a paso:

1. Acceda al menú de Enviados;
2. Ubique el Proceso que desea cancelar;
3. Haga clic en Historial;
4. Haga clic en Cancelar;
5. Confirme la cancelación haciendo clic en Sí.

</details>

<details>

<summary>¿Cómo editar, corregir o cambiar el correo electrónico del firmante?</summary>

1. Acceda a la bandeja de enviados;
2. Ubique el Proceso cuyo correo electrónico del firmante desea editar, corregir o cambiar;
3. Haga clic en el botón de Reenviar;
4. Haga clic en Editar;
5. Realice la modificación necesaria;
6. Haga clic en Reenviar.

Cuando la fecha límite para la firma del Proceso haya vencido, el reenvío se realiza para todos los firmantes pendientes de firma en el orden actual.

Si la fecha límite para la firma del Proceso no ha vencido, el usuario podrá editarlo y reenviarlo a uno o más firmantes pendientes de firma en el orden actual.

[Haga clic aquí](https://app.gitbook.com/o/Ai1YjbPQxIuvTaVzoZ4H/s/zDlPVk00J5AKVvFiB3dg/) y vea el video con el paso a paso.

</details>

<details>

<summary>¿Cómo reenviar un Proceso?</summary>

1. Acceda a la bandeja de enviados;
2. Ubique el Proceso que desea reenviar;
3. Haga clic en el botón de Reenviar;
4. Haga clic nuevamente en el botón Reenviar.

Un nuevo envío se realizará únicamente para los firmantes que aún no hayan firmado el Proceso.

[Haga clic aquí](https://www.youtube.com/watch?v=K11hU-ZOWnk\&feature=youtu.be) y vea el video con el paso a paso.

</details>
