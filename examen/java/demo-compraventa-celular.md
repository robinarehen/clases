# Demo Compra Venta Celular
1. crear un micro de nombre `demo-compraventa-celular`, crear un nuevo reporitorio del mismo nombre en `GITHUB` y conectarlos.
2. crear los paquetes de nombre `[controller,dto, service]`.

**En el paquete `dto` crear las siguientes clases**
> Al terminar el punto 5, guardar y subir los cambios a `GITHUB`

1. `UsuarioDto` con los siguientes atributos `[codigo, nombreCompleto]`
2. `PersonaDto` con los siguientes atributos `[documento, nombreCompleto]`
3. `CelularDto` con los siguientes atributos `[marca, modelo, valor]`
4. `CompraDto` con los siguientes atributos `[numeroCompra, usuario, celular, cantidad]`
5. `VentaDto` con los siguientes atributos `[numeroVenta, usuario, persona, celular, cantidad]`

**En el paquete `service` crear las siguientes clases**
> Al terminar cada punto, guardar y subir los cambios a `GITHUB`

1. `UsuarioService` con lo siguiente
    1. crear un atributo de tipo lista de nombre `usuarios` inicializada.
    2. crear un metodo de nombre `getAll` que retorne la lista `usuarios`.
    3. crear un metodo de nombre `getByCodigo` que retorne un `UsuarioDto` buscando en la lista `usuarios` el que coincida por el parametro `codigo`.
    4. crear el metodo `createUsuario` que reciba como parametros los atributos de la clase `UsuarioDto`, crear un objeto y guardarlo en la lista `usuarios`, pero primero validar que no exista en la lista.
2. `PersonaService` con lo siguiente
    1. crear un atributo de tipo lista de nombre `personas` inicializada.
    2. crear un metodo de nombre `getAll` que retorne la lista `personas`.
    3. crear un metodo de nombre `getByDocumento` que retorne una `PersonaDto` buscando en la lista `personas` el que coincida por el parametro `documento`.
    4. crear el metodo `createPersona` que reciba como parametros los atributos de la clase `PersonaDto`, crear un objeto y guardarlo en la lista `personas`, pero primero validar que no exista en la lista.
3. `CompraService` en la cual se deben crear los metodos que me permitan crear una compra, consultar una comprar por los atributos de `[marca, modelo]` de la clase `CelularDto`, imprimir todas las compras, imprimir una compra por `numeroCompra`.
4. `VentaService` en la cual se deben crear los metodos que me permitan crear una venta, consultar una venta por los atributos de `[marca, modelo]` de la clase `CelularDto`, imprimir todas las ventas, imprimir una venta por `numeroVenta`, imprimir todas las ventas hechas a una persona consultando por `documento`.

**En el paquete `controller` crear las siguientes clases**

1. `CompraVentaController` con lo siguiente
    1. crear el metodo `main`
    2. crear 3 `[usuarios, personas, celulares, compras, ventas]`
    3. llamar a los metodos imprimir de las clase `[compras, ventas]`

