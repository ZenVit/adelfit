# Adelfit

Landing estática adaptada de ZenVit/articumina. Mantiene su estructura visual, checkout con ubicación, departamentos y ciudades de Paraguay, combos y pago al recibir.

## Precios conservados
- 1 frasco: Gs. 159.000
- 2 frascos: Gs. 259.000 (ahorro Gs. 59.000)
- 3 frascos: Gs. 320.000 (ahorro Gs. 157.000)

## Pedidos
El formulario envía el pedido a la edge function `create-adelfit-order` (Supabase PROD), que lo guarda en el panel (`pedidos_web`, origen `landing_adelfit`) con los precios fijados en el servidor y avisa por Telegram. Después el cliente confirma por WhatsApp con el número de pedido. Si la función falla, se ofrece enviar el pedido por WhatsApp.

## Meta y visitas
Pixel VENTA CAPI: PageView, ViewContent, InitiateCheckout y Purchase con eventID `<pedido>:purchase`. El servidor manda la misma compra por la API de conversiones (`meta-purchase-worker`), así Meta la deduplica. `zv-visitas.js` alimenta la Vista en tiempo real del panel (`data-landing="landing_adelfit"`).

## Contenido y recursos
La composición se tomó de la fotografía de la etiqueta suministrada por el usuario. No se incluyeron promesas de adelgazamiento, reseñas ficticias ni resultados inventados. Las imágenes de presentación son ilustrativas; se incluye la fotografía real de ingredientes y alérgenos. La imagen original del proveedor se conserva.

## Desarrollo
No requiere dependencias ni compilación. Ejecutar `python -m http.server 4173` desde esta carpeta. La configuración del producto y las ofertas está en `CONFIG` dentro de `index.html`.

## Publicación
Preparada para GitHub Pages, rama `main`, raíz `/`. No contiene credenciales privadas. Conserva el Pixel público de la plantilla original y etiqueta los eventos como Adelfit.
