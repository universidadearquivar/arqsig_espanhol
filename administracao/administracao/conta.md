# 🟪 Cuenta

En el menú Cuenta se encuentran las informaciones sobre la cuenta del usuario.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

***

## **Pestaña Datos Fiscales**

En la pestaña Datos Fiscales se presentan las informaciones fiscales y financieras del usuario. Los datos proporcionados al crear una cuenta y adquirir un plan en la plataforma ArgSign se muestran en esta pantalla.

Si la cuenta del usuario es de un plan gratuito, la información estará en blanco, pero podrá ser editada haciendo clic en el botón "Editar".

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

En esta pestaña se presentan las siguientes informaciones del usuario:

* **Nombre de la cuenta:** Nombre creado para la cuenta en el momento del registro en la plataforma. Puede ser, por ejemplo, el nombre del usuario o de la empresa propietaria de la cuenta.
* **Segmento:** Segmento profesional en el que el usuario o empresa actúa.
* **Cantidad de Empleados:** Cantidad de empleados que tiene la empresa en la que actúa el usuario.
* **Tipo de Registro:** Tipo de registro de la cuenta, que puede ser CPF, CNPJ u otros.
* **Número de registro:** Número de registro de la cuenta que debe completarse de acuerdo con la opción elegida en el campo "Tipo de Registro".
* **Idioma predeterminado para nuevos usuarios:** Idioma en que se presentará la plataforma para los nuevos usuarios asociados a la cuenta, que puede ser Portugués, Inglés o Español.
* **Nombre de la aplicación:** Este dato se mostrará en el historial de las firmas de los documentos que se envíen a través de nuestra [API de Integración que tengan el parámetro “retornarLinkProcesso = 1”](https://manual.arquivar.com/manual-arqsign-or-espanhol/administracao/integracoes/api/metodos-disponibles-en-la-api/1.-proceso/1.1.post-api-v2-processo-enviar-documento-para-assinar). Este campo no altera ningún parámetro para envíos de Procesos a través de la plataforma.
* **Dirección:** Dirección residencial o comercial del usuario o empresa.
* **Número:** Número de la residencia o inmueble comercial.
* **Complemento:** Complemento de la dirección.
* **Barrio:** Barrio del usuario o empresa.
* **Código Postal:** Código postal de la dirección residencial o comercial del usuario o empresa.
* **País:** País del usuario o empresa.
* **Estado:** Estado del usuario o empresa.
* **Ciudad:** Ciudad del usuario o empresa.

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

***

## Pestaña de Facturación y Uso

En la pestaña de Facturación y Uso se presenta el historial de compras de la cuenta del usuario.

### Plan y Consumo

En la subpestaña Plan y Consumo se presenta el tipo de plan, el período de facturación (anual o mensual), la fecha de suscripción del plan y la fecha de vencimiento de la suscripción.

Por defecto, al crear una cuenta, la opción de "**Renovación Automática**" estará habilitada automáticamente. Para cancelar esta renovación, basta con desmarcar esta opción.

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">Al dejar habilitada la renovación automática, cuando el plan venza, el sistema realizará la renovación del pago de forma automática, utilizando el mismo medio de pago de la compra anterior. Si se deshabilita la opción, se mostrará el botón "Comprar Ahora", para que el usuario realice nuevamente la compra del mismo plan o de otro plan que desee.</mark>
{% endhint %}

Para cambiar la forma de pago del plan, haga clic en "**Alterar Forma de Pagamento**". Se enviará un enlace al correo electrónico o teléfono del usuario responsable de la cuenta con un enlace para que se realice esta modificación.

<figure><img src="../../.gitbook/assets/image (5) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Al hacer clic en "**Detalles del Plan**", se mostrarán los detalles del plan actual del usuario, como el tipo de plan, el período de facturación (mensual o anual), el monto pagado por el plan, la descripción y la cantidad de los elementos a los que el plan otorga acceso, los valores de créditos, los créditos excedentes y la fecha de vencimiento del plan.

<figure><img src="../../.gitbook/assets/image (6) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

En esta pantalla, también es posible visualizar la cantidad de créditos restantes que el usuario aún tiene para el envío de documentos. En "**Uso Acumulado del Plan**", el usuario puede ver la cantidad de envíos de documentos a los que tiene derecho según el plan contratado.

En "**Créditos Restantes de la Suscripción del Plan**", se presentan los créditos que el usuario aún posee en el plan firmado. El usuario puede ver la cantidad de créditos disponibles para enviar documentos a través de WhatsApp y correo electrónico, así como los códigos de seguridad por SMS.

{% hint style="warning" %}
<mark style="color:orange;">**No es posible enviar documentos por SMS. Los créditos adquiridos para el envío por SMS solo pueden ser utilizados para el envío de códigos de seguridad. El código de seguridad o token es una contraseña utilizada para acceder a los documentos enviados por correo electrónico o WhatsApp, y puede ser utilizada para añadir una capa extra de seguridad al proceso de firma electrónica de documentos.**</mark>
{% endhint %}

Si el usuario ha comprado créditos adicionales a los incluidos en el plan, al hacer clic en "**Fechas de expiración de los créditos extra**" podrá visualizar las fechas en las que los créditos comprados por separado del plan van a expirar.

<figure><img src="../../.gitbook/assets/image (7) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Cuando el plan de la firma de la cuenta sea ArqGED, ArqSign no mostrará:**</mark>

* <mark style="color:orange;">**Los campos “Renovación Automática”, "Cambiar forma de pago" y el botón "Comprar Créditos".**</mark>

<mark style="color:orange;">**La facturación de estas cuentas se realizará a través de ArqGED, de acuerdo con el servicio establecido en el contrato.**</mark>
{% endhint %}

### Historico de Compras

En la pestaña Histórico de Compras se presenta la descripción de los productos ya adquiridos por el usuario, el período de vigencia de cada uno, el número de cuotas en las que se dividió el pago, el valor y el estado de esas cuotas.

<figure><img src="../../.gitbook/assets/image (8) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Al hacer clic en "**Detalles del plan**", se presenta la descripción y cantidad detallada de los elementos que componen el plan, los valores de créditos y los valores excedentes (cuando se adquieren), así como la fecha de caducidad de cada uno de los elementos.

<figure><img src="../../.gitbook/assets/image (9) (1) (1).png" alt=""><figcaption></figcaption></figure>

***

## **Pestaña Configuraciones**

### Procesos

Por defecto, algunas configuraciones de esta pestaña se completan automáticamente, pero es posible modificarlas haciendo clic en el botón "Editar".

<figure><img src="../../.gitbook/assets/image (10) (1) (1).png" alt=""><figcaption></figcaption></figure>

Los valores definidos aquí se adoptarán como estándar para la configuración de envío y renovaciones de documentos y procesos de firma realizados por el usuario, pero pueden modificarse en cada documento durante su creación en la pantalla [<mark style="color:blue;">Nuevo Documento > Agregar Documentos y Destinatarios > Configuraciones Avanzadas</mark>](https://app.gitbook.com/o/Ai1YjbPQxIuvTaVzoZ4H/s/zDlPVk00J5AKVvFiB3dg/).

**Tiempo estándar de \_\_\_\_ días para la expiración del documento, cuando no esté firmado por uno o más destinatarios a partir de la fecha de envío:** En este campo se define el tiempo estándar (en días) que los usuarios tendrán para firmar un documento antes de que expire y se vuelva indisponible.

**Tiempo estándar de \_\_\_\_ días para aviso antes de la fecha de expiración:** En este campo se define cuántos días antes de que un documento expire los destinatarios que aún no hayan firmado el documento deberán ser notificados sobre su expiración.

**Configuración estándar para recordatorios recurrentes que se enviarán a los destinatarios después de la fecha de envío:** Al marcar esta opción, desde el momento del envío del documento hasta la fecha de su vencimiento, se enviarán recordatorios a los destinatarios cada período de tiempo determinado en el campo "Tiempo estándar de \_\_\_\_\_ días para recurrencia de recordatorio a los destinatarios sobre alguna acción pendiente en el documento". Si la opción está deshabilitada, el campo a continuación también se deshabilitará automáticamente.

**Agrupar los documentos del proceso en un archivo único:** Configuración de agrupamiento de los documentos del proceso en un archivo único. Esta opción estará, por defecto, desmarcada.

**Obligar al firmante a leer los documentos antes de firmar:** Esta configuración obliga a la lectura de los documentos del proceso. Esta opción estará, por defecto, desmarcada.

<figure><img src="../../.gitbook/assets/image (11) (1).png" alt=""><figcaption></figcaption></figure>

**Generar QR Code de acceso del documento en el Registro de Firmas:** Si esta opción está habilitada, en el Registro de Firmas de un documento firmado se presentará un QR Code, a través del cual la persona que accede podrá visualizar el documento firmado.

**Tiempo estándar de \_\_\_\_\_ días para la expiración del enlace de acceso al documento, después de la conclusión de la firma:** En este campo se define el tiempo estándar (en días) que los usuarios tendrán para acceder a un documento después de que se haya completado el proceso de firmas, hasta que expire y se vuelva indisponible.

**Adjuntar archivo menor de 10MB al correo enviado al finalizar las firmas:** Si se marca esta opción, todo documento completado cuyo archivo del proceso tenga un tamaño menor a 10MB se enviará a los destinatarios como adjunto en el correo de notificación de la conclusión del proceso de firma.

{% hint style="warning" %}
<mark style="color:orange;">**Al concluir el proceso de firmas, el sistema enviará un enlace de acceso al documento en el cuerpo del correo electrónico a todos los destinatarios.**</mark>
{% endhint %}

<figure><img src="../../.gitbook/assets/image (710).png" alt=""><figcaption></figcaption></figure>

**Configuración predeterminada para recordatorios recurrentes que se enviarán a los remitentes después de la fecha de renovación programada de un documento:** Si se marca esta opción, cuando haya un documento concluido que tenga una renovación programada, el sistema recordará al remitente del documento que está listo para ser renovado. Este recordatorio se enviará en el período definido en el campo "Tiempo estándar de \_\_\_\_ días para la recurrencia de recordatorios a los remitentes sobre la renovación del documento". Si se desactiva esta opción, este campo también se deshabilitará.

<figure><img src="../../.gitbook/assets/image (711).png" alt=""><figcaption></figcaption></figure>

### Rol del Firmante

En esta pestaña se crean los roles de los firmantes. Los roles de firmantes se presentarán al usuario en el momento de la configuración de los destinatarios/firmantes en la pantalla [<mark style="color:blue;">Nuevo Documento > Agregar Documentos y Destinatarios > Agregar Documentos > Destinatarios</mark>](https://app.gitbook.com/o/Ai1YjbPQxIuvTaVzoZ4H/s/zDlPVk00J5AKVvFiB3dg/).

{% hint style="info" %}
<mark style="color:blue;">El rol del firmante es la función que desempeña en el contrato, ya sea como parte, persona contratada o contratante, testigo, representante legal, etc.</mark>
{% endhint %}

Por defecto, la plataforma presenta los roles “Contratada”, “Contratante”, “Fiador”, “Parte” y “Testigo”.

<figure><img src="../../.gitbook/assets/image (712).png" alt=""><figcaption></figcaption></figure>

Para editar estos roles, basta seleccionar el que desea modificar y hacer clic en el ícono “Editar”.

<figure><img src="../../.gitbook/assets/image (713).png" alt=""><figcaption></figcaption></figure>

Se podrá cambiar el nombre del rol y definirlo como rol predeterminado.

{% hint style="warning" %}
<mark style="color:orange;">**El rol predeterminado es aquel que se asignará al signatario si el remitente del documento no define un rol específico para él en el momento del registro del documento. Por defecto, el sistema establece el rol "Parte" como predeterminado, pero esta elección puede ser modificada por el usuario remitente. No es obligatorio determinar un rol predeterminado, pero si es necesario, solo uno de los roles puede ser el predeterminado.**</mark>
{% endhint %}

<figure><img src="../../.gitbook/assets/image (717).png" alt=""><figcaption></figcaption></figure>

Para crear un nuevo rol, haz clic en el ícono “Agregar” e ingresa un nombre para el rol. Si deseas establecerlo como el rol predeterminado, marca la opción “Definir este rol como predeterminado”. Para finalizar, haz clic en “Guardar”.

<figure><img src="../../.gitbook/assets/image (718).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (720).png" alt="" width="409"><figcaption></figcaption></figure>

Para cambiar el rol predeterminado, haz clic en “Eliminar Predeterminado” o “Establecer como Predeterminado”, según sea necesario.

<figure><img src="../../.gitbook/assets/image (721).png" alt=""><figcaption></figcaption></figure>

Para eliminar un papel, haz clic en el ícono “Eliminar”. También es posible encontrar un tipo de papel utilizando la barra de búsqueda en la pantalla.

<figure><img src="../../.gitbook/assets/image (722).png" alt="" width="360"><figcaption></figcaption></figure>

### Notificaciones

**Notificar al alcanzar el \_\_\_\_ % de uso de los ítems de mi suscripción:** Al completar este campo, el usuario será notificado por el sistema cuando su consumo del plan alcance un cierto porcentaje. Esta configuración será deshabilitada en el plan con envíos ilimitados.

**Notificar cada \_\_\_\_\_ días, a partir de \_\_\_\_\_ días antes del vencimiento de la suscripción:** Al completar estos campos, los administradores globales de la cuenta serán notificados en el período determinado cuando la fecha de vencimiento del plan se acerque. Después del vencimiento de la suscripción, este tipo de notificación ya no se enviará.

<figure><img src="../../.gitbook/assets/image (723).png" alt=""><figcaption></figcaption></figure>

Si se habilita el campo "**Notificaciones Personalizadas - Personalización con colores y logo de la marca**", será posible insertar un banner y definir los colores de destaque de las notificaciones enviadas a los destinatarios por correo electrónico y Whatsapp.

<figure><img src="../../.gitbook/assets/image (724).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Atente-se a la dimensión estándar de la imagen para el banner. Las imágenes que no cumplan con los tamaños especificados no serán aceptadas.**</mark>

![](<../../.gitbook/assets/image (725).png>)
{% endhint %}

Al hacer clic en el ícono "Eliminar imagen", se excluirá el banner.

Al hacer clic en "Ver Notificación", será posible ver cómo se presentará al destinatario el correo electrónico de notificación y la notificación a través de WhatsApp.

<figure><img src="../../.gitbook/assets/image (726).png" alt="" width="416"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (729).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Si estos campos no son completados, el sistema enviará el banner y utilizará los colores predeterminados de la plataforma ArqSign.**</mark>
{% endhint %}

***

## Pestaña Término de Aceptación

### Término

En esta pestaña, el usuario puede insertar o editar el Término de aceptación para la Firma Electrónica que se presenta a los signatarios en el momento de firmar un documento. El objetivo de este término es asegurar que los signatarios han aceptado firmar el documento electrónicamente.

La plataforma presenta el término predeterminado, pero si el usuario desea editar o reemplazar este texto, puede hacerlo haciendo clic en "Editar".

<figure><img src="../../.gitbook/assets/image (730).png" alt=""><figcaption></figcaption></figure>

También podrá cambiar la formateación y los colores del texto utilizando la barra de herramientas de edición.

<figure><img src="../../.gitbook/assets/image (731).png" alt=""><figcaption></figcaption></figure>

Al hacer clic en "Visualizar", se muestra el Término de la forma en que será presentado a los signatarios. El usuario podrá imprimir el texto haciendo clic en "Imprimir".

<figure><img src="../../.gitbook/assets/image (732).png" alt="" width="362"><figcaption></figcaption></figure>

### Histórico de Aceite

En esta pestaña se presentan todos los Aceptes al Término de Firma Electrónica realizados por los signatarios, es decir, cada vez que un signatario acepte el Término de Aceptación que se le presenta, esta acción será registrada y podrá ser consultada en esta pantalla.

* **Fecha del Acepto:** En esta columna se presenta la fecha en que el signatario aceptó el Término de Firma Electrónica.
* **Nombre:** Nombre del signatario que realizó el acepto.
* **Correo Electrónico/Teléfono:** Contacto del signatario a través del cual recibió el enlace para acceder al documento para la firma y realizó el acepto.
* **Versión del Término:** Esta columna muestra la versión del Término de Firma Electrónica aceptada por el usuario. Cada vez que el Término es editado o sustituido, el sistema le asigna una nueva versión.
* **IP:** Esta columna presenta la IP de la máquina utilizada por el signatario en el momento del acepto del Término de Firma Electrónica.
* **Geolocalización:** Esta columna presenta la geolocalización de la máquina del signatario en el momento en que realizó el acepto al Término de Firma Electrónica.
* **Visualizar Término:** Al hacer clic en este botón, se muestra la versión del término que fue aceptada por el signatario.

<figure><img src="../../.gitbook/assets/image (733).png" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (734).png" alt="" width="454"><figcaption></figcaption></figure>

## 🗪 Preguntas y Respuestas Frecuentes

<details>

<summary>¿Cómo personalizar la plataforma ArqSign con los colores y logotipo del cliente?</summary>

En la plataforma ArqSign, las notificaciones (correos electrónicos y mensajes de WhatsApp) para los remitentes y destinatarios pueden tener los siguientes diseños:

1. Diseño Predeterminado de la Plataforma ArqSign o
2. Diseño con sus colores y logotipo.

Los ítems disponibles para personalización son:

* Encabezado
* Color del texto superior
* Color del botón del correo electrónico o mensaje de WhatsApp

Para personalizar las notificaciones de la Plataforma ArqSign, el Administrador de la cuenta debe acceder a: Administración > Cuenta > Configuraciones > Otros y seguir los siguientes pasos:

1. En la esquina inferior derecha haga clic en editar;
2. En "Notificaciones Personalizadas", cambie a Activado;
3. En "Notificaciones por Correo Electrónico", realice los siguientes pasos:
   * inserte una imagen para el encabezado de los mensajes con las dimensiones indicadas en el campo;
   * elija el color destacado para el texto del correo electrónico.
4. En "Notificaciones por WhatsApp", realice el siguiente paso:
   * inserte una imagen para el encabezado de los mensajes con las dimensiones indicadas en el campo.
5. Si desea visualizar las notificaciones con los cambios que realizó, haga clic en "Visualizar Notificación";
6. Cuando todos los ajustes estén correctos, haga clic en "Guardar".

<div align="left"><figure><img src="../../.gitbook/assets/image (851).png" alt="" width="125"><figcaption></figcaption></figure></div>

Notificación predeterminada:

<div align="left"><figure><img src="../../.gitbook/assets/image (852).png" alt="" width="348"><figcaption></figcaption></figure></div>

Ejemplo de notificación personalizada simulación:

<div align="left"><figure><img src="../../.gitbook/assets/image (853).png" alt="" width="188"><figcaption></figcaption></figure></div>

</details>

<details>

<summary>¿Cómo cambiar la tarjeta de crédito para facturación y compras en la plataforma ArqSign?</summary>

Puede cambiar su tarjeta de crédito para facturación y compras en la Plataforma ArqSign siguiendo los siguientes pasos:

1. Vaya al menú "Administración";
2. Haga clic en "Cuenta";
3. Haga clic en "Facturación y Uso";
4. Haga clic en "Cambiar la forma de pago".

</details>

<details>

<summary>¿Cómo personalizar las configuraciones para Proceso de Firma, Disponibilidad del enlace para documento firmado, recordatorios y notificaciones de la plataforma?</summary>

Puede personalizar las configuraciones predeterminadas y, si lo necesita, ajustar recordatorios y notificaciones durante la creación de sus Procesos.

Para personalizar las configuraciones predeterminadas siga el paso a paso:

1. Acceda al menú Administración > Cuenta > Configuraciones;
2. Haga clic en Editar;
3. Realice los ajustes según su necesidad;
4. Haga clic en Guardar.

**Entienda en detalle cada uno de los ítems personalizables:**

* Configuraciones sobre el Proceso de firma.

- Tiempo predeterminado en días para la expiración del Proceso a partir de la fecha de envío.
- Tiempo predeterminado en días para aviso antes de la expiración.
- Habilitar, deshabilitar y definir periodicidad de recordatorios para firma a los firmantes pendientes.

* Configuraciones de disponibilidad del enlace para el documento firmado.

- Configure el tiempo predeterminado para la expiración del enlace de acceso al documento después de la firma.
- Habilite o deshabilite la opción de adjuntar archivo menor de 20 MB al correo electrónico enviado al finalizar las firmas.

* Configuraciones sobre recordatorios para vencimiento, renovación, reajuste:

- Configure la recurrencia de recordatorios para vencimiento, renovación, reajuste de documentos y Procesos.

* En Otros, configure notificaciones relacionadas con la cuenta:

- Notificación para porcentaje de uso de los ítems de la cuenta.
- Notificación para recordatorio de vencimiento de la suscripción.

</details>

<details>

<summary>¿Cómo habilitar y deshabilitar la renovación automática del plan?</summary>

Durante la vigencia del plan, el cliente puede habilitar o deshabilitar la renovación automática del mismo. Para ello, acceda a:\
[Administración > Cuenta > Facturación y Uso > Renovación Automática.](https://manual.arquivar.com/manual-arqsign-or-espanhol/administracao/administracao/conta#pestana-de-facturacion-y-uso)

</details>

<details>

<summary>¿Cómo verificar el plan, vencimiento, renovación automática y consumo?</summary>

Acceda al menú [Administración > Cuenta > Facturación y Uso.](https://manual.arquivar.com/manual-arqsign-or-espanhol/administracao/administracao/conta#pestana-de-facturacion-y-uso)

Consulte el plan contratado, el período del plan, la fecha de suscripción, la fecha de vencimiento, la renovación automática, los ítems consumidos y disponibles, el período de renovación y el Historial de compras.

</details>

<details>

<summary>¿Cómo personalizar el Término de Aceptación para firma electrónica?</summary>

La funcionalidad Término de Aceptación para firma electrónica formaliza y registra el historial de aceptación de los firmantes para firmar en formato electrónico, lo cual es un requisito legal previo para la validez jurídica de la firma. Puede utilizar nuestra sugerencia de Término de Aceptación o personalizar el suyo. Para personalizar, siga los siguientes pasos:

1. Haga clic en [Administración > Cuenta > Término de Aceptación](https://manual.arquivar.com/manual-arqsign-or-espanhol/administracao/administracao/conta#pestana-termino-de-aceptacion);
2. Haga clic en editar y personalice su término;
3. Haga clic en publicar.

[Haga clic aquí](https://www.youtube.com/watch?v=MBJB6RW7y7E\&feature=youtu.be) y vea el paso a paso.

</details>
