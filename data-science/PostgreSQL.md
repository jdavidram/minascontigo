# PostgreSQL

Configurar PostgreSQL en Ubuntu puede parecer un reto difícil, pero con el proceso adecuado, es un procedimiento claro y rápido. Saber instalar y ajustar esta herramienta es fundamental para trabajar eficientemente con bases de datos en entornos Linux, ampliamente utilizados en la industria.

## ¿Qué comandos se necesitan para la instalación de PostgreSQL?

Para instalar PostgreSQL, ejecuta el comando básico:

> sudo apt install postgresql

En ocasiones puede presentarse un error por permisos, para solucionarlo escribe:

> sudo !!

Luego, acepta la instalación escribiendo "Sí" cuando lo solicite.

## ¿Cómo configurar PostgreSQL luego de la instalación?

Primero, verifica la versión instalada ingresando a la carpeta específica en terminal:

> cd /etc/postgresql/14/main

El archivo clave para configurar es postgresql.conf, ábrelo con:

> sudo nano postgresql.conf

Busca el parámetro listen_addresses, procede a cambiar localhost por un asterisco (*) para aceptar conexiones desde cualquier dirección. Guarda los cambios usando Control+X y luego Y.

Después, crea un usuario con contraseña cifrada desde la terminal del servidor PostgreSQL, para ello se debe correr el siguiente comando:

> sudo -u postgresql psql |**Template**|

Luego dentro de la terminal de Postgres, se escribe:

> ALTER USER postgres WITH ENCRYPTED PASSWORD 'tuPassword';

Finalizado esto, verifica la IP de tu servidor con:

> ifconfig

Edita ahora el archivo pg_hba.conf para habilitar la conexión SSL:

> sudo nano pg_hba.conf

Agrega estas líneas al final con la información correspondiente:

> *hostssl **Template** postgres tu_dirección_IP sha256*

Para desarrollar o aprender desde diferentes redes utiliza la configuración:

> *hostssl **Template** postgres 0.0.0.0/0 sha256*

Finalmente, reinicia el servidor PostgreSQL para aplicar toda la configuración:

> sudo systemctl restart postgresql.service

## ¿Cómo comprobar el funcionamiento y conectarte?

Verifica que todo esté activo y funcionando adecuadamente con:

> sudo service postgresql status

Instala la herramienta cliente con este comando:

> sudo apt install postgresql-client

Para conectarte, escribe lo siguiente en la terminal:

> psql --host tu_dirección_IP --username postgres --password --dbname **Template**

Después de introducir tu contraseña encriptada, podrás consultar bases de datos y tablas.

---

Crear tablas en una base de datos es esencial para almacenar información de forma estructurada, clara y eficiente. Mediante PGAdmin, podemos elaborar estas tablas visualmente, simplificando así el manejo de bases de datos y optimizando nuestro trabajo con datos.

## ¿Cómo comenzar a crear tablas con PGAdmin?

Para empezar a crear tablas, abre PGAdmin y selecciona la base de datos que previamente creaste. Expande la categoría de esquemas, luego abre la opción "public" y posteriormente da clic derecho en la sección tablas. Selecciona la opción crear tabla y utiliza el asistente visual para configurar fácilmente cada elemento que contengan tus tablas.

## ¿Qué elementos debo configurar al crear una tabla nueva?

Al utilizar el asistente visual de PGAdmin, debes considerar los siguientes elementos clave:

Nombre: Define claramente el nombre que llevará tu tabla para identificar fácilmente su propósito.

Propietario y esquema: Asegúrate de asignar los valores correctos según los permisos y organización de tu base de datos.

Columnas y tipos de datos: Decide cuidadosamente qué columnas tendrá tu tabla y selecciona el tipo de datos adecuado para cada una. Recuerda, cambiar el tipo de datos posteriormente es complicado.

## ¿Qué tipos de datos puedo seleccionar para las columnas?

PGAdmin ofrece variedad de tipos de datos que puedes escoger según cómo planees usar la información. Entre estos están:

Char o arreglo de caracteres: Para almacenar letras individuales o grupos pequeños de caracteres.

Texto como arreglo: Ideal para almacenar cadenas extensas como nombres completos o descripciones.

Bit y Booleano: Guardan información binaria de forma básica (0 o 1) o como true/false respectivamente.

Entero: Perfecto para campos numéricos que funcionen como identificadores (por ejemplo, ID).

Date: Almacena fechas; revisa detenidamente si tu información necesita precisar día, mes y año.

En PostgreSQL, los tipos de dato más comunes son:

* Integer: Almacena números enteros.

* Serial: Entero auto-incremental, útil para llaves primarias.

* Bigint: Números enteros grandes.

* Boolean: Verdadero o falso (true/false).

* Character(n): Cadena de texto de longitud fija.

* Varchar(n): Cadena de texto de longitud variable.

* Text: Texto sin límite de longitud.

* Date: Fecha (año, mes, día).

* Timestamp: Fecha y hora.

* Array: Colección de elementos del mismo tipo.

Cada tipo de dato tiene características específicas que afectan cómo se almacenan y manipulan los datos en la base de datos.

## ¿Qué debo saber sobre las llaves primarias y nulidad?

Cuando defines campos, puedes seleccionar una llave primaria si necesitas identificar de manera única cada registro almacenado:

Asegúrate de activar la opción primary key en el campo que elijas como identificador único, por ejemplo, un campo "ID".

Recuerda evitar que los campos con llave primaria acepten valores nulos para mantener la integridad de tu base.

## ¿Cuándo usar la herramienta de consultas SQL en lugar del asistente visual?

PGAdmin ofrece dos vías para crear tablas: con el asistente visual o escribiendo directamente sentencias SQL:

Ambas opciones cumplen la misma función y lograrás exactamente el mismo objetivo.
Selecciona la alternativa con la que te sientas más cómodo según tu nivel de experiencia o preferencia al trabajar.

Utiliza esta información para construir y optimizar tus tablas en tu proyecto de base de datos y continúa aprendiendo mediante la práctica constante. ¿Ya has probado ambas opciones en PGAdmin? Comparte cuál prefieres y por qué.
