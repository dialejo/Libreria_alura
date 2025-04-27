# 📚 Modelado de Base de Datos - E-commerce de Libros

Este proyecto consiste en el diseño del modelo de base de datos para una tienda en línea enfocada en la venta de libros. El objetivo principal es estructurar de manera adecuada la información de clientes, libros, editoriales y pedidos, con sus respectivas relaciones y atributos.

## 🧩 Objetivo del Modelo

Permitir el almacenamiento y consulta eficiente de:

- Datos personales de los clientes (naturales y jurídicos).
- Información detallada de los libros.
- Datos de las editoriales proveedoras.
- Registro de pedidos de compra.
- Control de inventario por libro.

---

## 🧑‍💼 Entidad: Cliente

El cliente puede ser una:

- **Persona Natural**
  - DNI
  - RUT
- **Persona Jurídica**
  - NIT
  - RUES

Atributos comunes:
- Nombre
- Dirección
- Teléfono
- E-mail

---

## 📚 Entidad: Libro

Cada libro tiene los siguientes atributos:

- Título
- Categoría
- ISBN
- Año de publicación
- Valor
- Autor(a)
- Casa editorial (una sola editorial por libro)

---

## 🏢 Entidad: Editorial

Los libros son provistos por **una única editorial**. Cada editorial cuenta con:

- Nombre
- E-mail
- Nombre de contacto
- Teléfono (máximo 2 números)

---

## 📦 Entidad: Pedido de Compra

Un pedido puede incluir **uno o varios libros**.

- El cliente realiza el pedido.
- Antes de registrar un pedido, se valida la disponibilidad del libro en inventario.

---

## 🗃️ Entidad: Inventario

Asocia libros con su **disponibilidad actual**.

- Cada vez que se realiza un pedido, se descuenta del inventario.
- No se permiten ventas si el inventario está agotado.

---

## 🔗 Relaciones Clave

- Un cliente puede tener múltiples pedidos.
- Un pedido puede tener múltiples libros.
- Un libro pertenece a **una sola editorial**.
- Una editorial puede proveer **varios libros**.

---

## 📐 Alcance del Proyecto

✔️ Este proyecto incluye:

- Modelado entidad-relación (ER).
- Definición de entidades, atributos y relaciones.
- Reglas de negocio clave reflejadas en las relaciones.
- Modelo logico
- Modelo Fisico

❌ Este proyecto **no incluye**:

- Desarrollo del backend o frontend.
- Implementación de lógica de inventario o flujo de compra.

---

## ✍️ Autor 

- Diego Maldonado