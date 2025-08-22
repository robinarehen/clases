# Demo Objetos

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
8. en la clase `FacturaController` llamar al metodo `imprimirFacturas`.
