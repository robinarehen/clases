# Demo Objetos Version 2
1. Crear un proyecto de nombre `demo-objetos-v2` y conectarlo con `github` en un repositorio del mismo nombre.
2. Crear los paquetes `[controller, dto, service]`
3. En el paquete `dto`, crear lo siguiente:
    * Los atributos `persona` debe ser del tipo `PersonaDto`, `centroTrabajo` debe ser del tipo `CentroTrabajoDto`.
    * Una clase de nombre `PersonaDto` con los atributos `[tipoDocumento, documento, nombres, apellidos]`.
    * Una clase de nombre `ClienteDto` con los atributos `[persona, email, celular]`.
    * Una clase de nombre `CentroTrabajoDto` con los atributos `[codigo, nombre, codigoPostal, dirreccion]`.
    * Una clase de nombre `UsuarioDto` con los atributos `[persona, codigoUsuario, centroTrabajo]`.
