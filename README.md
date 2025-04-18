# 🍓📦 Proyecto-Final-ED1 — Sistema de Gestión de Inventario para Tienda de Frutas y Verduras

Este es un proyecto final desarrollado en Python que implementa un **Sistema de Gestión de Inventario** para una tienda de frutas y verduras. El sistema permite llevar un control detallado de productos, proveedores, clientes, transacciones y movimientos de inventario, incluyendo funciones avanzadas como gestión de productos de temporada y rebajas por fecha de expiración.

## 📌 Funcionalidades principales

- ✅ Registro, consulta, actualización y eliminación de productos.
- ✅ Control de stock, fechas de expiración y aplicación de rebajas.
- ✅ Gestión completa de proveedores y clientes.
- ✅ Registro de ventas con distintos métodos de pago.
- ✅ Seguimiento de movimientos de inventario (compras y ventas).
- ✅ Módulo de rotación de inventario con lógica de temporada y expiración.

## 🧱 Estructura del sistema

El proyecto se estructura mediante programación orientada a objetos. Las clases principales son:

### 🔸 `Producto`
Controla toda la información relacionada con los productos: stock, rebajas, expiración, etc.

### 🔸 `Proveedor`
Gestiona la información de los proveedores de la tienda.

### 🔸 `Cliente`
Administra los datos de los clientes y su tipo (minorista/mayorista), además de un sistema de crédito.

### 🔸 `Transaccion`
Registra ventas y pagos, asociándolos a los clientes.

### 🔸 `EstadoMovimiento`
Lleva un registro de todos los movimientos del inventario por fecha o tipo (venta/compra).

### 🔸 `RotacionInventario`
Controla la disponibilidad de productos por temporada y detecta cuándo aplicar rebajas.

## 🗃️ Base de datos (SQLite)

El sistema utiliza SQLite con tablas bien definidas para manejar la persistencia de datos:

- `productos`
- `proveedores`
- `clientes`
- `transacciones`
- `estado_movimiento`
- `rotacion_inventario`

## 🔁 Flujo de operaciones

1. El usuario puede registrar productos nuevos y controlar el stock.
2. Se vinculan productos a proveedores para mantener trazabilidad.
3. Los clientes pueden comprar productos según su tipo y método de pago.
4. Las transacciones se registran y se reflejan en el movimiento de inventario.
5. El sistema aplica automáticamente rebajas a productos cercanos a su expiración.
6. Los productos de temporada se gestionan para que solo estén disponibles en fechas específicas.

## 🧪 Casos especiales implementados

- 🗓️ **Productos por temporada**
- ⏰ **Rebajas automáticas por expiración**
- 📊 **Consultas por tipo y fecha de movimiento**

## 🛠️ Tecnologías utilizadas

- Python 3.x
- SQLite3
- Módulos estándar: `datetime`, `json`, etc.

## 🚀 Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/a-nxwball/Proyecto-Final-ED1.git
   cd Proyecto-Final-ED1
