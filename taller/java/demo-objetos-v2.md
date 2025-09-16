# Demo Objetos Version 2
1. Crear un proyecto de nombre `demo-objetos-v2` y conectarlo con `github` en un repositorio del mismo nombre.
2. Crear los paquetes `[controller, dto, service]`
3. En el paquete `dto`, crear lo siguiente:
    * El atributo `persona` debe ser del tipo `PersonaDto` y el atributo `centroTrabajo` debe ser del tipo `CentroTrabajoDto`.
    * Una clase de nombre `PersonaDto` con los atributos `[tipoDocumento, documento, nombres, apellidos]`.
    * Una clase de nombre `ClienteDto` con los atributos `[persona, email, celular]`.
    * Una clase de nombre `CentroTrabajoDto` con los atributos `[codigo, nombre, codigoPostal, dirreccion]`.
    * Una clase de nombre `UsuarioDto` con los atributos `[persona, codigoUsuario, centroTrabajo]`.
4. En el paquete `service`, crear una clase de cada una de las clases que hay en el paquete `dto` y cambiar la terminación `Dto` por `Service`
5. Crear las siguientes clases en el paquete `service`
    * `PersonaService` con atributo del tipo lista `PersonaDto` inicializada y crear los siguientes metodos:
      * `consultarPersonas` que retorne una lista del tipo `PersonaDto`.
      * `consultarPersonaByDocumento` que retorne un objeto `PersonaDto` y reciba como parametro `[tipoDocumento, documento]`.
      * `crearPersona` que retorne y reciba como parametro un objeto `PersonaDto` el cual se debe agregar a la lista, pero primero se debe validar que no exista.
      * `eliminarPersonaByDocumento` que reciba como parametro `[tipoDocumento, documento]`
6. Crear las siguientes clases en el paquete `controller`
    * `PersonaController` y crear el método `main`
      * Crear un objeto de `PersonaDto` y llenar los atributos
      * Crear un objeto de `PersonaService` y con el objeto llamar al metodo `crearPersona` y pasar el objeto `PersonaDto`
      * Con el objeto `PersonaService` llamar al metodo `crearPersona` 3 veces más y pasar un objeto `PersonaDto` sin crear un objeto previo.
