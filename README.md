# Sistema de Gestión de Inventario y Compras

## Descripción

Este proyecto consiste en una serie de funciones que gestionan el inventario de una tienda y permiten realizar diversas operaciones como agregar productos, visualizar el inventario, buscar productos, actualizar el stock, eliminar productos, calcular el valor total del inventario y realizar compras. Además, incluye funcionalidades para gestionar clientes y registrar sus compras.

## Funciones Principales

### `agregar_producto(nombre, precio, cantidad)`
- Agrega un nuevo producto al inventario o actualiza su cantidad si ya existe.
- Compara el nombre del producto con los existentes en el inventario.
- Si el producto ya existe, actualiza la cantidad. Si no, lo agrega.

### `ver_inventario()`
- Muestra todos los productos en el inventario junto con sus detalles (nombre, precio, cantidad).
- Utiliza un bucle para iterar sobre cada producto y mostrar su información.

### `buscar_producto(nombre)`
- Busca un producto por su nombre dentro del inventario.
- Si se encuentra, muestra sus detalles (nombre, precio, cantidad).

### `actualizar_stock(nombre, cantidad)`
- Actualiza la cantidad de stock de un producto existente en el inventario.
- Si el producto no existe, muestra un mensaje informando al usuario.

### `eliminar_producto(nombre)`
- Elimina un producto del inventario si existe.
- Si no se encuentra, se muestra un mensaje al usuario.

### `calcular_valor_inventario()`
- Calcula y muestra el valor total del inventario.
- Multiplica el precio de cada producto por su cantidad y suma los valores para obtener el total.

### `realizar_compra()`
- Permite a un cliente seleccionar productos del inventario y realizar una compra.
- Muestra el inventario al cliente y solicita los productos que desea comprar.
- Calcula el costo total de la compra y actualiza el inventario.

### `procesar_pago()`
- Procesa el pago de una compra y calcula el cambio.
- Utiliza `try...except` para manejar excepciones en caso de que la cantidad pagada sea insuficiente.

### `agregar_cliente(nombre, email)`
- Agrega un nuevo cliente al sistema de clientes de la tienda.
- El cliente es registrado con su nombre y correo electrónico.

### `ver_clientes()`
- Muestra una lista de los clientes registrados, incluyendo sus nombres y correos electrónicos.

### `registrar_compra(nombre_cliente, carrito)`
- Registra una compra realizada por un cliente específico.
- Si el cliente no está en el sistema, muestra un mensaje indicando que no se puede registrar la compra.
- Calcula el total de la compra y lo añade al historial del cliente.

### `ver_compras_cliente(nombre_cliente)`
- Muestra el historial de compras de un cliente, incluyendo los detalles de los productos comprados y los totales.

### `calcular_ventas_totales()`
- Calcula y muestra las ventas totales de la tienda sumando los totales de todas las compras realizadas.
