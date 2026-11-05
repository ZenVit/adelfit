# Adelfit

Landing estática adaptada de ZenVit/articumina. Mantiene su estructura visual, checkout con ubicación, departamentos y ciudades de Paraguay, combos y pago al recibir.

## Precios conservados
- 1 frasco: Gs. 159.000
- 2 frascos: Gs. 259.000 (ahorro Gs. 59.000)
- 3 frascos: Gs. 320.000 (ahorro Gs. 157.000)

## Pedidos
El formulario valida datos y prepara un resumen para WhatsApp al 595972738779. El cliente debe enviar ese mensaje. No registra pedidos en el endpoint de Articumina ni muestra una compra confirmada antes del envío. No se ha configurado un endpoint de panel para Adelfit.

## Contenido y recursos
La composición se tomó de la fotografía de la etiqueta suministrada por el usuario. No se incluyeron promesas de adelgazamiento, reseñas ficticias ni resultados inventados. Las imágenes de presentación son ilustrativas; se incluye la fotografía real de ingredientes y alérgenos. La imagen original del proveedor se conserva.

## Desarrollo
No requiere dependencias ni compilación. Ejecutar `python -m http.server 4173` desde esta carpeta. La configuración del producto y las ofertas está en `CONFIG` dentro de `index.html`.

## Publicación
Preparada para GitHub Pages, rama `main`, raíz `/`. No contiene credenciales privadas. Conserva el Pixel público de la plantilla original y etiqueta los eventos como Adelfit. No envía eventos Purchase para pedidos que aún no fueron recibidos.
