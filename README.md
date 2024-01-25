# Desafio1RamirezPB

Primer desafío entregable del curso de Programación Backend de CoderHouse.

## Consigna

- Realizar una clase **ProductManager** que gestione un conjunto de productos.
- Debe crearse desde su constructor con el elemento **products**, el cual será un arreglo vacío.

- Cada producto que gestione debe contar con las propiedades:

  - **code** (código identificador)
  - **title** (nombre del producto)
  - **description** (descripción del producto)
  - **price** (precio)
  - **thumbnail** (ruta de imagen)
  - **stock** (número de piezas disponibles)

- Debe contar con un método **addProduct** el cual agregará un producto al arreglo de productos inicial.

  - Validar que no se repita el campo **code** y que todos los campos sean obligatorios.
  - Al agregarlo, debe crearse con un **id** autoincrementable.
  - **id** y **code** son dos atributos diferentes.

- Debe contar con un método **getProducts** el cual debe devolver el arreglo con todos los productos creados hasta ese momento.

- Debe contar con un método **getProductById** el cual debe buscar en el arreglo el producto que coincida con el **id**.

  - En caso de no coincidir ningún **id**, mostrar en consola un error **Not found**.

## Entrega

Archivo de Javascript listo para ejecutarse desde node.

## Prueba

- Se creará una instancia de la clase **ProductManager**.
- Se llamará **getProducts** recién creada la instancia, debe devolver un arreglo vacío **[]**.

- Se llamará al método **addProduct** con los campos:

  - **title**: _producto prueba_,
  - **description**: _Este es un producto prueba_,
  - **price**: _200_,
  - **thumbnail**: _Sin imagen_,
  - **code**: _abc123_,
  - **stock**: _25_

- El objeto debe agregarse satisfactoriamente con un **id** generado automáticamente **sin repetirse**.
- Se llamará el método **getProducts** nuevamente, esta vez debe aparecer el producto recién agregado.
- Se llamará al método **addProduct** con los mismos campos de arriba, debe arrojar un error porque el código estará repetido.
- Se evaluará que **getProductById** devuelva error si no encuentra el producto, o el producto en caso de encontrarlo.
