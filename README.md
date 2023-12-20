# Grupo2
Proyecto
INSTALACION 
MYSQL APACHE PHP CLAROLINE

NOMBRES:ARTURO RUIZ ALMANZA
        Bernardo flores castro 
        María Jesús Gómez Mamani




#INTRODUCCION
In this report, we carried out installations of fundamental services such as MySQL, HTTP server, Apache, and Claroline. The main objective is to acquire a deeper understanding of these tools by exploring their characteristics, uses, and installation processes through specific commands and programming in the Ubuntu operating system and/or similar operating systems. This detailed analysis will allow us to broaden 
En este informe, realizamos as instalaciones de servicios fundamentales como MySQL, servidor HTTP, Apache y Claroline. El objetivo principal es adquirir un conocimiento más profundo sobre estas herramientas, comprendiendo sus características, usos y los procesos de instalación mediante comandos y programación específicos en el sistema operativo Ubuntu y/o en sistemas operativos similares. Este análisis detallado nos permitirá ampliar nuestra comprensión práctica de estos servicios esenciales en el ámbito de los sistemas operativos

#MARCO TEORICO 

¿QUÉ ES EL MYSQL?
MySQL es un sistema de bases de datos de Oracle que se utiliza en todo el mundo para gestionar bases de datos. Se basa en el álgebra relacional y se utiliza principalmente para el almacenamiento de datos de diversos servicios web.

#HISTORIA Y VERSIONES DE MYSQL
La historia de MySQL comienza cuando Michael Widenius, un programador de software, buscaba una solución sencilla que permitiera dar salida a sus proyectos sin recurrir a soluciones de terceros. Al comienzo MySQL carecía de elementos considerados esenciales como la integridad referencial y transacciones pero a pesar de ello atrajo rápidamente a desarrolladores web.

Esto dió lugar a la fundación de la empresa MySQL AB (empresa fundada por David Axmark, Allan Larsson y Michael Widenius) para dar continuidad al proyecto. Posteriormente la empresa fue adquirida por Sun MicroSystems en 2008 quien vió en MySQL una solución para competir con su competidor Oracle quien, curiosamente, acabó por hacerse con la compañía en 2010.


#CARACTERÍSTICAS DE MYSQL
MySQL presenta algunas ventajas que lo hacen muy interesante para los desarrolladores. La más evidente es que trabaja con bases de datos relacionales, es decir, utiliza tablas múltiples que se interconectan entre sí para almacenar la información y organizarla correctamente.

Al ser basada en código abierto es fácilmente accesible y la inmensa mayoría de programadores que trabajan en desarrollo web han pasado usar MySQL en alguno de sus proyectos porque al estar ampliamente extendido cuenta además con una ingente comunidad que ofrece soporte a otros usuarios. Pero estas no son las únicas características como veremos a continuación:

Arquitectura Cliente y Servidor: MySQL basa su funcionamiento en un modelo cliente y servidor. Es decir, clientes y servidores se comunican entre sí de manera diferenciada para un mejor rendimiento. Cada cliente puede hacer consultas a través del sistema de registro para obtener datos, modificarlos, guardar estos cambios o establecer nuevas tablas de registros, por ejemplo.

Compatibilidad con SQL: SQL es un lenguaje generalizado dentro de la industria. Al ser un estándar MySQL ofrece plena compatibilidad por lo que si has trabajado en otro motor de bases de datos no tendrás problemas en migrar a MySQL.

Vistas: Desde la versión 5.0 de MySQL se ofrece compatibilidad para poder configurar vistas personalizadas del mismo modo que podemos hacerlo en otras bases de datos SQL. En bases de datos de gran tamaño las vistas se hacen un recurso imprescindible.

Procedimientos almacenados. MySQL posee la característica de no procesar las tablas directamente, sino que a través de procedimientos almacenados es posible incrementar la eficacia de nuestra implementación.

Desencadenantes. MySQL permite además poder automatizar ciertas tareas dentro de nuestra base de datos. En el momento que se produce un evento otro es lanzado para actualizar registros u optimizar su funcionalidad.

Transacciones. Una transacción representa la actuación de diversas operaciones en la base de datos como un dispositivo. El sistema de base de registros avala que todos los procedimientos se establezcan correctamente o ninguna de ellas. En caso por ejemplo de una falla de energía, cuando el monitor falla u ocurre algún otro inconveniente, el sistema opta por preservar la integridad de la base de datos resguardando la información.

sudo mysql_secure_installation
Este comando inicia un script que te ayuda a mejorar la seguridad de tu instalación de MySQL 
realizando varias tareas.  El script te pedirá que realices las siguientes acciones:
1.	Establecer una contraseña para el usuario root de MySQL.
2.	Eliminar usuarios anónimos.
3.	No permitir el inicio de sesión remoto para el usuario root.
4.	Eliminar la base de datos de prueba y el acceso a la misma.
5.	Recargar las tablas de privilegios para aplicar los cambios
INSTALACIÓN DE PHPMYADMIN
sudo apt-get install -y php php-tcpdf php-cgt php-pear php-mbstring libapache2-mod-php php php-common php-phpseclib php-mysql
En conjunto, estos paquetes amplían las capacidades de PHP, permitiendo la generación de PDF, comunicación segura, manipulación de cadenas multibyte, acceso a bases de datos MySQL, entre otras funciones. La combinación de estos paquetes es común en entornos de desarrollo web que utilizan PHP como lenguaje del lado del servidor.

sudo apt install phpmyadmin php-mbstring php-zip php-gd php-json php-curl
Este conjunto de paquetes es típicamente utilizado en entornos web que requieren la administración de bases de datos MySQL a través de phpMyAdmin, junto con extensiones de PHP necesarias para diversas operaciones, como manejo de cadenas, manipulación de imágenes y comunicación con servicios externos a través de HTTP.
sudo systemctl is-enabled mysql.service 
se utiliza para verificar si el servicio MySQL está habilitado para iniciarse automáticamente al arrancar el sistema
sudo systemctl start mysql.service
. Este comando te dará información detallada sobre el estado actual del servicio MySQL, incluyendo si está en ejecución y si hubo algún problema durante el inicio
sudo phpenmod mbstring
se utiliza para habilitar (activar) el módulo de PHP llamado "mbstring" en sistemas que utilizan la herramienta phpenmod para gestionar los módulos de PHP. Este módulo es esencial para manejar cadenas multibyte en PHP.
sudo systemctl restart apache2
se utiliza para reiniciar el servidor web Apache en sistemas que utilizan
 systemd para la gestión de servicios
sudo nano /etc/apache2/apache2.conf
se utiliza para reiniciar el servidor web Apache en sistemas que siguen
 la estructura de inicio tradicional de System 








VENTAJAS DE USAR MYSQL
Descritas las principales características de MySQL es fácil ver sus ventajas. MySQL es una opción razonable para ser usado en ámbito empresarial. Al estar basado en código abierto permite a pequeñas empresas y desarrolladores disponer de una solución fiable y estandarizada para sus aplicaciones. Por ejemplo, si se cuenta con un listado de clientes, una tienda online con un catálogo de productos o incluso una gran selección de contenidos multimedia disponible, MySQL ayuda a gestionarlo todo debida y ordenadamente.


¿QUÉ ES UN SERVIDOR HTTP?
Un servidor web es un software que forma parte del servidor y tiene como misión principal devolver información (páginas) cuando recibe peticiones por parte de los usuarios. En otras palabras, es el software que permite que los usuarios que quieren ver una página web en su navegador puedan hacerlo.


HISTORIA
La historia de HTTP empezó en 1989, cuando Tim Berners-Lee y su equipo del CERN (Suiza) empezaron a desarrollar la World Wide Web. La versión inicial de HTTP fue bautizada con el número de versión 0.9, consistía en una sola línea y solo permitía solicitar un archivo HTML del servidor cada vez.

CARACTERÍSTICAS DEL PROTOCOLO HTTP
LAS CARACTERÍSTICAS PRINCIPALES DEL PROTOCOLO HTTP SON:

1. CONEXIÓN ÚNICA
Desde la versión 2.0 de HTTP, este usa una conexión única para generar múltiples solicitudes y respuestas en paralelo, lo cual a la hora de procesar las solicitudes genera una eficiencia mayor en la respuesta.

2. ELIMINA LA INFORMACIÓN REDUNDANTE
Al eliminar la información redundante se busca evitar el envío de datos repetidos durante una misma conexión, así se consigue un menor consumo de recursos y, por lo tanto, se obtiene una menor latencia.

3. TIENE MULTIPLEXACIÓN
Al ser un protocolo multiplexado, puede enviar y recibir varios mensajes al mismo tiempo, optimizando la comunicación. Esta característica mejora considerablemente la velocidad de carga.

4. ES UN PROTOCOLO BINARIO
HTTP trabaja mediante tramas y al ser un protocolo binario facilita encontrar el comienzo y el final de cada frame, lo cual al ser un protocolo de texto podría llegar a ser complicado de identificar. Adicionalmente, los protocolos binarios son más simples, por lo que tienden a ser menos propensos a errores.

5. SERVICIO SERVER PUSH
Este servicio de HTTP se basa en estimaciones con las que el servir es capaz de enviar información al usuario antes de que esta sea solicitada para conseguir que la información esté disponible de forma inmediata.

6. COMPRESIÓN DE CABECERAS
En versiones anteriores, dados los requerimientos de las solicitudes, las cabeceras tenían un tamaño considerable, lo cual aumentaba el tiempo para obtener respuestas. A partir de la versión 2.0 las cabeceras empezaron a ser comprimidas para mejorar la eficiencia en la respuesta haciendo uso de un algoritmo simple y poco flexible llamado HPACK.

7. PRIORIZACIÓN DE FLUJOS
Un mensaje HTTP se puede dividir en múltiples fragmentos al ir desde el cliente hasta el servidor o viceversa y el orden en que lleguen a su destino es fundamental, es por eso que a cada flujo de le puede asignar un peso que va desde 1 hasta 256 y una dependencia. Haciendo uso de las prioridades y dependencias el protocolo crea un árbol de prioridades para los mensajes y solicitudes.

VENTAJAS DEL PROTOCOLO HTTPS:
SEGURIDAD DE DATOS: El certificado HTTPS nos permite “blindar “nuestra información enviada.
VERIFICACIÓN DE IDENTIDAD: Garantiza que la información que el usuario envía llega al destino correcto y queda registrado tal y como ha escrito el usuario.

CONFIANZA: El protocolo HTTPS aporta una confianza extra al consumidor.
Mejora el posicionamiento orgánico de la web: el sitio web aparecerá en posiciones más altas si cuenta con el certificado de seguridad HTTPS.

FAVORECE LAS VENTAS: Este protocolo ayuda a que se produzcan mayores conversiones en tu sitio web.

MEJORA LA SATISFACCIÓN DEL USUARIO: Al ganar en confianza y seguridad el usuario quedará más satisfecho con su experiencia en la web.


SERVIDOR APACHE
Apache es un servidor web que se encarga de almacenar, procesar y servir las páginas web a los usuarios de las mismas. Se distribuye bajo una licencia de código abierto, lo que quiere decir que es gratuito y fácilmente adaptable, personalizable y reutilizable.

SERVIDOR APACHE: QUÉ ES Y CUÁL ES SU IMPORTANCIA
Apache es uno de los servidores web más importantes del mundo. Es utilizado por gigantes como Netflix, Microsoft, Adobe, PayPal, LinkedIn y Facebook.

HISTORIA
Creado por el desarrollador de software estadounidense Robert McCool en 1995, es considerado una de las tecnologías que impulsó el crecimiento inicial de Internet.
Desde entonces, es ofrecido por la Apache Software Foundation, una organización sin fines de lucro que se encarga de supervisar la comunidad de usuarios que lo desarrollan y mantienen.

PRINCIPALES CARACTERÍSTICAS DE APACHE
El servidor web Apache ofrece un conjunto de funcionalidades amplio, al que se le pueden instalar diversos complementos para obtener soporte a todavía más características. Algunas de las más populares son:

MANEJO DE SOLICITUDES HTTP
El primer objetivo de Apache y los servidores web es el manejo de solicitudes HTTP. Por supuesto, es capaz de manejar este protocolo y todos los relacionados, como HTTPS, o HTTP2.

SOPORTE PARA DIFERENTES SISTEMAS OPERATIVOS
Aunque inicialmente se desarrolló para sistemas basados en Unix, Apache ofrece soporte para todos los sistemas operativos populares, incluyendo Windows, MacOS, y por supuesto Linux. En ambientes de producción lo normal es que se ejecute sobre Linux, pero el hecho de soportar Windows o MacOS permite que los profesionales puedan usar el servidor web en local, para probar y desarrollar páginas web con sus ordenadores personales.

CONFIGURACIÓN Y PERSONALIZACIÓN
Uno de los puntos fuertes de Apache es su flexibilidad y sus amplias capacidades de personalización. Para ello se utilizan archivos de configuración de los que hablaremos más adelante, en los que los administradores de sistemas pueden indicar cómo se debe de comportar el servidor web, permitiendo que esta configuración cambie según las necesidades de cada sitio web alojado.

¿QUÉ ES Y PARA QUÉ SIRVE CLAROLINE?
Claroline es una plataforma de aprendizaje y trabajo virtual (eLearning y eWorking) de código abierto y software libre (open source) que permite a los formadores construir eficaces cursos online y gestionar las actividades de aprendizaje y colaboración en la web.

HISTORIA DE CLAROLINE
El proyecto de la plataforma de Claroline se inició en el año 2000 en el Instituto Universitario de Multimedia (IPM) de la Universidad Católica de Lovaina.  Fue creado por Thomas De Praetere, Hugues Peeters y Christophe Gesché, financiado por la Fundación Louvain de la propia Universidad. Con respecto al logotipo, hace referencia al rostro de una musa griega perteneciente a la poesía épica y a la elocuencia, Calíope
El motivo de la creación de Claroline fue por una mala experiencia con una plataforma comercial. Con su desarrollo, los alumnos y profesores tenían un apoyo en su aprendizaje, partiendo de sus necesidades y basándose en sus experiencias.
En el 2004, el Centro de Investigación y Desarrollo (CERDECAM) perteneciente al Instituto Superior de Ingeniería Belga (ECAM) empezó a participar en el desarrollo de la plataforma de Claroline, gracias a un equipo que fue subvencionado por la Región Valona. Además, un grupo internacional de desarrolladores y profesores contribuyeron en el desarrollo del proyecto.




   VENTAJAS:
Claroline es una plataforma estable, abierta a todos.
 Su funcionamiento no requiere conocimientos técnicos especiales.
 Es Fácil de instalar y de usar
Es posible configurar cada sector de la plataforma, para lograr apariencias y estilos personalizados de acuerdo a las necesidades del usuario. 
 El profesor no está limitado en sus opciones educativas y dispone de herramientas que se pueden organizar y utilizar de acuerdo a sus necesidades.
Claroline es un sistema ideal para los formadores, profesores y profesionales de la educación, la cual de manera casi instantánea les va a permitir administrar sus cursos virtuales en entornos e- learning.
Claroline se utiliza no sólo en las escuelas y universidades, sino también en centros de formación, asociaciones y empresas. Es personalizable y ofrece un entorno de trabajo flexible y personalizado.

CARACTERISTICAS:
Dentro de las principales características de Claroline podemos encontrar:

Compatibilidad con SCORM Administración de usuarios, esto se traduce en la posibilidad de crear grupos y tutores de grupos
Dashboards de métricas para el análisis del proceso de aprendizaje
Admite formatos PDF, videos, HTML
Herramientas de sociabilidad como foros, chats, wikis
Exámenes, cuestionarios.
Gamificación.
  

DESARROLLO
INSTALACION DE LINUX UBUNTU

Paso 1 Descargar Ubuntu:

•	Ve al sitio web oficial de Ubuntu: https://ubuntu.com/.
•	Haz clic en la sección "Download" y selecciona la versión de Ubuntu que deseas instalar (por ejemplo, Ubuntu LTS para una versión estable a largo plazo).
•	Descarga la imagen ISO del sistema operativo.

Paso 2: Crear un medio de instalación:
Si estás utilizando una unidad USB, utiliza una herramienta como "Rufus" en Windows o "dd" en Linux para crear un medio de instalación bootable. Si estás utilizando un DVD, graba la imagen ISO en el DVD.

Paso 3: Arrancar desde el medio de instalación:
Inserta la unidad USB o el DVD en tu computadora.Reinicia la computadora y configura la BIOS/UEFI para arrancar desde el medio de instalación.

Paso 4: Iniciar el proceso de instalación:
Selecciona "Install Ubuntu" en el menú de inicio. Selecciona el idioma y haz clic en "Install Ubuntu".

Paso 5: Configurar el teclado y la ubicación:
Elige tu disposición de teclado y haz clic en "Continue". Selecciona tu ubicación y haz clic en "Continue".

Paso 6: Configurar particiones:
Selecciona el método de instalación. Puedes elegir "Erase disk and install Ubuntu" para una instalación sencilla o "Something else" para configurar las particiones manualmente. Sigue las instrucciones para configurar las particiones según tus preferencias.

Paso 7: Configurar detalles de usuario:
Completa el formulario con tu nombre, nombre de usuario, contraseña y otros detalles. Haz clic en "Continue" para iniciar la instalación.

Paso 8: Esperar a que termine la instalación:
Espera a que se complete la instalación. Una vez finalizada, se te pedirá que reinicies el sistema.

Paso 9: Reiniciar: 
Retira el medio de instalación y haz clic en "Restart Now". 

INSTALACION DE MySQL
Paso 1: Actualización del sistema:
Abre una terminal y asegúrate de que tu sistema esté actualizado antes de instalar APACHE. Ejecuta los siguientes comandos:
 Sudo apt-get update     
INSTALACION DE APACHE
Instalar Apache con "sudo apt-get install apache2" 
configura un servidor web en tu sistema, permitiéndote publicar contenido en la web.

Paso 2: Verificación del estado de Apache:
Una vez completada la instalación, Apache debería iniciarse automáticamente. Puedes verificar su estado con el siguiente comando:
sudo systemctl start apache2 
estás iniciando el servidor web Apache inmediatamente. Esto significa que Apache comenzará a aceptar y procesar solicitudes HTTP.


sudo systemctl status apache2 

Este comando te mostrará el estado actual del servicio Apache.

sudo systemctl enable apache2 

El comando sudo systemctl enable apache2 se utiliza para configurar el inicio automático del servidor web Apache en sistemas que utilizan systemd como gestor de servicios. Cuando ejecutas este comando, le estás diciendo al sistema que Apache se inicie automáticamente cada vez que se inicia el sistema operativo.

Paso 3: Instalación de MySQL: 
Este comando instalará el servidor de MySQL versión 8.0 en tu sistema
sudo apt install mysql-server-8.0

sudo systemctl start mysql.service
este comando inicia el servicio MySQL, permitiéndote utilizar y acceder a la base de datos.
Durante la instalación, se te pedirá que configures una contraseña para el usuario
Ejecuta el siguiente comando para instalar el servidor de MySQL:
 
Sudo mysql_secere_installation

Este comando inicia un script que te ayuda a mejorar la seguridad de tu instalación de MySQL realizando varias tareas. El script te pedirá que realices las siguientes acciones:
1.	Establecer una contraseña para el usuario root de MySQL.
2.	Eliminar usuarios anónimos.
3.	No permitir el inicio de sesión remoto para el usuario root.
4.	Eliminar la base de datos de prueba y el acceso a la misma.
5.	Recargar las tablas de privilegios para aplicar los cambios

sudo mysql_secure_installation
Este comando inicia un script que te ayuda a mejorar la seguridad de tu instalación de MySQL 
realizando varias tareas.  El script te pedirá que realices las siguientes acciones:
1.	Establecer una contraseña para el usuario root de MySQL.
2.	Eliminar usuarios anónimos.
3.	No permitir el inicio de sesión remoto para el usuario root.
4.	Eliminar la base de datos de prueba y el acceso a la misma.
5.	Recargar las tablas de privilegios para aplicar los cambios

INSTALACIÓN DE PHPMYADMIN

sudo apt-get install -y php php-tcpdf php-cgt php-pear php-mbstring libapache2-mod-php php php-common php-phpseclib php-mysql
En conjunto, estos paquetes amplían las capacidades de PHP, permitiendo la generación de PDF, comunicación segura, manipulación de cadenas multibyte, acceso a bases de datos MySQL, entre otras funciones. La combinación de estos paquetes es común en entornos de desarrollo web que utilizan PHP como lenguaje del lado del servidor.

sudo apt install phpmyadmin php-mbstring php-zip php-gd php-json php-curl

Este conjunto de paquetes es típicamente utilizado en entornos web que requieren la administración de bases de datos MySQL a través de phpMyAdmin, junto con extensiones de PHP necesarias para diversas operaciones, como manejo de cadenas, manipulación de imágenes y comunicación con servicios externos a través de HTTP.

sudo systemctl is-enabled mysql.service 

se utiliza para verificar si el servicio MySQL está habilitado para iniciarse automáticamente al arrancar el sistema

sudo systemctl start mysql.service

. Este comando te dará información detallada sobre el estado actual del servicio MySQL, incluyendo si está en ejecución y si hubo algún problema durante el inicio

sudo phpenmod mbstring

se utiliza para habilitar (activar) el módulo de PHP llamado "mbstring" en sistemas que utilizan la herramienta phpenmod para gestionar los módulos de PHP. Este módulo es esencial para manejar cadenas multibyte en PHP.

sudo systemctl restart apache2

se utiliza para reiniciar el servidor web Apache en sistemas que utilizan
 systemd para la gestión de servicios

sudo nano /etc/apache2/apache2.conf

se utiliza para reiniciar el servidor web Apache en sistemas que siguen
 la estructura de inicio tradicional de System 


