# MyRentall Quotas Widget

Este es un ejemplo funcional de cómo integrar el widget de cuotas de **MyRentall** en cualquier sitio web, permitiendo mostrar automáticamente las opciones de financiación disponibles para un producto.

---

## 🚀 Ejecutar el ejemplo

### 1. Abrir el archivo localmente

No se requiere compilación ni entorno de desarrollo. Simplemente abre el archivo `index.html` en tu navegador, o sírvelo desde un servidor local para evitar posibles restricciones por CORS.

### 2. Configura el `sku` y el `price`

Abre `index.html` y reemplaza los valores de `sku` y `price` por los correspondientes a tu producto:

```js
widget.mount({
  sku: 'SKU_DEL_PRODUCTO',     // Código único del producto. Obligatorio.
  price: 1000,                 // (Opcional) Precio sin IVA. Si no se indica, se usará el almacenado en nuestra base de datos.
  selector: '#sdk-product-quotas' // ID del contenedor HTML donde se montará el widget
});
