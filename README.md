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

## Banners informativos actualizados
Se integraron el banner de composición aprobado y cuatro piezas nuevas: presentación, uso y precauciones, comparación de combos y proceso de compra. Los prompts exactos están en `docs/PROMPTS-BANNERS-V3.md` y `docs/PROMPT-BANNER-V2.md`. Los textos también se ofrecen en HTML desplegable, con botones de compra accesibles.

Las cinco imágenes suman 919.024 bytes en sus versiones WebP de mayor tamaño, frente a 9.965.780 bytes de los originales PNG (91 % menos). Se incluyen versiones de 560, 840 y 1120 px y miniaturas de 160 px. La web elige con `srcset`/`sizes`, carga los banners diferidamente y reserva sus dimensiones. La primera imagen del producto tiene precarga y prioridad alta. Los originales de generación se conservan localmente; no se descargan como parte de la página.

## Galería principal
La galería inicial contiene exactamente tres imágenes: frasco Adelfit, composición aprobada y fotografía real de la etiqueta. La composición no se repite como banner más abajo. Las otras cuatro piezas informativas aparecen una sola vez en sus secciones.
