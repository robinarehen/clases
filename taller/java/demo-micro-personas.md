# Micro Servicio Personas
1. Crear un proyecto de nombre `demo-micro-personas`
    1. crear los siguentes paquetes `[controller, dto, service]`

**Crear las siguientes clases**
1. `PersonaDto` con los siguientes atributos `[tipoDocumento, documento, nombre, apellidos]`
2. `PersonaService` con lo siguiente
    1. crear un atributo del tipo lista de `PersonaDto` de nombre `personas` inicializado
    2. crear un método de nombre `crearPersona` que reciba como parametro un objeto `PersonaDto`
       el cual se debe agregar a la lista `personas`
    3. crear un método que retorne la lista `personas` de nombre `consultarPersonas`
    4. crear un método que retorne una `PersonaDto` buscando en la lista `personas` de nombre `consultarPersonaPorTipoDocumentoYDocumento`
3. `PersonaController` y hacer lo siguientes
    1. crear un atributo de la clase `PersonaService` inicializado
    2. crear los mismo metodos de la clase `PersonaService` y dentro de cada método llamar al método de la clase `PersonaService` con el atributo
    3. agregar las anotaciones para que poder llamar el controller desde **Postman**
