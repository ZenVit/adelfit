# Verificación de la secuencia lifestyle

- Cinco imágenes nuevas generadas con Imagegen integrada; revisadas visualmente, con texto legible, frasco de referencia, escenas con personas adultas y sin resultados clínicos inventados.
- Se ajustaron las frases sobre apetito, hinchazón y peso de los prompts originales por falta de respaldo en el etiquetado disponible. Los prompts finales completos quedan documentados.
- Cinco imágenes consecutivas y en orden 1–5, dentro del mismo contenedor, sin secciones intercaladas. Los cuatro banners anteriores se retiraron de la página; sus archivos se conservan en el repositorio.
- Galería inicial intacta: frasco, composición y etiqueta real, tres miniaturas centradas.
- WebP principales: 1.015.324 bytes. Originales PNG: 11.215.880 bytes. Reducción: 91 %. Versiones de 540, 810 y 1080 px.
- Dimensiones reservadas, carga diferida y transcripciones HTML agrupadas al final del bloque. La última imagen contiene un botón real para abrir el formulario.
- Navegador a 390 px: sin desbordamiento, las cinco imágenes miden 351 × 438,75 px y conservan proporción 4:5. Vista de escritorio a 1280 px también revisada.
- Botón final abre el checkout. Total predeterminado Gs. 259.000 y selección de 3 frascos Gs. 320.000 comprobados. No se confirmó ni se creó ningún pedido nuevo.
- Scripts comprobados con `node --check`, IDs únicos y recursos de imagen existentes. El bloque de envío de pedidos, los precios y la galería inicial se compararon con HEAD y permanecen intactos.
- No se atribuyen métricas de Core Web Vitals reales ni una puntuación Lighthouse.
