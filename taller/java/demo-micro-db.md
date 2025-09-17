# Demo Micro DB
1. Se debe crear un micro de nombre `demo-micro-db` y conectarlo con un repositorio del mismo nombre en `github`.
2. Crear los siguientes paquetes `[controller, dto, service, entity, repository]`
3. Crear las siguientes clases en el paquete `dto`:
    * `PersonaDto` con los siguientes atributos `[id, tipoDocumento, documento, nombres, apellidos]`
    * `CentroTrabajoDto` con los siguientes atributos `[id, codigo, nombreCentro, direccion, codigoPostal]`
    * `UsuarioDto` con los siguientes atributos `[personaDto, centroTrabajoDto, codigoUsuario]`
    * `ClienteDto` con los siguientes atributos `[personaDto, email, celular]`
4. Crear las siguientes clases en el paquete `entity`:
    * `PersonaEntity` con los siguientes atributos `[id, tipoDocumento, documento, nombres, apellidos]`
    * `CentroTrabajoEntity` con los siguientes atributos `[id, codigo, nombreCentro, direccion, codigoPostal]`
5. Crear las siguientes clases en el paquete `service`
    * `PersonaService` con los siguientes metodos:
      * `consultarPersonas` que retorne una lista del tipo `PersonaDto`.
      * `consultarPersonaByDocumento` que retorne un objeto `PersonaDto` y reciba como parametro `[tipoDocumento, documento]`.
      * `crearPersona` que retorne y reciba como parametro un objeto `PersonaDto`, dentro crear un objeto `PersonaEntity` y llenar los atributos con los atributos del parametro `PersonaDto` a lo cual se le llama mapear objetos.
      * `actualizarPersona` que retorne un objeto `PersonaDto` y que reciba como parametro `[id, personaDto]`, dentro crear un objeto `PersonaEntity` y llenar los atributos con los atributos del parametro `PersonaDto`.
      * `eliminarPersonaByDocumento` que reciba como parametro `[tipoDocumento, documento]`
6. Crear las siguientes clases en el paquete `controller`
    * `PersonaController` con un atributo del tipo `PersonaService` y crear los mismo metodos de la clase `PersonaService`, dentro de cada metodo de la clase `PersonaController` llamar los metodos de la clase `PersonaService`.
      * agregar las anotaciones necesarias para acceder al controlador desde **Postman** mediante los verbos HTTP
    
