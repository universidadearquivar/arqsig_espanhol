# 💻 Visión General de la Plataforma 2.6.0

## Características de la plataforma

ArqSign es una plataforma para firmas electrónicas que funciona de la siguiente manera: el usuario carga el documento, elige los signatarios, establece las firmas y realiza el envío a los involucrados en el proceso de firma.

El usuario puede acceder a los documentos enviados y recibidos para firma en cualquier momento, desde cualquier lugar, en cualquier dispositivo – celular, computadora, tableta – sin perder la seguridad y la encriptación de los datos, conforme a la Ley General de Protección de Datos (LGPD).

ArqSign cuenta con la implementación de una API (Interfaz de Programación de Aplicaciones), lo que permite que el usuario integre su Firma Electrónica y Digital de Documentos con las soluciones de su empresa.

La funcionalidad principal de la plataforma ArqSign es ofrecer a los usuarios la posibilidad de enviar, gestionar, recopilar y firmar documentos digitalmente, mediante firmas electrónicas o certificados digitales.

El signatario puede firmar los documentos a través de correo electrónico, WhatsApp o su cuenta ArqSign, si tiene una.

{% hint style="info" %}
<mark style="color:blue;">**FIRMA ELECTRÓNICA VS. FIRMA DIGITAL (ICP Brasil y otros certificados digitales)**</mark>

<mark style="color:blue;">La firma electrónica es aquella que no requiere un certificado digital. Se utiliza principalmente para firmar contratos y documentos entre entidades privadas (B2B, B2C).</mark>

<mark style="color:blue;">La firma digital es aquella que requiere un certificado digital. Se usa principalmente para la emisión de facturas y para transacciones con el gobierno.</mark>

<mark style="color:blue;">En la plataforma ArqSign, al configurar un flujo de firmas, puede determinar qué tipo de firma debe ser ejecutada por el destinatario, eligiendo entre:</mark>

<mark style="color:blue;">a)</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Firma electrónica**</mark><mark style="color:blue;">: ArqSign genera firmas electrónicas avanzadas con validez jurídica de acuerdo con la MP 2.200-2 del 24/08/2001 y la Ley 14.063 del 23/11/2020. Siempre que un signatario firma un documento de forma electrónica, ArqSign aplica un certificado digital propio de la plataforma, capturando el</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Hash**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">(identificación única) del archivo, verificando la integridad del archivo y anexando al certificado la identificación del signatario.</mark>

<mark style="color:blue;">b)</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Firma digital – ICP-Brasil o ICP Otros**</mark><mark style="color:blue;">: ArqSign genera firmas digitales calificadas de acuerdo con la MP 2.200-2 del 24/08/2001 y la Ley 14.063 del 23/11/2020. Cuando el usuario ya tiene un certificado digital y desea usarlo para realizar la firma a través de ArqSign, este certificado se utiliza para verificar la integridad de la firma e identificar al usuario como signatario en el documento.</mark>
{% endhint %}

***

### Usuario y Signatario

Usuario es la persona que utiliza la Plataforma ArqSign para enviar, acompañar el flujo, recopilar firmas, acceder y gestionar documentos. Un usuario debe estar vinculado a una cuenta o, cuando también debe firmar un documento, se convierte en un signatario.

En la plataforma ArqSign, un usuario puede tener los siguientes perfiles:

* **Remitente de Documentos:** Usuario sin permiso de acceso a las funcionalidades de gestión de la plataforma. Su acceso está enfocado en el envío y gestión de sus documentos.
* **Administrador Global:** Usuarios con permiso de acceso a todas las funcionalidades de la plataforma, incluida la gestión de carpetas y usuarios.

Signatario es una persona física o jurídica que participa en el proceso de firma (firma un documento). El signatario no necesita tener una cuenta o usuario en la Plataforma ArqSign para firmar un documento.

***

### Sitio web de la plataforma ArqSign

El sitio de ArqSign ([https://arquivar.com.br/arqsign/](https://arquivar.com.br/arqsign/)) presenta toda la información y funcionalidades de la plataforma, además de las características de los planes de suscripción. En la página principal, el usuario también tendrá acceso a la página de inicio de sesión de la plataforma y a la creación de una cuenta de prueba gratuita.

<figure><img src=".gitbook/assets/Animação (2).gif" alt=""><figcaption></figcaption></figure>

***

### Soporte técnico y atención al cliente

Para solicitar soporte o atención, en el menú inferior de la página, haga clic en “Apoyo”.

<figure><img src=".gitbook/assets/Screenshot_6 (1).png" alt=""><figcaption></figcaption></figure>

El usuario será dirigido a la Central de Ayuda de la plataforma, donde podrá buscar entre los contenidos publicados la solución a su duda o solicitar contacto con el equipo de atención.

<figure><img src=".gitbook/assets/Screenshot_7 (2).png" alt=""><figcaption></figcaption></figure>

El contacto con el equipo de atención podrá hacerse a través de WhatsApp, chat, correo electrónico (faleconosco@arqsign.com) o teléfono (4003-8839).

<figure><img src=".gitbook/assets/image (470).png" alt=""><figcaption></figcaption></figure>

Después de autenticado, el usuario también podrá contar con el menú de soporte en la plataforma, ubicado en la esquina inferior derecha de la pantalla.

<figure><img src=".gitbook/assets/image (772).png" alt=""><figcaption></figcaption></figure>

***

## Características de los planes de suscripción

### Plan gratuito

La cuenta de prueba gratuita de la Plataforma ArqSign ofrece al usuario casi todas las funcionalidades y recursos de la cuenta paga, incluyendo el envío de documentos para firma con o sin certificado digital, creación de carpetas dedicadas para la gestión de documentos, importación de certificado digital ICP-Brasil A1 e integración con otros sistemas. Durante un período de 15 días, el usuario podrá realizar cinco envíos de documentos para firma de forma gratuita.

{% hint style="warning" %}
<mark style="color:orange;">**En la cuenta de prueba gratuita no está permitida la inclusión de otros usuarios, es decir, solo el propietario puede acceder y gestionar los documentos enviados y recibidos para firma.**</mark>

<mark style="color:orange;">**La creación de una cuenta de prueba gratuita está permitida para cualquier usuario que no tenga un correo electrónico registrado en otras pruebas gratuitas de la plataforma ArqSign.**</mark>
{% endhint %}

#### Creación de Cuenta de Prueba Gratuita

1\. Para crear una cuenta de prueba gratuita, en la página inicial del sitio de la plataforma ArqSign, haga clic en "Prueba Gratuita".

<figure><img src=".gitbook/assets/image (181).png" alt=""><figcaption></figcaption></figure>

2\. El usuario será redirigido a la página de inicio de sesión, donde deberá ingresar su correo electrónico y hacer clic en "Continuar".

<figure><img src=".gitbook/assets/image (182).png" alt=""><figcaption></figcaption></figure>

3\. Luego, deberá ingresar los datos solicitados:

* **Nombre completo:** Ingrese el nombre completo.
* **Teléfono:** Número de teléfono con código de área.
* **Segmento:** Seleccione el segmento en el que la empresa o el profesional dueño de la cuenta trabaja.
* **Estoy probando ArqSign para:** Seleccione el objetivo de la prueba que se realizará en la plataforma ArqSign.
*   **Contraseña:** Cree una contraseña cumpliendo con los requisitos mínimos de seguridad (mínimo de ocho caracteres, incluyendo al menos una letra mayúscula, una letra minúscula, un número y un carácter especial).

    <figure><img src=".gitbook/assets/image (183).png" alt=""><figcaption></figcaption></figure>

4\. Para concluir, haga clic en "Comenzar mi Prueba Gratuita". Se mostrará un mensaje de confirmación de creación de cuenta. Para acceder a la plataforma, haga clic en el enlace indicado.

<figure><img src=".gitbook/assets/image (184).png" alt=""><figcaption></figcaption></figure>

5\. El usuario recibirá dos correos electrónicos de la plataforma. El primero presentará instrucciones sobre el uso de la prueba gratuita.

<figure><img src=".gitbook/assets/image (471).png" alt=""><figcaption></figcaption></figure>

6\. En el segundo correo electrónico, el usuario recibirá el enlace para la activación de la cuenta, en el cual deberá hacer clic para realizar el primer acceso.

<figure><img src=".gitbook/assets/image (180).png" alt=""><figcaption></figcaption></figure>

7\. El usuario será dirigido a la pantalla de inicio de sesión, en la cual deberá ingresar la contraseña creada anteriormente, en el momento del registro, y hacer clic en "Ingresar" para realizar el primer acceso.

<figure><img src=".gitbook/assets/image (188).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Al término del período de 30 días de prueba o después de consumir los diez envíos gratuitos, el usuario podrá seguir accediendo a la plataforma normalmente, pero para realizar nuevos envíos deberá adquirir un plan pago (para realizar nuevos envíos por correo electrónico) o comprar créditos extras (para envíos vía WhatsApp y SMS).**</mark>
{% endhint %}

***

### Planes pagos

Al contratar un plan ArqSign, tendrá acceso a un número de envíos de acuerdo con cada plan. Los envíos incluidos en el plan pueden realizarse por correo electrónico o WhatsApp.

Para el envío de flujos vía WhatsApp, es necesario que la cuenta tenga disponibilidad de envíos y créditos para WhatsApp, ya que en este caso, el envío del flujo se realiza a través de una integración con WhatsApp Oficial. Para contratar créditos de WhatsApp, después de autenticarse en la plataforma, acceda al menú "Comprar Créditos". El cobro será por envío de mensaje. En el envío de un flujo, se utilizan dos mensajes por signatario (uno para enviar el documento para firma y otro para enviar el documento firmado al final del proceso).

Para el envío de flujos vía correo electrónico, es necesario que la cuenta tenga disponibilidad de envíos, ya que la propia Plataforma ArqSign ejecuta el envío del flujo. Si los envíos incluidos en el plan del usuario se agotan, también podrá adquirir créditos extra de envío por correo electrónico accediendo al menú "Comprar Créditos" después de autenticarse en la plataforma.

Todos los planes pagos cuentan con las mismas funcionalidades. La única diferencia está en el número de envíos de cada paquete y la disponibilidad entre planes anuales y mensuales.

#### Cobro de los planes pagos

La base de cobro de cada plan es el servicio de envío de un flujo para firma. Un envío de flujo puede contener varios archivos y firmas y, aun así, solo se descontará un envío del plan.

Para los planes mensuales, usted paga una mensualidad al contratar el plan y ya comienza a utilizar la herramienta. Mensualmente, el mismo día de la compra, se facturará automáticamente la mensualidad en la misma tarjeta, a menos que desactive la renovación automática.

Para los planes anuales hay opción de adquisición en hasta 12 cuotas sin interés en la tarjeta.

#### Comprar un plan

1. Para adquirir un plan, en la página inicial del sitio de ArqSign, haga clic en "Planes y Precios" en el menú superior.

<figure><img src=".gitbook/assets/image (190).png" alt=""><figcaption></figcaption></figure>

2.  Se presentarán las características y precios de cada uno de los planes. Haga clic en "Comenzar Ahora" en el plan que desea adquirir.

    <figure><img src=".gitbook/assets/image (191).png" alt=""><figcaption></figcaption></figure>

3\. El usuario será dirigido a la página de finalización de compra, donde se presentará la información sobre el plan elegido. Deberá ingresar los datos de facturación y pago, y hacer clic en "Finalizar la compra".

<figure><img src=".gitbook/assets/image (178).png" alt=""><figcaption></figcaption></figure>

4\. Después de realizar el pago, el usuario recibirá por correo electrónico el enlace para la activación de la cuenta, en el cual deberá hacer clic para realizar el primer acceso.

***

## Página de inicio de sesión (autenticación) en la plataforma ArqSign

La página de inicio de sesión de la plataforma ArqSign solicita el correo electrónico y la contraseña registrados por el usuario al crear su cuenta.

Si aún no tiene una cuenta, debe hacer clic en el enlace "Regístrese aquí".

<figure><img src=".gitbook/assets/image (179).png" alt=""><figcaption></figcaption></figure>

Se le ofrecerá al usuario la [<mark style="color:blue;">creación de una cuenta de prueba gratuita</mark>](./#plan-gratuito). Para crear esta cuenta, deberá proporcionar su correo electrónico y hacer clic en “Siguiente”.

### Olividé mi contraseña

Si el usuario olvida su contraseña, simplemente debe hacer clic en “Olvidé mi contraseña”.

<div data-full-width="true"><figure><img src=".gitbook/assets/image (472).png" alt="" width="375"><figcaption></figcaption></figure></div>

En la pantalla de recuperación de contraseña, el usuario deberá proporcionar el mismo correo electrónico utilizado para acceder a la plataforma y hacer clic en “Recuperar”.

<figure><img src=".gitbook/assets/image (473).png" alt=""><figcaption></figcaption></figure>

El usuario recibirá por correo electrónico un enlace en el que deberá hacer clic para establecer una nueva contraseña.

<figure><img src=".gitbook/assets/image (474).png" alt=""><figcaption></figcaption></figure>

***

## Página inicio - Usuario con sesión iniciada

Al acceder a su cuenta, la pantalla de inicio del usuario mostrará en el menú superior los siguientes botones:

**Nuevo Documento:** Al hacer clic en este botón, el usuario podrá registrar un documento que será enviado a los firmantes para su firma.

**Firma por Lote:** Al hacer clic en este botón, el usuario podrá visualizar y firmar en lote todos los documentos que ha recibido y que están pendientes de firma.

**Vencidos:** Al hacer clic en este botón, el usuario podrá visualizar todos los documentos que envió a otras personas para su firma, pero que no fueron firmados dentro del plazo y expiraron. Aquí podrá reenviar dichos documentos.

**Comprar Ahora / Cambiar Plan:** Los botones "Comprar Ahora" o "Cambiar Plan" se mostrarán a los usuarios que tienen una cuenta de prueba gratuita o a los usuarios que tienen un plan pago que ha expirado o está próximo a expirar. El botón "Comprar Ahora" aparecerá para los usuarios con la suscripción del plan vencida. El botón "Cambiar Plan" se mostrará a los usuarios con una suscripción de plan pago cuyo vencimiento está próximo (30 días antes de la expiración de planes anuales y 10 días antes de la expiración de planes mensuales).

**Comprar Créditos:** En cuentas con el plan vigente se mostrará el botón "Comprar Créditos", donde el usuario podrá adquirir créditos para enviar documentos por correo electrónico, WhatsApp y SMS, de acuerdo con el tipo de plan de la cuenta.

**Perfil del usuario:** Al hacer clic en este menú, el usuario tendrá acceso a la información de su cuenta.

**Idiomas:** La página de inicio y la interfaz de la plataforma se presentarán en el idioma seleccionado por el usuario al momento de registrarse. Para cambiar el idioma, haga clic en el ícono de la bandera ubicado en la esquina superior derecha de la pantalla y elija entre Portugués (Brasil), Español e Inglés.

**Salir:** Utilizado para cerrar la sesión en la plataforma.

<figure><img src=".gitbook/assets/image (475).png" alt=""><figcaption></figcaption></figure>

A la izquierda de la pantalla se encuentran todos los menús disponibles, organizados por grupos. Es importante destacar que estos menús se presentarán según el nivel de permiso de cada usuario.

**Buzón de Correos:** En este grupo se concentran los menús relacionados con el proceso de tramitación de documentos.

**Directorios:** En este grupo se encuentra el menú de Documentos. Se considera un repositorio de almacenamiento de los documentos tramitados por la plataforma, es decir, aquí se encuentran todos los documentos con el proceso de firma completado.

**Administración:** En este grupo se encuentran las configuraciones de cuenta, usuarios y grupo de usuarios.

<figure><img src=".gitbook/assets/image (476).png" alt=""><figcaption></figcaption></figure>

En la esquina inferior derecha de la pantalla, el usuario encontrará el menú de **Apoyo**, donde podrá acceder al tutorial demostrativo de cómo enviar y firmar un documento, acceder a las **Preguntas Frecuentes** sobre el uso de la plataforma, aprender a verificar la validez jurídica de un documento y acceder a los contenidos sobre las novedades de la Plataforma.

<figure><img src=".gitbook/assets/image (773).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (479).png" alt=""><figcaption></figcaption></figure>
