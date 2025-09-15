# Demo Micro DB
1. Se debe crear un micro de nombre `demo-micro-db` y conectarlo con un repositorio del mismo nombre en `github`.
2. Crear los siguientes paquetes `[controller, dto, service, entity, repository]`
3. Crear las siguientes clases en el paquete `dto`:
    * `PersonaDto` con los siguientes atributos `[id, tipoDocumento, documento, nombres, apellidos]`
    * `CentroTrabajoDto` con los siguientes atributos `[id, codigo, nombreCentro, direccion, codigoPostal]`
    * `UsuarioDto` con los siguientes atributos `[persona, centroTrabajo, codigoUsuario]`
    * `ClienteDto` con los siguientes atributos `[persona, email, celular]`
4. Crear las siguientes clases en el paquete `entity`:
    * `PersonaEntity` con los siguientes atributos `[id, tipoDocumento, documento, nombres, apellidos]`
    * `CentroTrabajoEntity` con los siguientes atributos `[id, codigo, nombreCentro, direccion, codigoPostal]`
5. Crear las siguientes clases en el paquete `service`
    * `PersonaService` con los siguientes metodos:
      * `consultarPersonas` que retorne una lista del tipo `PersonaDto`.
      * `consultarPersonaByDocumento` que retorne un objeto `PersonaDto` y reciba como parametro `[tipoDocumento, documento]`.
      * `crearPersona` que retorne un objeto `PersonaDto` y que reciba como parametro un objeto `PersonaDto`.
      * `actualizarPersona` que retorne un `PersonaDto` y que reciba como parametro `[id, persona]`.
      * `deletePersonaByDocumento` que reciba como parametro `[tipoDocumento, documento]`
6. Crear las siguientes clases en el paquete `controller`
    * `PersonaController` con los siguientes metodos:
    
