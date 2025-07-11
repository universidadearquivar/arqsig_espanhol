# 🟪 Configuración de directorios para clientes que ya han firmado documentos

## Creación de la estructura de directorios

### ETAPA 1 – Revisión de los permisos de los usuarios

Lo importante en esta etapa es garantizar que solo los usuarios que pueden tener acceso a todos los documentos que se están enviando para firma en la cuenta tengan el permiso de Administrador Global.

Para ello, accede a la pantalla [<mark style="color:blue;">Administración > Usuarios</mark> ](https://app.gitbook.com/o/Ai1YjbPQxIuvTaVzoZ4H/s/zDlPVk00J5AKVvFiB3dg/)y revisa los perfiles de usuarios asociados a la cuenta, asegurando que tengan el perfil de Remitente de Documentos (excepto el gestor de la cuenta, que debe poseer el perfil de Administrador Global).

<figure><img src="../../.gitbook/assets/image (709).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Solo los usuarios con perfil de Administrador Global podrán acceder a todas las carpetas del directorio.**</mark>
{% endhint %}

***

### ETAPA 2 – Creación de carpetas sectoriales

1\. Identifica los sectores que usarán la Plataforma ArqSign para el envío de documentos para firma, y de acuerdo con estos sectores, crea una carpeta para cada uno. Para ello, en la pantalla [Carpetas](https://manual.arquivar.com/manual-arqsign-or-espanhol/directorios/documentos), accede a la <mark style="color:blue;">carpeta raíz</mark> y haz clic en el ícono "Incluir carpeta".

<figure><img src="../../.gitbook/assets/image (12) (1).png" alt=""><figcaption></figcaption></figure>

2. Ingresa el nombre del sector y haz clic en Guardar.

<figure><img src="../../.gitbook/assets/image (13) (1).png" alt="" width="524"><figcaption></figcaption></figure>

3\. Repite el proceso hasta concluir la creación de todas las carpetas necesarias.

<figure><img src="../../.gitbook/assets/image (14) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**El Administrador Global debe realizar todas las configuraciones, ajustes de permisos, liberación de usuarios, etc., antes de iniciar el envío de documentos para firma.**</mark>
{% endhint %}

***

### ETAPA 3 – Movimiento de documentos a las carpetas

Acceda a la [<mark style="color:blue;">carpeta raíz de Directorios</mark>](./#pasta-raiz-de-diretorios), seleccione todos los documentos que desea mover a una carpeta específica y haga clic en el ícono “Mover”.

<figure><img src="../../.gitbook/assets/image (15) (1).png" alt=""><figcaption></figcaption></figure>

Seleccione en la lista la carpeta a la cual desea mover los documentos seleccionados y haga clic en “Mover”.

<figure><img src="../../.gitbook/assets/image (16) (1).png" alt="" width="375"><figcaption></figcaption></figure>

Repita el proceso con todos los documentos sueltos que aún estén en la carpeta raíz. Lo ideal es que todos los documentos se almacenen en alguna de las carpetas creadas, evitando la permanencia de documentos sueltos en la carpeta raíz.

***

### ETAPA 4 - Creación de grupos por sectores o funciones

Cree grupos de usuarios separándolos por sectores, funciones o combinando ambos. Para ello, acceda a la pantalla[ <mark style="color:blue;">Administración > Grupos de Usuarios</mark>](../../administracao/administracao/grupo-de-usuarios.md).

{% hint style="info" %}
<mark style="color:blue;">Estos grupos se utilizarán para asignar permisos en las carpetas, por lo que la forma de crearlos dependerá de cómo desee atribuir los permisos en las carpetas. Nuestra sugerencia es combinar el sector y la función, como por ejemplo:</mark>

* <mark style="color:blue;">Comercial – Gerencia</mark>
* <mark style="color:blue;">Comercial – Vendedores</mark>
* <mark style="color:blue;">Comercial - Otras funciones con lectura</mark>
{% endhint %}

<figure><img src="../../.gitbook/assets/image (18) (1).png" alt=""><figcaption></figcaption></figure>

***

### ETAPA 5 - Inserción de los grupos creados en la carpeta raíz

Los grupos creados en la etapa anterior deben ser insertados en la [<mark style="color:blue;">carpeta raíz de Directorios</mark>](./#pasta-raiz-de-diretorios) con permiso de "Lector". Para ello, en la carpeta raíz, haga clic en Acciones > Editar Permisos.

<figure><img src="../../.gitbook/assets/image (19) (1).png" alt=""><figcaption></figcaption></figure>

Haga clic en el ícono "Incluir".

<figure><img src="../../.gitbook/assets/image (20) (1).png" alt=""><figcaption></figcaption></figure>

Seleccione cada uno de los grupos creados en la etapa anterior y en la columna "Perfil" asigne el perfil de "Lector de Documentos" a todos los grupos. Haga clic en el ícono "Confirmar" para guardar los cambios.

<figure><img src="../../.gitbook/assets/image (21) (1).png" alt=""><figcaption></figcaption></figure>

***

### ETAPA 6 - Ajuste de las permisos de las carpetas sectoriales

Los permisos de las carpetas sectoriales deben ajustarse para que el acceso sea realizado solamente por personas del sector, y para esto será necesario:

**1. Dejar de heredar los permisos de la carpeta raíz:** En la columna "Acciones" de la carpeta sectorial deseada, haga clic en "Editar Permisos". Haga clic en "Dejar de Heredar".

<figure><img src="../../.gitbook/assets/image (22) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (24) (1).png" alt=""><figcaption></figcaption></figure>

**2. Excluir los grupos de otros sectores:** Seleccione todos los demás grupos/sectores que no deben tener acceso al contenido de la carpeta seleccionada y haga clic en el ícono "Eliminar". Deben permanecer solo los grupos que podrán acceder a la carpeta.

<figure><img src="../../.gitbook/assets/image (25) (1).png" alt=""><figcaption></figcaption></figure>

**3. Editar el perfil de acceso del sector en cuestión:** Ajuste los permisos de los grupos restantes seleccionándolos y haciendo clic en el ícono "Editar".

<figure><img src="../../.gitbook/assets/image (26) (1).png" alt=""><figcaption></figcaption></figure>

**4. En la columna "Perfil":** Defina si ese grupo continuará solo como "Lector de Documentos" o si será "Administrador de Documentos y Carpetas" o "Colaborador de Documentos".

* _Administrador de Documentos y Carpetas_: Un usuario o grupo de usuarios con este perfil de directorios puede consultar y descargar contenido, incluir, mover, compartir y renombrar documentos, excluir o incluir nuevas carpetas, además de poder cambiar permisos de acceso.
* _Colaborador de Documentos_: Un usuario o grupo de usuarios con este perfil de directorios puede consultar y descargar contenido, incluir, mover, compartir y renombrar documentos en la carpeta a la que tiene este perfil.
*   _Lector de Documentos_: Un usuario o grupo de usuarios con este perfil de directorios puede únicamente consultar y descargar el contenido de la carpeta y documentos.

    <figure><img src="../../.gitbook/assets/image (27) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Este proceso debe repetirse para todas las demás carpetas sectoriales y subcarpetas que puedan ser creadas dentro de las carpetas de los sectores.**</mark>
{% endhint %}

***

## P**ermisos para Directorios**

Solo el Administrador Global de la cuenta tendrá acceso al menú de directorios, y por este motivo es tan importante asegurarse de que solo personas sin restricciones de acceso estén con este perfil. A continuación, se muestran las diferencias entre los permisos otorgados a cada perfil:

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Todos los usuarios deben estar asociados a un grupo de permisos. De esta manera, la plataforma obligará al usuario a guardar el documento en una carpeta sectorial, evitando que los documentos se almacenen en la carpeta raíz.**</mark>
{% endhint %}

***

## Creación/Mantenimiento de Permisos por usuario

Una vez creada la estructura de directorios y aplicados los permisos, el mantenimiento en la Plataforma se resume en incluir o excluir usuarios de los grupos para que accedan o dejen de acceder a determinada carpeta.

Este mantenimiento puede realizarse en la edición del usuario o en la edición de un grupo específico.

**Edición de un grupo específico**: Acceda a la pantalla [<mark style="color:blue;">Administración > Grupo de Usuarios</mark>](../../administracao/administracao/grupo-de-usuarios.md). Seleccione el grupo deseado e incluya o excluya usuarios.

**Edición del usuario**: Acceda a la pantalla [<mark style="color:blue;">Administración > Usuarios</mark>](../../administracao/administracao/usuarios.md). Seleccione el usuario que desea editar y haga clic en “Editar”. Defina los grupos a los que el usuario debe tener acceso y haga clic en “Guardar”.

***

## Reglas Generales de Directorios

<details>

<summary>Carpetas</summary>

1. Toda cuenta, al ser creada, automáticamente tendrá una carpeta raíz asociada.
2. La carpeta raíz creada automáticamente por la plataforma recibe el nombre de la cuenta y puede ser renombrada posteriormente por su Administrador Global.
3. Para cada cuenta se permite una única carpeta raíz. Las demás carpetas deben ser creadas obligatoriamente dentro de la carpeta raíz..
4. &#x20;Los documentos exhibidos en "Directorios" son solamente aquellos con estado "Concluido" y que no estén "Excluidos", es decir, si el documento está en proceso de firma, no aparecerá en el directorio.eja, se o documento estiver em processo de assinatura ele não vai aparecer no diretório.

</details>

<details>

<summary>Perfil de Usuarios</summary>

1. El perfil de usuario Administrador Global tiene acceso total al directorio de documentos, siempre que el plan de la cuenta incluya acceso a la funcionalidad de directorios.
2. El perfil de usuario Remitente de Documentos tendrá acceso a la navegación en las carpetas si forma parte de algún grupo que tenga al menos permiso de lectura.

</details>

