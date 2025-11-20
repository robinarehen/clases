# Examen Compra Venta de Autos

En todos los micros se debe crear el `CRUD`, implementar `[ResponseEntity, Interfaz]` y tambien se debe crear el metodo buscar por el `campo unico` de cada micro.

> En el DTO se debe eliminar el atributo ID

## Micro Autos
crear un micro de nombre `demo-micro-autos` del cual se deben guardar en la base de datos los siguientes datos:

1. marca: no puede ser nulo
2. modelo: no puede ser nulo
3. año de matriculacion: no puede ser nulo
4. matricula: debe ser unico y no puede ser nulo

## Micro Clientes
crear un micro de nombre `demo-micro-cliente` del cual se deben guardar en la base de datos los siguientes datos:

1. nombres: no puede ser nulo
2. primer apellido: no puede sr nulo
3. segundo apellido
3. codigo cliente: debe ser unico y no puede ser nulo

## Micro Vendedores
crear un micro de nombre `demo-micro-vendedores` del cual se deben guardar en la base de datos los siguientes datos:

1. nombres: no puede ser nulo
2. primer apellido: no puede sr nulo
3. segundo apellido
3. codigo Vendedor: debe ser unico y no puede ser nulo

## Micro Compra Venta de Coche
crear un micro de nombre `demo-micro-compraventa-coches`, en el cual la meta es conectar con los micros anteriores, para confirmar que el cliente, el vendedor y el auto existen previamente antes de registrar la venta.

  > Crear el CRUD y todas las clases e interfaces que se necesitan.

1. Se debe crear los paquetes `[controller, dto, entity, repository, service]`
2. En el paquete `entity` se debe crear la clase `CompraVentaCocheEntity`, la cual debe tener los siguientes atributos, los cuales **no deben ser nulo**.
    * 2.1 codigo Vendedor
    * 2.2 codigo Cliente
    * 2.3 matricula
    * 2.4 tipo transaccion: solo debe tener dos valores `[compra o venta]`
    * 2.5 fecha transaccion
3. Dentro el paquete `service` se debe crear un nuevo paquete de nombre `external` en el cual vamos a crear la consulta a los micros `[auto, vendedor, cliente]`.