# 🟪 Usuarios

En el menú Usuarios se presentan todos los usuarios que participan en la cuenta del usuario que ha iniciado sesión.

Los usuarios administradores globales pueden invitar a otras personas para que participen en la cuenta y realicen acciones en la plataforma.

La cantidad de usuarios que pueden ser invitados varía según el plan contratado. En el plan gratuito, solo es posible que un usuario acceda a la cuenta.

En los planes de pago, se pueden crear tantos usuarios como sea necesario (ilimitados).

<figure><img src="../../.gitbook/assets/image (8) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Después de que el Administrador registre un nuevo usuario, el invitado recibe por correo electrónico una invitación para unirse a la cuenta. Si ya tiene un registro en la plataforma, solo deberá ingresar su contraseña. Si aún no tiene uno, deberá ingresar su nombre y crear una contraseña para realizar el primer acceso.

<figure><img src="../../.gitbook/assets/image (736).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (738).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (740).png" alt=""><figcaption></figcaption></figure>

***

## Columnas de la pantalla principal – Usuarios

<figure><img src="../../.gitbook/assets/image (741).png" alt=""><figcaption></figcaption></figure>

**Correo electrónico:** Muestra el correo electrónico de los usuarios asociados o invitados a la cuenta.

**Nombre:** Presenta los nombres de los usuarios. Para los usuarios con estado “Pendiente” no se muestra el nombre, ya que aún no se han registrado en la plataforma.

**Fecha de Registro:** Muestra la fecha y hora en que el usuario fue registrado en la cuenta.

**Perfiles:** Muestra los perfiles asignados al usuario, que pueden ser Administrador (acceso a todas las funcionalidades) y Remitente de Documentos (envía y firma documentos). Un mismo usuario puede tener ambos perfiles.

**Estado:** Presenta el estado del usuario, que puede ser “Activo” (ya está registrado en la cuenta), “Pendiente” (aún no ha aceptado la invitación para unirse a la cuenta), “Bloqueado” o “Inactivo” (usuario que ya no forma parte de la cuenta).

{% hint style="info" %}
<mark style="color:blue;">**DIFERENCIA ENTRE USUARIO BLOQUEADO E INACTIVO:**</mark>&#x20;

<mark style="color:blue;">Al</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**bloquear un usuario**</mark><mark style="color:blue;">, se impide su acceso a la cuenta. Los documentos que son de su responsabilidad permanecen con él, y al desbloquearlo, el usuario continuará teniendo acceso a ellos normalmente. Esta funcionalidad es útil en casos de ausencia temporal de un empleado, por ejemplo.</mark>&#x20;

<mark style="color:blue;">Al</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**inactivar un usuario**</mark><mark style="color:blue;">, se impide su acceso a la cuenta, y los documentos que son de su responsabilidad pueden permanecer con él o ser transferidos a otro propietario. Si se reactiva al usuario y los documentos fueron transferidos, perderá el acceso a esos archivos; si no fueron transferidos, seguirá teniendo acceso a ellos normalmente. Esta funcionalidad es útil en casos de desvinculación de un empleado, por ejemplo.</mark>
{% endhint %}

***

## Acciones de la pantalla – Usuarios

Las acciones de la pantalla de Usuarios pueden accederse a través de los botones superiores, de la columna de acciones a la derecha o haciendo clic en cualquier información del usuario en la cuadrícula de la pantalla principal.

<div align="left"><figure><img src="../../.gitbook/assets/image (742).png" alt="" width="375"><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (854).png" alt="" width="319"><figcaption></figcaption></figure></div>

**Nuevo:** Para invitar a un nuevo usuario a unirse a la cuenta, haz clic en “Nuevo”. Por defecto, el usuario tendrá el estado “Pendiente” hasta que acepte la invitación para unirse a la cuenta.&#x20;

Se debe ingresar el correo electrónico del usuario y definir el tipo de perfil que se le asignará, que puede ser Administrador (acceso a todas las funcionalidades), Remitente de Documentos (envía y firma documentos) o ambos.

<figure><img src="../../.gitbook/assets/image (744).png" alt=""><figcaption></figcaption></figure>

Si el usuario invitado tiene únicamente el perfil de Remitente de Documentos, también será necesario definir el Grupo de Usuarios al cual estará asociado. Este grupo de usuarios determinará a qué carpetas del directorio tendrá acceso el nuevo miembro de la cuenta y deberá haberse creado previamente en el menú [<mark style="color:blue;">Administración > Grupo de Usuarios</mark>](grupo-de-usuarios.md). También es posible crear un grupo haciendo clic en “Nuevo Grupo”.

<figure><img src="../../.gitbook/assets/image (745).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**La asignación de grupo no se solicita para los usuarios creados con el perfil de Administrador, ya que estos usuarios tienen acceso a todas las carpetas de**</mark> [<mark style="color:blue;">**Documentos del Directorio**</mark>](../../diretorios/documentos/)<mark style="color:orange;">**, por lo que no es necesario aplicar esta restricción.**</mark>
{% endhint %}

**Activar:** Solo se pueden activar usuarios con estado “Bloqueado” o “Inactivo”. Al activar a los usuarios bloqueados o inactivos, tendrán acceso nuevamente a la cuenta.

<figure><img src="../../.gitbook/assets/image (746).png" alt=""><figcaption></figcaption></figure>

**Bloquear:** Podem ser bloqueados apenas usuários com status “Ativo”. Usuários bloqueados perdem a propriedade de todos os documentos.

<figure><img src="../../.gitbook/assets/image (747).png" alt=""><figcaption></figcaption></figure>

Editar: Se utiliza para editar la información del usuario.

**Inactivar:** Solo se pueden inactivar usuarios con estado “Activo”. Al inactivar un usuario, será necesario definir si los documentos enviados por ese usuario serán transferidos a otro miembro de la cuenta o si se procederá a la inactivación sin transferencia.

Si se elige la opción “Inactivar sin Transferir”, el usuario, aunque inactivo, seguirá siendo el propietario de los documentos.

<figure><img src="../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>

Si se elige la opción “Transferir”, será necesario informar quién será el nuevo propietario de los documentos y si se transferirán todos los documentos o solo aquellos en proceso de firma o con renovación programada.

<figure><img src="../../.gitbook/assets/image (749).png" alt=""><figcaption></figcaption></figure>

**Excluir:** Solo se pueden excluir de la cuenta aquellos usuarios con estado “Pendiente”, es decir, que han sido invitados pero aún no se han unido a la cuenta.

<figure><img src="../../.gitbook/assets/image (750).png" alt=""><figcaption></figcaption></figure>

**Filtrar:** Es posible buscar un usuario utilizando los filtros disponibles en la barra de búsqueda superior.

<figure><img src="../../.gitbook/assets/image (751).png" alt=""><figcaption></figcaption></figure>
