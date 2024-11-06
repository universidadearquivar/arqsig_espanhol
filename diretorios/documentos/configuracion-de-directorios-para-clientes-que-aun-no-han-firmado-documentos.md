# 🟪 Configuración de directorios para clientes que aún no han firmado documentos

## Creación de la estructura de directorios

### ETAPA 1 - Estructuración de directorios

1\. Identifique qué sectores utilizarán la Plataforma ArqSign para el envío de documentos para firma y, de acuerdo con estos sectores, cree una carpeta para cada uno. Para ello, en la pantalla [<mark style="color:blue;">Documentos</mark>](./), acceda a la carpeta raíz y haga clic en el ícono "Incluir Carpeta".

<figure><img src="../../.gitbook/assets/image (695).png" alt=""><figcaption></figcaption></figure>

2\. Informe el nombre del sector y haga clic en Guardar.

<figure><img src="../../.gitbook/assets/image (696).png" alt=""><figcaption></figcaption></figure>

3\. Repita el proceso hasta concluir la creación de todas las carpetas necesarias.

<figure><img src="../../.gitbook/assets/image (697).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**El Administrador Global debe realizar todas las configuraciones, ajustes de permisos, liberación de usuarios, etc., antes del inicio del envío de documentos para firma.**</mark>
{% endhint %}

***

### ETAPA 2 - Creación de grupos por sectores o funcionales

Cree grupos de usuarios separándolos por sectores, funciones o mezclando entre ambos. Para ello, acceda a la pantalla [<mark style="color:blue;">Administración > Grupos de Usuarios</mark>](../../administracao/administracao/grupo-de-usuarios.md).

{% hint style="info" %}
<mark style="color:blue;">Estos grupos se utilizarán para asignar permisos en las carpetas, por lo que la forma de crearlos dependerá de cómo desee asignar los permisos en las carpetas. Nuestra sugerencia es mezclar el sector y la función, como por ejemplo:</mark>

* <mark style="color:blue;">Comercial – Gerencia</mark>
* <mark style="color:blue;">Comercial – Vendedores</mark>
* <mark style="color:blue;">Comercial - Otras funciones con lectura</mark>
{% endhint %}

***

<figure><img src="../../.gitbook/assets/image (698).png" alt=""><figcaption></figcaption></figure>

### ETAPA 3 - Inserción de los grupos creados en la carpeta raíz

Los grupos creados en la etapa anterior deben ser insertados en la [<mark style="color:blue;">carpeta raíz de Directorios</mark>](./#pasta-raiz-de-diretorios) con permiso de "Lector". Para ello, en la carpeta raíz haga clic en Acciones > Editar Permisos.

<figure><img src="../../.gitbook/assets/image (699).png" alt=""><figcaption></figcaption></figure>

Haga clic en el ícono "Incluir".

<figure><img src="../../.gitbook/assets/image (700).png" alt=""><figcaption></figcaption></figure>

Seleccione cada uno de los grupos creados en la etapa anterior y en la columna "Perfil" asigne el perfil de "Lector de Documentos" para todos los grupos. Haga clic en el ícono "Confirmar" para guardar los cambios.

<figure><img src="../../.gitbook/assets/image (701).png" alt=""><figcaption></figcaption></figure>

***

### ETAPA 4 - Ajuste de permisos de las carpetas sectoriales

Los permisos de las carpetas sectoriales deben ajustarse para que el acceso se realice únicamente por personas del sector, y para ello será necesario:

**1. Dejar de heredar el permiso de la carpeta raíz:** En la columna "Acciones" de la carpeta sectorial deseada, haga clic en "Editar Permisos". Haga clic en "Dejar de Heredar".

<figure><img src="../../.gitbook/assets/image (702).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (704).png" alt=""><figcaption></figcaption></figure>

**2. Excluir los grupos de otros sectores:** Seleccione todos los demás grupos/sectores que no deben tener acceso al contenido de la carpeta seleccionada y haga clic en el ícono “Excluir”. Deben permanecer solo los grupos que podrán acceder a la carpeta.

<figure><img src="../../.gitbook/assets/image (705).png" alt=""><figcaption></figcaption></figure>

**3. Editar el perfil de acceso del sector en cuestión:** Ajuste las permisos de los grupos restantes seleccionándolos y haciendo clic en el ícono “Editar”.

<figure><img src="../../.gitbook/assets/image (706).png" alt=""><figcaption></figcaption></figure>

**4. En la columna “Perfil”:** Defina si ese grupo continuará solo como “Lector de Documentos” o si será “Administrador de Documentos y Carpetas” o “Colaborador de Documentos”.

* **Administrador de Documentos y Carpetas:** Un usuario o grupo de usuarios con este perfil de directorios puede consultar y descargar contenido, incluir, mover, compartir y renombrar documentos, excluir o incluir nuevas carpetas, además de poder cambiar permisos de acceso.
* **Colaborador de Documentos:** Un usuario o grupo de usuarios con este perfil de directorios puede consultar y descargar contenido, incluir, mover, compartir y renombrar documentos en la carpeta a la que tiene este perfil.&#x20;
*   **Lector de Documentos:** Un usuario o grupo de usuarios con este perfil de directorios puede únicamente consultar y descargar el contenido de la carpeta y documentos.

    <figure><img src="../../.gitbook/assets/image (707).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Este proceso debe repetirse para todas las demás carpetas sectoriales y subcarpetas que puedan ser creadas dentro de las carpetas de los sectores.**</mark>
{% endhint %}

***

## Permisos para Directorios

Solo el Administrador Global de la cuenta tendrá acceso al menú de directorios, y por esta razón es tan importante asegurarse de que solo personas sin restricciones de acceso tengan este perfil. A continuación, se presentan las diferencias entre los permisos concedidos a cada perfil:

<figure><img src="../../.gitbook/assets/image (708).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Todos los usuarios deben estar asociados a un grupo de permisos. De esta manera, la plataforma obligará al usuario a guardar el documento en una carpeta sectorial, evitando que los documentos se almacenen en la carpeta raíz.**</mark>
{% endhint %}

***

## Creación/Mantenimiento de Permisos por usuario

Una vez creada la estructura de directorios y aplicados los permisos, el mantenimiento en la Plataforma se resume en incluir o excluir usuarios de los grupos para que accedan o dejen de acceder a determinadas carpetas.

Este mantenimiento puede realizarse en la edición del usuario o en la edición de un grupo específico.

**Edición de un grupo específico:** Acceda a la pantalla [<mark style="color:blue;">Administración > Grupo de Usuarios</mark>](../../administracao/administracao/grupo-de-usuarios.md). Seleccione el grupo deseado e incluya o excluya usuarios.

**Edición del usuario:** Acceda a la pantalla [<mark style="color:blue;">Administración > Usuarios</mark>](https://app.gitbook.com/s/zDlPVk00J5AKVvFiB3dg/sending-and-signing-a-document/sending-documents). Seleccione el usuario que desea editar y haga clic en “Editar”. Defina los grupos a los que el usuario debe tener acceso y haga clic en “Guardar”.

***

## Reglas Generales de Directorios

<details>

<summary><strong>Carpetas</strong></summary>

1. Toda cuenta al ser creada, automáticamente tendrá una carpeta raíz asociada.
2. La carpeta raíz creada automáticamente por la plataforma recibe el nombre de la cuenta y puede ser renombrada posteriormente por su Administrador Global.
3. &#x20;Para cada cuenta se permite una única carpeta raíz. Las demás carpetas deben ser creadas obligatoriamente dentro de la carpeta raíz.
4. Los documentos exhibidos en "Directorios" son solamente aquellos con estado "Concluido" y que no estén "Eliminados", es decir, si el documento está en proceso de firma no aparecerá en el directorio.

</details>

<details>

<summary>Perfil de Usuarios</summary>

1. El perfil del usuario Administrador Global tiene acceso total al directorio de documentos, siempre que el plan de la cuenta tenga acceso a la funcionalidad de directorios.
2. El perfil de usuario Remitente de Documentos tendrá acceso a la navegación en las carpetas si forma parte de algún grupo que tenga permiso de al menos lectura.

</details>
