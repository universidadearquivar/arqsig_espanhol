# 👤 Mi Perfil

{% embed url="https://app.supademo.com/demo/cmcxgg3sy0h9vc4kj92q5x9cz" %}

En el menú Mi Perfil se presentan la información del usuario autenticado. &#x20;

<figure><img src="../.gitbook/assets/image (82).png" alt="" width="393"><figcaption></figcaption></figure>

***

## Pestaña Mis Datos&#x20;

En la pestaña Mis Datos se presentan la información de registro del usuario. Es posible editar los datos haciendo clic en el botón "Editar".

<figure><img src="../.gitbook/assets/image (83).png" alt=""><figcaption></figcaption></figure>

**Foto de perfil:** Para insertar o editar la foto de perfil, haga clic en la imagen y seleccione la opción "Subir Nueva Imagen". Elija la foto deseada y haga clic en "Guardar". Para eliminar la foto de perfil, simplemente haga clic en la foto y seleccione la opción "Eliminar Imagen Actual".

<figure><img src="../.gitbook/assets/image (84).png" alt="" width="215"><figcaption></figcaption></figure>

**Correo electrónico**: El correo electrónico mostrado en este campo es el mismo utilizado al momento del registro de la cuenta del usuario en la plataforma y no puede ser modificado.

Si desea utilizar otro correo como "Remitente de documentos", cree otro [**usuario** ](../administracao/administracao/usuarios.md)para este correo. En la Plataforma ArqSign, los usuarios son ilimitados.

**Nombre completo:** Presenta el nombre completo del usuario. El nombre registrado en este campo aparece como el remitente de documentos de este usuario en los correos electrónicos y mensajes de WhatsApp.

**Cargo:** El usuario puede informar en este campo el cargo que ocupa en la empresa en la que trabaja.

**Tipo de documento de identificación:** En este campo, el usuario debe elegir un documento de identificación que puede ser CPF, CNH, RG u otro documento.

**Número de identificación:** En este campo, el usuario debe informar el número del documento elegido en el campo "Tipo de documento de identificación".

**Zona horaria:** En este campo, el usuario puede elegir la zona horaria que desea que la plataforma considere. Esta configuración es útil para las parametrizaciones que involucran programaciones, por ejemplo.

**Su idioma predeterminado:** El usuario puede elegir el idioma predeterminado en el que desea que se presente la interfaz de la plataforma entre "Portugués – Brasil", "Inglés – EE.UU." y "Español – España".

**Teléfono:** En este campo, el usuario debe ingresar su número de teléfono de contacto y hacer clic en "Agregar Teléfono". Los números ingresados aquí se mostrarán justo abajo, en el campo "Teléfonos".\


<figure><img src="../.gitbook/assets/image (85).png" alt=""><figcaption></figcaption></figure>

***

## Pestaña Mis Contactos&#x20;

En la pestaña Mis Contactos, el usuario puede registrar información de destinatarios para el envío de documentos.

**Guardar los destinatarios de un documento enviado para firma en mi lista de contactos:** Al dejar marcada esta opción, cada vez que el usuario envíe un documento para firma a un destinatario que aún no esté incluido en la lista de contactos, la información de contacto de ese destinatario se guardará automáticamente y pasará a formar parte de la lista.

<figure><img src="../.gitbook/assets/image (584).png" alt=""><figcaption></figcaption></figure>

**Columna Nombre:** En esta columna se presenta el nombre del contacto tal como fue registrado en la lista o como fue informado durante el envío de un documento. Si el contacto ha sido compartido con el usuario por otro miembro de la cuenta, se mostrará el nombre del contacto seguido de la información de quién lo registró.

**Columna Correo electrónico / WhatsApp:** En esta columna se presenta el nombre o el correo electrónico del contacto informado en el registro o durante el envío de un documento.

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

**Ícono Agregar Contacto:** Para agregar un nuevo contacto, haga clic en el ícono "Agregar Contacto" e informe el nombre y correo electrónico o número de WhatsApp del contacto. Al seleccionar la opción "Compartir con todos los usuarios de la cuenta", el contacto registrado se guardará en la lista de contactos de todos los usuarios que forman parte de la cuenta. Para concluir, haga clic en "Guardar".

<figure><img src="../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure>

**Ícono Editar Contacto:** Para editar la información de un contacto, seleccione el destinatario deseado marcando la casilla de verificación a la izquierda y haga clic en el ícono "Editar Contacto".

**Ícono Eliminar Contacto(s):** Para eliminar uno o más contactos, seleccione los deseados marcando la casilla de verificación a la izquierda y haga clic en el ícono "Eliminar Contacto(s)".

{% hint style="warning" %}
<mark style="color:orange;">**Solo es posible editar o eliminar contactos que hayan sido registrados por el propio usuario.**</mark>
{% endhint %}

**Barra de Búsqueda:** Es posible localizar un contacto específico utilizando los filtros de correo electrónico o WhatsApp para la búsqueda.

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

#### Importación de Contactos

Además de la opción de añadir nuevos contactos manualmente, el sistema también permite la importación de datos mediante un archivo en formato CSV. Para ello:

* Acceda a **Mi perfil** en el menú superior.
* Haga clic en la pestaña **Mis contactos**.
* Haga clic en el ícono de **importación** que aparece junto a la lista de contactos.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

Se abrirá una ventana para realizar la carga del archivo CSV.

<figure><img src="../.gitbook/assets/image (2).png" alt="" width="410"><figcaption></figcaption></figure>

#### Hoja modelo

Haga clic en **Descargar hoja modelo** para descargar un archivo CSV en blanco.\
Este es el modelo que debe utilizarse para la importación.

Complete el archivo según las siguientes instrucciones:

* **Campo "Compartido":** Complete con **1** para indicar "Sí" o **0** para indicar "No". Cualquier valor diferente será considerado como "0".
* **Campo "Teléfono":** Debe ser informado en el formato internacional, con **DDI + DDD + número**. Ejemplo: 553198766871.
* **Campos "Correo electrónico" y "Teléfono" completados:** Si ambos campos están llenos, el contacto será importado dos veces. Para importar solo una vez, complete solo uno de los campos.

<figure><img src="../.gitbook/assets/image (3).png" alt="" width="375"><figcaption></figcaption></figure>

#### Importación y registros

Si el archivo contiene errores en algún campo, solo se importarán los registros válidos. Se generará un **LOG de fallos** (según se indica en verde a continuación) que podrá ser descargado para corregir el archivo e intentar una nueva importación.

<figure><img src="../.gitbook/assets/image (4).png" alt="" width="410"><figcaption></figcaption></figure>

Los registros que ya existan en la lista no serán duplicados.

La importación puede tardar algunos segundos o minutos, dependiendo del tamaño del archivo.\
El usuario puede cerrar la pantalla y consultar los datos posteriormente.

***

## Mensaje Predeterminado

En la pestaña Mensaje Predeterminado, el usuario podrá crear varios mensajes específicos para seleccionar al momento de enviar un documento para firma.

<figure><img src="../.gitbook/assets/image (68).png" alt=""><figcaption></figcaption></figure>

**Agregar:** Haga clic en Agregar "+", para incluir un nuevo mensaje.

<figure><img src="../.gitbook/assets/image (69).png" alt=""><figcaption></figcaption></figure>

Complete los campos presentados en la pantalla, prestando atención al límite de caracteres permitidos en cada uno de ellos. Haga clic en Guardar.

<figure><img src="../.gitbook/assets/image (70).png" alt="" width="344"><figcaption></figcaption></figure>

El mensaje predeterminado creado se mostrará al firmante según la imagen; observe el área destacada, donde se encuentra el texto previamente registrado en la plataforma.

<figure><img src="../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure>

Cuando el destinatario no defina un mensaje predeterminado de su lista, la plataforma deberá considerar el mensaje predeterminado del sistema. Observe en el área destacada la información del proceso recibido considerando el nombre de los archivos adjuntos al proceso.

Repita el proceso hasta agregar todos los mensajes que desea mantener como predeterminados.

En caso de mensajes enviados a través de WhatsApp, el mensaje predeterminado tendrá un formato diferente, y se mostrará de la siguiente manera:

<figure><img src="../.gitbook/assets/image (5).png" alt="" width="281"><figcaption></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">La lista de mensajes predeterminados no puede ser compartida entre usuarios, es decir, cada usuario podrá visualizar y/o seleccionar solo los mensajes creados por él.</mark>
{% endhint %}

**Editar:** Seleccione en la lista el mensaje que desea modificar, así el sistema habilitará la opción de Editar.

**Excluir:** Seleccione en la lista el mensaje que desea eliminar.

**Filtrar:** Utilice esta opción para buscar un mensaje predeterminado específico en la lista disponible.

***

## Pestaña Estilo de Firma&#x20;

En la pestaña Estilo de Firma, el usuario debe definir la representación visual de su firma. El usuario puede registrar tres tipos de Estilo de Firma haciendo clic en "Editar".

<figure><img src="../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure>

**Estilo Predeterminado:** En este estilo de firma, el usuario debe ingresar su nombre completo y definir el estilo de fuente para el texto. Para ello, debe hacer clic en "Estilo" y realizar la configuración. Para eliminar, debe hacer clic en el ícono de la papelera.

<figure><img src="../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure>

**Estilo Diseño:** Para firmar con un diseño, el usuario deberá, en el campo "Área de Diseño de la Firma", dibujar su firma utilizando el mouse o el dedo si está usando un celular o tablet. Para corregir, debe hacer clic en el ícono de la papelera.

<figure><img src="../.gitbook/assets/image (74).png" alt=""><figcaption></figcaption></figure>

**Estilo Imagen:** Si lo desea, el usuario puede subir la imagen que represente su firma. Para eliminar, debe hacer clic en el ícono de la papelera.

<figure><img src="../.gitbook/assets/image (75).png" alt=""><figcaption></figcaption></figure>

Los estilos de firma para las representaciones visuales registradas aquí se mostrarán al usuario siempre que deba [<mark style="color:blue;">firmar un documento</mark>](https://app.gitbook.com/o/Ai1YjbPQxIuvTaVzoZ4H/s/zDlPVk00J5AKVvFiB3dg/). Para concluir la inclusión de uno de los Estilos de Firma, selecciónelo y haga clic en "Aplicar".

***

## Pestaña Certificado Digital&#x20;

En la pestaña Certificado Digital, deben registrarse los certificados digitales del tipo A1 que el usuario utilizará para la firma de documentos.

En la pantalla principal se presentan las informaciones de todos los certificados registrados por el usuario. &#x20;

<figure><img src="../.gitbook/assets/image (76).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">Los certificados digitales del tipo A1 almacenan la firma del usuario en su propia máquina y tienen una contraseña para el acceso. Al importar un certificado digital A1, se alojará en la plataforma ArqSign (nube), pudiendo ser utilizado para realizar la firma en cualquier dispositivo o computadora.</mark>
{% endhint %}

Para realizar la carga de un certificado, el usuario debe hacer clic en el ícono "Nuevo", importar el archivo del certificado, definir un nombre e ingresar la contraseña del certificado.

<figure><img src="../.gitbook/assets/image (78).png" alt=""><figcaption></figcaption></figure>

***

## Pestaña Solicitudes&#x20;

En el menú Solicitudes se presentan todas las solicitudes de transferencia de documentos realizadas por el usuario. Siempre que en los menús [<mark style="color:blue;">Documentos</mark>](../diretorios/documentos/)<mark style="color:blue;">,</mark> [<mark style="color:blue;">Bandeja de Entrada</mark>](../caixa-postal/caixa-de-entrada.md) <mark style="color:blue;">y</mark> [<mark style="color:blue;">Enviados</mark>](../caixa-postal/enviados.md) el usuario transfiera la propiedad de un documento de su autoría a otro usuario, esta solicitud se mostrará aquí.

También se incluirán las solicitudes de transferencia de propiedad de documentos debido a la [<mark style="color:blue;">desactivación de usuarios</mark>](../administracao/administracao/usuarios.md#acoes-da-tela-usuarios) de la cuenta.

Si se solicita la transferencia de un solo documento, se realiza de manera instantánea, pero si la solicitud de transferencia es en lote, puede tardar hasta 24 horas en ejecutarse.&#x20;

<figure><img src="../.gitbook/assets/image (79).png" alt=""><figcaption></figcaption></figure>

**Fecha de Solicitud:** En esta columna se presenta la fecha en que el usuario solicitó la transferencia de los documentos.

**Responsable Anterior:** Nombre del usuario que solicitó la transferencia de propiedad del documento.

**Nuevo Responsable:** Nombre del usuario que será el nuevo propietario del documento.

Cantidad: Cantidad de documentos que se transferirán al nuevo responsable.

**Estado de Solicitud:** El estado de una solicitud de transferencia puede ser "Finalizado" (la transferencia se ha completado), "En proceso" (la transferencia está siendo procesada y debe ocurrir en un plazo de hasta 24 horas después de la solicitud) o "Solicitado" (se ha programado una fecha futura para que la transferencia ocurra).

**Fecha de Conclusión:** Fecha de finalización de la transferencia de propiedad.

<figure><img src="../.gitbook/assets/image (80).png" alt=""><figcaption></figcaption></figure>

**Acciones:** Si el estado de la solicitud es "Finalizado" o "En proceso", no será posible ejecutar ninguna acción en relación a ella. Si el estado aún es "Solicitado", se podrán realizar dos acciones respecto a la solicitud:

* **Cancelar:** Cancela la transferencia de propiedad.
* **Editar:** Modifica el usuario definido como el nuevo propietario del documento.

<figure><img src="../.gitbook/assets/image (81).png" alt="" width="563"><figcaption></figcaption></figure>

## 🗪 Preguntas y Respuestas Frecuentes

<details>

<summary>¿Cómo guardar contactos en la plataforma ArqSign?</summary>

Usted puede guardar contactos en la Plataforma ArqSign de dos formas.

_Primera forma:_

Al registrar un destinatario, mantenga marcada la casilla "Guardar este destinatario en mi lista de contactos".

_Segunda forma:_

1. Acceda al menú "Mi Perfil"
2. Acceda a la opción "Mis contactos"
3. Para agregar un contacto, haga clic en el botón +, ingrese los datos, elija si desea compartir el contacto con todos los usuarios de la cuenta y haga clic en Guardar.
4. Para que todos los contactos a los que usted envíe un Proceso para firma a partir de ahora se guarden automáticamente, habilite el botón "Guardar los destinatarios de un Proceso enviado para firma en mi lista de contactos".

El Nombre y el Correo/WhatsApp del(os) destinatario(s) será(n) guardado(s) como contacto(s) del usuario en la cuenta. Los contactos estarán vinculados a la cuenta en la que el usuario está conectado. Es decir, cuando este usuario inicie sesión en otra cuenta, los contactos serán diferentes.

_Reglas:_

No se permite registrar un contacto con el mismo Correo electrónico de un contacto ya registrado que:

\_ Sea contacto del usuario conectado a la cuenta en cuestión.

\_ Esté relacionado con otros usuarios activos de la cuenta conectada y esté siendo compartido en la cuenta.

Solo se permite registrar contactos del tipo correo electrónico con un correo válido.

No se permite registrar un contacto con el mismo Teléfono de un contacto ya registrado que:

\_ Sea contacto del usuario conectado a la cuenta en cuestión.

\_ Esté relacionado con otros usuarios activos de la cuenta conectada y esté siendo compartido en la cuenta.

Solo se permite registrar contactos de WhatsApp con un número de teléfono válido.

El campo "Compartir con todos los usuarios de la cuenta." es de llenado opcional para que el usuario informe si el contacto que está creando será compartido o no con otros usuarios de la cuenta.

Para entender mejor, [haga clic aquí](https://www.youtube.com/watch?v=b73Cu1HCaWA) y vea el video explicativo.

</details>

<details>

<summary>¿Cómo compartir un contacto guardado en la plataforma ArqSign con otros usuarios de la cuenta?</summary>

En el Menú "Mi perfil", opción "Mis contactos", seleccione el contacto.

El sistema muestra los datos del registro en modo de visualización y los respectivos botones de acción según el permiso del usuario en cuestión.

Las opciones de acción que pueden mostrarse son:

\_ Para contactos del usuario conectado en la cuenta actual: Nuevo, Editar y Cancelar.

\_ Para contactos compartidos por otros usuarios activos en la cuenta actual: Nuevo y Cancelar.

Para compartir un contacto, elija la opción "Editar", marque la opción de compartir y haga clic en Guardar.

</details>

<details>

<summary>¿Cómo eliminar un contacto guardado en la plataforma ArqSign?</summary>

En el Menú "Mi perfil", opción "Mis contactos", seleccione el contacto.

El sistema muestra los datos del registro en modo de visualización y los respectivos botones de acción según el permiso del usuario en cuestión.

Las opciones de acción que pueden mostrarse son:

\_ Para contactos del usuario conectado en la cuenta actual: Nuevo, Editar y Cancelar.

\_ Para contactos compartidos por otros usuarios activos en la cuenta actual: Nuevo y Cancelar.

Para eliminar un contacto, elija la opción "Eliminar" y confirme la eliminación.

</details>

<details>

<summary>¿Cómo editar un contacto guardado en la plataforma ArqSign?</summary>

En el Menú "Mi perfil", opción "Mis contactos", seleccione el contacto.

El sistema muestra los datos del registro en modo de visualización y los respectivos botones de acción según el permiso del usuario en cuestión.

Las opciones de acción que pueden mostrarse son:

\_ Para contactos del usuario conectado en la cuenta actual: Nuevo, Editar y Cancelar.

\_ Para contactos compartidos por otros usuarios activos en la cuenta actual: Nuevo y Cancelar.

Para editar un contacto, elija la opción "Editar", realice la edición y haga clic en Guardar.

</details>

<details>

<summary></summary>



</details>
