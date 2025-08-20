# Clases
En este repositorio quedaran reflejadas los temas y tareas para aprender `GIT` y `Java - Spring Boot`


# git
	https://es.wikipedia.org/wiki/Git
	https://es.wikipedia.org/wiki/GitHub
	https://es.wikipedia.org/wiki/GitLab
	https://es.wikipedia.org/wiki/Bitbucket
	https://git-scm.com/
	https://www.udemy.com/course/git-y-github-desde-cero-a-experto/
	https://commitizen-tools.github.io/commitizen/

### Temas
1. Explicar que es git
2. Instalacion y configuración de git, user.name y user.email
3. Primeros comandos: init, status, add, commit
4. Ramas
5. Github
6. conectar repositorio local con el global
7. comandos push y pull
8. comando merge

### Tarea 
1. crear una carpeta de nombre `repo-prueba-20240609`
2. convertir la carpeta en un repositorio de git
3. crear 2 archivos de texto con los siguientes nombre `[prueba-1, prueba-2]`
4. en el archivo de nombre `prueba-1` agrega el siguiente texto `hola mundo`
5. en el archivo de nombre `prueba-2` agrega el siguiente texto `hola mundo, archivo hecho por Andres o Angeles`
6. guardar los cambios con los comando aprendidos.

### Tarea
> todos los archivos que se creen, guardarlos con los comandos aprendidos
1. crear un carpeta de nombre `taller-20250813` dentro de la carpeta `git`
2. convertir la carpeta en un repositorio de git y crear un nuevo archivo de nombre `prueba-en-master`.
3. crear una rama con el nombre  `develop` desde la rama `master`
4. crear un nuevo archivo en la rama `develop` de nombre `prueba-en-develop`.
5. crear una rama con el nombre  `feature/copia-develop` desde la rama `develop`
6. crear un nuevo archivo en la rama `feature/copia-develop` de nombre `prueba-en-feature-develop`.
7. crear una rama con el nombre  `feature/copia-master` desde la rama `master`
8. crear un nuevo archivo en la rama `feature/copia-master` de nombre `prueba-en-feature-master`.
9. unir las ramas `feature` a `develop`
10. crear un repositorio en `github` de nombre `taller-20250813` y conectarlo con el repositorio local, del punto 1
11. subir las ramas `master` y `develop`
12. crear un `pull request` de `develop` a `master`


# Micro servicios
[microservicios-spring-boot](https://www.qindel.com/que-son-los-microservicios-spring-boot/#:~:text=%C2%BFQu%C3%A9%20son%20los%20microservicios%20Spring,de%20realizar%20una%20tarea%20espec%C3%ADfica.)

	Programacion Orientada a Objetos con Java
	Bajar Aplicativos
		sts
		Java
		Maven
	Instalacion de Aplicativos y configurar variables de entorno
	Configurar Java Jdk en sts
	Conocer STS, proyectos, paquetes, clases, navegar, abrir y cerrar 
	Definición de clase

### Atributos
[Tipos de datos](https://www.manualweb.net/java/tipos-datos-primitivos-java/)

    Variables en el metodo main
    Que valores se deben pasar a los atributos y variables segun el tipo de dato

### Tarea - 2025-08-18
1. crea un proyecto de nombre `demo-objetos`
    1. crear los paquetes `[controller, dto, service]`
2. crear las clases `[PersonaDto, ProductoDto, FacturaDto]`
    1. en la clase `PersonaDto` crear los atributos `[tipoDoc, numeroDoc, nombreCompleto]`
    2. en la clase `ProductoDto` crear los atributos `[nombre, cantidad, valor]`
    3. en la clase `FacturaDto` crear los atributos `[persona, productos]`
3. crear la clase `PersonaService`
    1. crear una lista del tipo `PersonaDto` de nombre `personas`
    2. crar el constructor vacio `(que no reciba parametros)` y dentro inicializar la lista `personas`
    3. crear el metodo `crearPersona` que reciba como parametros los atributos de la clase `PersonaDto`, dentro del metodo crear un objeto de la clase `PersonaDto` pasar los parametros recibidos y agregar el objeto creado a la lista `personas`
    4. crear el metodo `consultarPersonas` que retorne la lista `personas`
    5. crear el metodo `consultarPersona` que reciba el parametro `numeroDocumento`, recora la lista `persona` para buscar y retornar el objeto `persona` que coincida con el parametro `numeroDocumento`
4. crear la clase `ProductoService`
    1. crear una lista del tipo `ProductoDto` de nombre `productos`
    2. crar el constructor vacio y dentro inicializar la lista `produtos`
    3. crear el metodo `crearProducto` que reciba como parametros los atributos de la clase `ProductoDto`, dentro del metodo crear un objeto de la clase `ProductoDto` pasar los parametros recibidos y agregar el objeto creado a la lista `productos`
    4. crear el metodo `consultarProductos` que retorne la lista `productos`
    5. crear el metodo `consultarProducto` que reciba el parametro `nombreProducto`, recora la lista `prodctos` para buscar y retornar el objeto `producto` que coincida con el parametro `nombreProducto`
5. crear la clase `FacturaService`
    1. crear una lista del tipo `FacturaDto` de nombre `faturas`
    2. crar el constructor vacio y dentro inicializar la lista `faturas`
    3. crear el metodo `crearFactura` que reciba como parametros un objeto `PersonaDto` y una lista de `ProductoDto`, dentro del metodo crear un objeto de la clase `FacturaDto` pasar los parametros recibidos y agregar el objeto creado a la lista `faturas`
6. crea la clase `FacturaController`
    1. crear el método `main`
    2. crear un objeto de `PersonaService` y llamar al metodo `crearPersona` 3 veces con datos diferentes
    3. crear un objeto de `ProductoService` y llamar al metodo `crearProducto` 3 veces con datos diferentes
    4. crear un objeto `FacturaService` y llamar al metodo `crearFactura`, pasar un objeto `PersondaDto` consultando uno de los creados previamente y la lista de `ProductoDto`
7. en la clase `FacturaService` crear un metodo `imprimirFacturas` que recorra la lista `faturas` e imprima en la consola, los atributos de `PersonaDto`, recorrer la lista de `Productos` e imprimir los atributos de cada objeto `ProductoDto`, dentro de cada objeto `FacturaDto`.

### Tarea
1. crear un micro de nombre `demo-taller-20250814`
