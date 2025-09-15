# Demo Micro DB
1. Se debe crear un micro de nombre `demo-micro-db` y conectarlo con un repositorio del mismo nombre en `github`.
2. Crear los siguientes paquetes `[controller, dto, service, entity, repository]`
3. Crear las siguientes clases en el paquete `dto`:
    * `PersonaDto` con los siguientes atributos `[tipoDocumento, documento, nombres, apellidos]`
    * `CentroTrabajoDto` con los siguientes atributos `[codigo, nombreCentro, direccion, codigoPostal]`
    * `UsuarioDto` con los siguientes atributos `[persona, centroTrabajo, codigoUsuario]`
    * `ClienteDto` con los siguientes atributos `[persona, email, celular]`
4. Crear las siguientes clases en el paquete `entity`:
    * `PersonaEntity` con los siguientes atributos `[tipoDocumento, documento, nombres, apellidos]`
    * `CentroTrabajoEntity` con los siguientes atributos `[codigo, nombreCentro, direccion, codigoPostal]`
5. Crear las siguientes clases en el paquete `service`
    
