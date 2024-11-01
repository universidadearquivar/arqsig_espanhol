# 🖊️ Firma en Lote

El proceso de firma en lote permite que el usuario firme más de un documento a la vez. La firma en lote solo está disponible para usuarios que tienen una cuenta registrada en la plataforma y están autenticados. En esta pantalla, se presentarán hasta 100 documentos por página, dependiendo de la cantidad de documentos pendientes de firma.

{% hint style="danger" %}
<mark style="color:red;">Documentos que requieren configuraciones:</mark>

<mark style="color:red;">•</mark> <mark style="color:red;"></mark><mark style="color:red;">**Código de seguridad**</mark>

<mark style="color:red;">**• Obligación de lectura de los documentos**</mark>

<mark style="color:red;">**• Estilo de firma predefinido**</mark>

<mark style="color:red;">**• Relleno o validación de los datos de firma**</mark>

<mark style="color:red;">**• Solicitud para adjuntar documentos**</mark>

<mark style="color:red;">No se listan para firma en lote. Para firmarlos, el usuario deberá acceder a su</mark> [<mark style="color:red;">Bandeja de Entrada</mark>](../caixa-postal/caixa-de-entrada.md) <mark style="color:red;">y firmarlos individualmente.</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (561).png" alt=""><figcaption></figcaption></figure>

## Columnas de la pantalla principal – Firma en Lote

<figure><img src="../.gitbook/assets/image (562).png" alt=""><figcaption></figcaption></figure>

**Columna Nombre del Documento:** En esta columna se muestra el nombre del documento.&#x20;

**Columna Responsable:** En esta columna se presentan el nombre y el correo electrónico de quien envió el documento (remitente).

**Columna Tipo de Firma:** En esta columna se muestra el tipo de firma requerida para la firma del documento, que puede ser [<mark style="color:blue;">Firma Electrónica</mark>](assinatura-de-documentos.md#a.-assinatura-eletronica) o [<mark style="color:blue;">Firma mediante Certificado Digital – ICP Brasil u Otros Certificados Digitales.</mark>](assinatura-de-documentos.md#a.-assinatura-eletronica)

**Columna Acciones:** Esta columna muestra botones de acción sobre el documento. Siempre se mostrará en este botón la acción prioritaria de ejecución, de acuerdo con el perfil del usuario y el estado del documento.

**Barra de Filtro:** Es posible localizar uno o más documentos utilizando los filtros disponibles para la búsqueda. En la pantalla Firma en Lote, la búsqueda se puede realizar por el nombre del documento, por el nombre del responsable o por el tipo de firma que deberá ser utilizada.

<figure><img src="../.gitbook/assets/image (563).png" alt=""><figcaption></figcaption></figure>

## Firmando documentos en lote. 

1\. En la lista de documentos pendientes, selecciona aquellos que deseas firmar y haz clic en el ícono “Firma en Lote”.

<figure><img src="../.gitbook/assets/image (564).png" alt=""><figcaption></figcaption></figure>

2\. Se presentará la pantalla de "Datos de la Firma". Complete los datos solicitados y haga clic en "Avanzar". El símbolo \* indica que la información es de llenado obligatorio.

{% hint style="warning" %}
<mark style="color:orange;">**En esta pantalla, se solicitarán todas las informaciones definidas como necesarias para la firma de todos los documentos seleccionados en la lista.**</mark>
{% endhint %}

{% hint style="info" %}
<mark style="color:blue;">**EJEMPLO:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Si en un documento se ha definido que la firma es de persona física, en esta pantalla se solicitará el CPF del firmante; si en otro documento se ha definido que la firma es de persona jurídica, también se solicitará el CNPJ, y así sucesivamente, hasta que se cumplan todos los requisitos obligatorios.</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (107).png" alt=""><figcaption></figcaption></figure>

3\. El siguiente paso será definir el [<mark style="color:blue;">Estilo de Firma</mark>](novo-documento.md#b.-destinatarios), que puede ser un estilo predeterminado, un diseño o una imagen. Una vez elegido, haz clic en "Concluir".

<figure><img src="../.gitbook/assets/image (567).png" alt=""><figcaption></figcaption></figure>

4\. Si se determina el uso de un certificado digital, puedes utilizar un certificado almacenado en la Plataforma ArqSign o uno que no esté almacenado en la plataforma. Para la firma mediante un certificado que no esté almacenado, si aún no lo has hecho, se solicitará al usuario que instale la extensión "ArqSign Certificado Digital" en el navegador y el aplicativo AppNative - Módulo Desktop en su equipo, necesarios para el uso de certificados digitales.

Después de instalados, se mostrarán todos los certificados digitales instalados en la máquina y aquellos alojados en la cuenta de ArqSign para que el usuario elija cuál desea utilizar para la firma e introduzca el código PIN (si es solicitado).

<details>

<summary>Instalación de los complementos necesarios para la utilización de los certificados digitales.</summary>

Caso ainda não tenha feito, ao assinar um documento pela primeira vez utilizando um certificado digital será solicitado ao usuário que instale os plugins “ArqSign Certificado Digital” (disponível [clicando aqui](https://chrome.google.com/webstore/detail/arqsign-certificado-digit/fjdnpmenmpfadeojgkhgiogiclmcjgbp?hl=pt-br)) e AppNative – Módulo Desktop (disponibilizado durante o processo).

<img src="../.gitbook/assets/image (568).png" alt="" data-size="original">

1\. Al hacer clic en "Instalar Ahora", se abrirá una ventana con el enlace para descargar el complemento "ArqSign Certificado Digital".

![](<../.gitbook/assets/image (569).png>)

2\. Instale la extensión de acuerdo con el navegador que esté utilizando.&#x20;

![](<../.gitbook/assets/image (570).png>)![](<../.gitbook/assets/image (571).png>)

3\. Después de completar la primera instalación, regrese a la plataforma ArqSign y continúe con la instalación de la aplicación AppNative haciendo clic en "Haga clic aquí para descargar...".

![](<../.gitbook/assets/image (572).png>)

4\. Después de completar la segunda instalación, regrese a la plataforma ArqSign. Se mostrará un mensaje confirmando la finalización de las instalaciones.

![](<../.gitbook/assets/image (573).png>)

</details>

<figure><img src="../.gitbook/assets/image (108).png" alt=""><figcaption></figcaption></figure>

5\. Se mostrará un informativo del proceso de firma y un contador de firmas completadas. De esta forma, el usuario podrá seguir el progreso de las firmas hasta que todas hayan sido completadas.

{% hint style="info" %}
<mark style="color:blue;">De acuerdo con la cantidad de documentos enviados en lote, el usuario podrá dejar la aplicación ArqSign funcionando en segundo plano y continuar con sus actividades rutinarias. No es necesario seguir el proceso de ejecución de las firmas hasta su finalización, pero es obligatorio mantener la sesión iniciada.</mark>
{% endhint %}

6\. Finalizada la firma del lote, se presenta un mensaje de conclusión al usuario. Haga clic en "Cerrar" para finalizar. La lista de documentos pendientes de firma se actualizará mostrando solo los documentos que deberán ser enviados nuevamente a los firmantes.

{% hint style="warning" %}
<mark style="color:orange;">**En caso de que ocurran fallas durante el proceso de firma en uno o más documentos seleccionados en el lote, la plataforma concluirá la firma de los documentos que estén en el estándar, informará sobre los que fueron firmados y las fallas encontradas, y mantendrá como pendientes los documentos en los que no fue posible concluir la firma.**</mark>
{% endhint %}

{% hint style="info" %}
<mark style="color:blue;">**EJEMPLO:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Algunos de los motivos para posibles fallas son más de un usuario firmando el documento al mismo tiempo, caída de conexión a Internet en el momento de la firma, acceso interrumpido, entre otros.</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (109).png" alt=""><figcaption></figcaption></figure>

## Acciones individuales – Firma en Lote

<figure><img src="../.gitbook/assets/image (110).png" alt=""><figcaption></figcaption></figure>

#### Estado

Al hacer clic en este botón, se muestra el estado en el que se encuentra ese documento, que puede ser "Esperando" (ningún participante ha firmado el documento hasta el momento) o "En proceso" (uno o más participantes ya han firmado el documento, pero aún faltan firmas). Además del estado, se muestran las siguientes informaciones sobre los firmantes: orden de firma determinada, nombre y correo electrónico/teléfono, y si ya ha completado o no la firma.

<figure><img src="../.gitbook/assets/image (111).png" alt=""><figcaption></figcaption></figure>

#### **R**ecusar Firma

Se utiliza cuando por algún motivo el firmante no desea firmar el documento. En este caso, debe ingresar una justificación para la negativa y hacer clic en “Recusar Firma”.

<figure><img src="../.gitbook/assets/image (112).png" alt=""><figcaption></figcaption></figure>
