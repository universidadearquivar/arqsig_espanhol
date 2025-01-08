# 🟪 Seguridad

Arquivar tiene más de treinta y un años de experiencia en la prestación de servicios de gestión de documentos, procesos e información, cumpliendo con la legislación brasileña y con las normas del Consejo Nacional de Archivos (CONARQ).

Nuestras soluciones atienden a más de 2.500 clientes y 20.000 usuarios.

A partir de este know-how, Arquivar desarrolló ArqSign, una plataforma que permite la firma electrónica y digital de documentos, en total conformidad con la legislación brasileña, por lo que tiene 100% de validez jurídica.

<details>

<summary>¿Este tipo de servicio ya está homologado por la LGPD?</summary>

El objetivo de ArqSign es proteger los derechos de sus clientes, asegurando la total seguridad de sus datos. Toda la información recopilada o procesada por ArqSign sigue estrictamente las disposiciones legales de la Ley General de Protección de Datos (LGPD).

</details>

<details>

<summary>¿Cómo queda un documento firmado a través de la Plataforma ArqSign?</summary>

En el Panel de Firmas de Adobe Reader es posible verificar:&#x20;

1. A Arquivar como certificadora del proceso de firma, al inicio de la ruta de firma;
2. Un certificado digital que identifica cada acción de firma (en el ejemplo a continuación, tenemos 2 firmantes).&#x20;
3. A Arquivar finalizando el flujo de firma y bloqueando el archivo para imposibilitar cambios.&#x20;

![](<../.gitbook/assets/image (1) (1) (1).png>)

![](<../.gitbook/assets/image (335).png>)

</details>

<details>

<summary>¿Qué tipo de criptografía se utiliza en la Plataforma ArqSign?</summary>

Para garantizar la seguridad de los datos que se transmiten entre el Cliente y el Servidor, los [<mark style="color:blue;">datos son cifrados</mark>](https://arquivar.com.br/politica-de-privacidade/) mediante un certificado SSL de SHA256.

Utilizamos criptografía en las comunicaciones y en los procesos de operación, siguiendo protocolos de transporte estándar de la industria entre los dispositivos del usuario y los centros de datos de Microsoft Azure, así como dentro de los propios centros de datos.

Para datos en reposo, nuestro servidor en Azure ofrece una amplia gama de recursos de cifrado, incluyendo AES-256.

* **Protección de redes:** infraestructura necesaria para conectar máquinas virtuales de manera segura entre sí y para conectar centros de datos locales con las VMs de Azure. Azure bloquea el tráfico no autorizado hacia los centros de datos de Microsoft o dentro de ellos, utilizando diversas tecnologías. La Red Virtual de Azure se extiende a su red local hacia la nube a través de una VPN de sitio a sitio.
* **Gestión de amenazas:** Microsoft Antimalware para servicios en la nube y máquinas virtuales. Microsoft también emplea detección de intrusiones, prevención de ataques DDoS (ataques de denegación de servicio distribuido), pruebas de penetración regulares y herramientas de análisis de datos y aprendizaje automático para ayudar a mitigar las amenazas contra la plataforma Azure.

</details>

<details>

<summary>¿Dónde se almacenan los datos y documentos ingresados en la Plataforma ArqSign?</summary>

Los datos y documentos se almacenan en el datacenter de Microsoft Azure, líder mundial en establecer requisitos de privacidad y seguridad.&#x20;

Microsoft Azure cumple con una amplia variedad de normas de conformidad internacionales y específicas del sector, como el GDPR (Reglamento General de Protección de Datos), ISO 27001, HIPAA, FedRAMP, SOC 1 y SOC 2, así como normas específicas de ciertos países, incluyendo IRAP de Australia, G-Cloud del Reino Unido y MTCS de Singapur. Rigurosas auditorías de terceros, como las realizadas por el British Standards Institute, confirman la adhesión de Azure a los estrictos controles de seguridad exigidos por tales normas.

Microsoft ha aprovechado su experiencia en la creación de protecciones de software empresarial y en la ejecución de algunos de los mayores servicios en línea del mundo para crear tecnologías y prácticas de seguridad robustas. Estas ayudan a garantizar que la infraestructura de Azure sea resistente a ataques, protegen el acceso del usuario al entorno de Azure y ayudan a mantener los datos del cliente seguros mediante comunicaciones cifradas y gestión de amenazas y prácticas de mitigación, que incluyen pruebas de penetración regulares. Haz clic aquí para ver el video explicativo.

[<mark style="color:blue;">Haz clic aquí</mark>](https://www.youtube.com/watch?v=yKNeahEQY8g) para ver el video explicativo.

</details>

<details>

<summary>¿Cuál es la base de normas que sirve de referencia para el proceso de firma de la Plataforma ArqSign?</summary>

La plataforma ArqSign se basa en los [<mark style="color:blue;">**REQUISITOS DE LAS POLÍTICAS DE FIRMA DIGITAL EN ICP-BRASIL**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">del ITI (Instituto Nacional de Tecnología de la Información).</mark> ](https://chrome-extension/efaidnbmnnnibpcajpcglclefindmkaj/https://www.gov.br/iti/pt-br/central-de-conteudo/doc-icp-15-03-requisitos-minimos-para-politicas-de-assinatura-pdf)

Este documento establece los requisitos que deben ser obligatoriamente observados por las entidades creadoras de Políticas de Firma Digital en el ámbito de la Infraestructura de Claves Públicas Brasileña (ICP-Brasil), en conformidad con la estructura propuesta por los estándares **ETSI TR 102 272** y **ETSI TR 102.038**.

</details>

<details>

<summary>¿Cuál es la diferencia entre la firma de ArqSign y la firma de otras plataformas del mercado?</summary>

¡ArqSign garantiza que el archivo firmado por todos los participantes del flujo siempre sea el mismo mediante su exclusivo proceso de firma!&#x20;

Cada vez que un signatario firma un documento sin su propio Certificado Digital, ArqSign aplica un Certificado Digital de la plataforma, capturando el _Hash_ (identificación única) del archivo, verifica la integridad del archivo y adjunta al Certificado la identificación del signatario.&#x20;

Cuando el usuario ya posee un certificado digital y desea utilizarlo para realizar la firma a través de ArqSign, usamos este certificado para verificar la integridad e identificarlo como signatario en el documento.

Aplicar un certificado digital al documento para cada acto de firma es el único medio posible para asegurar el nivel de seguridad de la firma avanzada o cualificada descrita en la Ley nº 14.063, de 23 de septiembre de 2020.

</details>

<details>

<summary>¿Cuáles son los elementos de autenticación disponibles en la plataforma?</summary>

ArqSign garantiza una amplia variedad de tecnologías de autenticación, entre las cuales se encuentran:

* Certificados digitales ICP-Brasil o de estándar internacional;
* Nombre(s) del/los signatario(s);
* Documentos de registro del signatario (CPF, CNPJ u otro);
* Direcciones de correo electrónico;
* Dirección(es) IP del/de los signatario(s);
* Captura de geolocalización del signatario (si está habilitada en el dispositivo);
* Término de aceptación para firma electrónica;
* Código de acceso;
* Cuenta ArqSign;
* Representación visual de la firma;
* Fecha y hora de la firma;
* Historial de movimientos (es decir, quién envió, visualizó, firmó, etc.);
* Historial de autenticación;
* Estado de finalización.

</details>
