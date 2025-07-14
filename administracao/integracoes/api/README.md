# 🟪 API

En el menú API, el cliente tiene acceso a las claves necesarias para la gestión y control de las solicitudes realizadas a través de la API de integración.

<figure><img src="../../../.gitbook/assets/image (752).png" alt=""><figcaption></figcaption></figure>

### **AppKey**

Para realizar la integración de la plataforma con otras herramientas a través de la API, se necesita una Clave de Acceso, que el usuario puede obtener haciendo clic en “Generar Clave”. La clave generada se mostrará en el campo “API AppKey”.

{% hint style="danger" %}
<mark style="color:red;">**Siempre que se genere una nueva clave de acceso, todas las integraciones realizadas utilizando la clave anterior se desconfigurarán. Sugerimos tener precaución al crear nuevas claves de acceso.**</mark>
{% endhint %}

### **SubscriptionKey**

Se trata de claves de acceso creadas para aportar más seguridad en el intercambio de información entre plataformas externas y ArqSign.

**Clave 1**: Cuando el cliente aún no tiene clave generada, el campo se presenta en blanco. Cuando el cliente ya tiene una clave generada, se mostrará la clave 1 que fue generada automáticamente por el sistema.

**Clave 2**: Igual que la clave 1, si no hay clave generada, el campo aparecerá en blanco. Si ya existe, se mostrará la clave 2 generada automáticamente.

Por defecto, el sistema generará siempre un "par" de claves, por lo que el cliente podrá utilizar una u otra, o usarlas de forma rotativa, es decir, en cada llamada, el usuario podrá usar una, o en casos donde la integración ocurre con terceros, el cliente utiliza una y el tercero usa la otra.Por **padrão** o sistema vai gerar sempre um **"par"** de **chaves**, então o cliente poderá utilizar **uma ou outra** ou **poderão ser usadas de forma rotacionada**, ou seja, a cada chamada o usuário poderá usar uma, ou ainda em casos em que a integração ocorre com terceiros, **o cliente utiliza uma e o terceiro a outra**.

Una vez que la clave es generada, debe incluirse en el HEADER de las solicitudes para que estas sean autorizadas.

Al hacer clic en "Generar Par de Claves", se muestra un mensaje en la pantalla de validación de la acción.

<figure><img src="../../../.gitbook/assets/image (753).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
<mark style="color:red;">Si después de regenerar las claves, el usuario no las actualiza en los parámetros de búsqueda de la integración ya existente, las llamadas a la API de ArqSign dejarán de funcionar.</mark>
{% endhint %}

Para **regenerar el par de claves, utilice** el botón "**Generar Par de Claves**". Para **regenerar solo una de las claves, utilice** el ícono de "**Regenerar Clave**" considerando la clave 1 o la 2.

<figure><img src="../../../.gitbook/assets/image (754).png" alt=""><figcaption></figcaption></figure>

### Cómo pasar la AppKey y la SubscriptionKey

Considerando la ruta: [https://api-rest.arqsign.com/](https://api-rest.arqsign.com/), es necesario enviar en los “Headers”, además de la “AppKey”, la “SubscriptionKey”.

<figure><img src="../../../.gitbook/assets/image (199).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

***

### Servicios de Integración ArqSign

<figure><img src="../../../.gitbook/assets/image (755).png" alt=""><figcaption></figcaption></figure>

Al hacer clic en este enlace, la aplicación abrirá la página [<mark style="color:blue;">**api.arqsign.com**</mark>](https://api.arqsign.com/index.html) con los métodos disponibles hasta el momento.

***

### Documenta**ción** API

<figure><img src="../../../.gitbook/assets/image (756).png" alt=""><figcaption></figcaption></figure>

Al hacer clic en este enlace, la aplicación abrirá la página [<mark style="color:blue;">**de detalle de la API**</mark>](../).

***

### D**escargar lista de IDs de usuarios**

<figure><img src="../../../.gitbook/assets/image (757).png" alt=""><figcaption></figcaption></figure>

Al hacer clic en este enlace, la aplicación descargará un archivo .csv con la lista de todos los usuarios activos en la cuenta y su respectivo ID.

{% hint style="success" %}
<mark style="color:green;">La búsqueda de los usuarios activos de la cuenta también puede realizarse mediante API. Para más información, acceda al detalle del método:</mark> [<mark style="color:green;">POST /api/v1/usuarios/buscar-usuarios</mark>](https://manual.arquivar.com/manual-arqsign-or-espanhol/administracao/integracoes/api/metodos-disponibles-en-la-api/3.-usuarios/3.1.post-api-v1-usuarios-buscar-usuarios)
{% endhint %}

***

### Descargar lista de IDs de carpetas

<figure><img src="../../../.gitbook/assets/image (758).png" alt=""><figcaption></figcaption></figure>

Al hacer clic en este enlace, la aplicación descargará un archivo .csv con la lista de todas las carpetas no eliminadas de la cuenta y su respectivo ID.

{% hint style="success" %}
<mark style="color:green;">La búsqueda de las carpetas no eliminadas de la cuenta también puede realizarse mediante API. Para más información, acceda al detalle del método:</mark> [<mark style="color:green;">POST /api/v1/diretorio/buscar-pastas</mark>](https://manual.arquivar.com/manual-arqsign-or-espanhol/administracao/integracoes/api/metodos-disponibles-en-la-api/2.-directorios/2.1.post-api-v1-diretorio-buscar-pastas)
{% endhint %}

## 🗪 Preguntas y Respuestas Frecuentes

<details>

<summary>¿Cómo puedo probar la API de integración de ArqSign?</summary>

Para probar la API de integración de ArqSign, puede crear una [cuenta de prueba gratuita](https://arquivar.com.br/arqsign-conta-teste-gratis/) > en nuestro sitio web y realizar pruebas a través de la herramienta Postman (no utilizar Swagger).

En su cuenta de prueba gratuita, tendrá acceso al menú "Integraciones", donde obtendrá la información necesaria para la prueba.

Ahora solo debe seguir las instrucciones de la documentación disponible haciendo [clic aquí](https://manual.arquivar.com/manual-arqsign-or-espanhol/administracao/integracoes).

</details>

<details>

<summary>¿Qué métodos están disponibles en la API de ArqSign?</summary>

La API de integración de la plataforma ArqSign está lista para que otros softwares construyan su integración con nuestra solución de firma.

Haga [clic aquí](https://manual.arquivar.com/manual-arqsign-or-espanhol/administracao/integracoes/api/metodos-disponibles-en-la-api) y consulte todos los métodos disponibles.

</details>

<details>

<summary>¿Qué es la API de integración de ArqSign?</summary>

API es la abreviatura de Application Programming Interface, o en español, Interfaz de Programación de Aplicaciones.\
Es decir, es una forma de comunicación entre sistemas que permite la integración entre ellos.

A través de la integración de sistemas es posible:

* Intercambio de información entre los sistemas integrados;
* Automatización de acciones entre los sistemas integrados.

Mediante la API de integración de ArqSign es posible integrar fácilmente la Firma Electrónica de ArqSign con las demás soluciones de su empresa.\
De esta manera, mejora la experiencia del usuario, aumenta la productividad y la seguridad, reduce riesgos operativos y tareas repetitivas, ya que muchos datos ya validados se utilizan en los procesos.

Haga [clic aquí](https://www.youtube.com/watch?v=oSHOBNiawgY\&feature=youtu.be) y vea el video explicativo.

</details>
