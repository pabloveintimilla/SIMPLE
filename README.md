#SIMPLE - Sistema de Implementación de Procesos Ligeramente Estandarizados


### Resumen
SIMPLE (Sistema para la Implementación de Procesos Ligeramente Estandarizados) corresponde a un sistema para la implementación de procesos electrónicos mediante un diseñador simplificado, desarrollado para entregar una solución flexible a instituciones públicas que deseen digitalizar sus trámites de forma amigable, rápida y sencilla.

### Licencia
Este software esta licenciado bajo la licencia BSD-3.

### Roadmap
https://trello.com/b/jlq22yiU/minsegpres-simple

### Ambiente de Ejecución
Los usuarios deben ingresar mediante ambiente web, a través de la URL provista por el organismo.

### Plataforma, Framework o Lenguaje de Programación / BBDD
PHP, HTML, Javascript, CSS, MySQL  
Codeigniter 2.1.0  
Twitter Bootstrap 2.3.1  
jQuery 1.7.2  

### Requisitos Técnicos
- Apache 2.x con modulo mod_rewrite instalado y activado.
- PHP >= 5.4.x
- MySQL >= 5.5.x

### Configuración de la plataforma
#### Framework
- Cambiar el nombre del archivo de configuración del framework que se encuentra dentro de la carpeta "application/config" de "config.php.sample" a "config.php"
- Setear el parametro encryption_key dentro del archivo config.php. Utiliza cualquier string aleatorio.
- Cambiar el nombre del archivo de configuración del envío de correos que se encuentra dentro de la carpeta "application/config" de "email.php.sample" a "email.php"
#### Base de datos
- Crear una base de datos para la plataforma
- Cargar la estructura inicial del archivo "sql/estructura.sql"
- Cambiar el nombre del archivo de configuración de base de datos que se encuentra dentro de la carpeta "application/config" de "database.php.sample" a "database.php"
- Editar el archivo "database.php" y actualizar los valores con los de su configuración, normalmente se deben editar sólo los campos "username, password, database"
- Para versiones de Mysql 5.6.x o superior cambiar en el archivo de configuracion (my.cnf) el parametro sql-mode=""
#### Aplicación de parches
- Aplicar los últimos parches a base de datos situandose en la raiz de la aplicación y ejecutando el comando: php index.php migration migrate
#### Carga de datos iniciales
- Cargar los datos iniciales del archivo "sql/datos.sql"

### Ejecución inicial
- Acceder a http://nombrededominio/backend
    Usuario: admin@admin.com
    Contraseña: 123456

### Administración de multiples cuentas:
- Acceder a http://nombrededominio/manager
    Usuario: admin@admin.com
    Contraseña: 123456

### Acerca de
La primera versión de SIMPLE fue creada por la Unidad de Modernización y Gobierno digital del Ministerio de Secretaría General de Presidencia, de Chile. Actualmente está siendo adaptado y enriquecido por varios países de la región en el marco del proyecto de Red Gealc "Mecanismo colaborativo regional de software público", que cuenta con el apoyo de la Iniciativa de Bienes Públicos Regionales del BID.
