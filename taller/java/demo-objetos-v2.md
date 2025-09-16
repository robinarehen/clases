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
    * `PersonaService` con los siguientes metodos:
      * `consultarPersonas` que retorne una lista del tipo `PersonaDto`.
      * `consultarPersonaByDocumento` que retorne un objeto `PersonaDto` y reciba como parametro `[tipoDocumento, documento]`.
      * `crearPersona` que retorne y reciba como parametro un objeto `PersonaDto`.
      * `actualizarPersona` que retorne y reciba como parametro un objeto `PersonaDto`.
      * `eliminarPersonaByDocumento` que reciba como parametro `[tipoDocumento, documento]`
6. Crear las siguientes clases en el paquete `controller`
    * `PersonaController`.
