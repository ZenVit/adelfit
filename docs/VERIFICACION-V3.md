# Verificación de los banners informativos

- Cinco banners finales: composición aprobada, presentación, uso y precauciones, comparación de combos y compra/entrega.
- Prompts completos: `PROMPTS-BANNERS-V3.md` y `PROMPT-BANNER-V2.md`. Generación con Imagegen integrada.
- Fuentes PNG finales: 9.965.780 bytes. Cinco WebP principales: 919.024 bytes; reducción del 91 %. Derivadas de 160, 560 y 840 px adicionales para miniaturas y pantallas pequeñas.
- Comprobación en navegador: 360 y 390 px en móvil y 1280 px en escritorio, sin desbordamiento horizontal.
- Galería de siete imágenes y fotografía real del etiquetado disponibles. En móvil el navegador eligió la variante de 560 px y miniaturas de 160 px.
- Al abrir desde arriba, solo se cargó el primer banner próximo a la pantalla; los otros cuatro permanecieron diferidos. Al recorrer la página, los cinco cargaron sin imágenes rotas.
- Dimensiones de imágenes reservadas; precarga y prioridad alta para la foto principal. Eliminada la descarga anticipada mediante sondas `new Image()` de los cinco banners.
- Texto alternativo específico y transcripciones HTML desplegables. Dos botones nuevos abren el formulario.
- Precios, subtotales y selección de combos comprobados: 159.000, 259.000 y 320.000 guaraníes. Validación de cinco campos obligatorios comprobada.
- JavaScript sin errores de sintaxis ni errores de consola observados; todas las rutas de imágenes existen y no hay IDs duplicados. El bloque de envío de pedidos conserva exactamente la integración del panel que ya estaba configurada.
- Una prueba completa registró PY92167233. El pedido se canceló y archivó, verificado en base de datos. Su evento de compra ya había sido enviado a Meta. No se hicieron más pedidos.
- No se dispone de una traza de rendimiento ni de métricas reales de Core Web Vitals: se verificaron pesos, carga diferida, selección adaptativa, dimensiones y comportamiento en navegador. No se atribuye una puntuación Lighthouse.
