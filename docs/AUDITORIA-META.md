# Revisión de Adelfit antes de anunciar en Meta

Fecha: 6 de noviembre de 2026, Paraguay.

## Comprobado
- Galería inicial con tres imágenes elegidas, miniaturas centradas y sin duplicar los banners inferiores.
- Foto principal proporcionada y sin desbordamientos observados. Imágenes WebP adaptativas y carga diferida.
- Combos de Gs. 159.000, 259.000 y 320.000; ahorro y precio por frasco visibles.
- Formulario, mapa opcional, lista de departamentos/ciudades y validación de cinco campos obligatorios. No se envió ningún pedido nuevo en esta revisión.
- Contacto WhatsApp al 595972738779 y pago al recibir.
- Precauciones, ingredientes, alérgenos y etiqueta real disponibles. No se encontraron promesas de adelgazamiento, antes/después ni testimonios ficticios en las piezas revisadas.
- Pixel 2141006803281667 configurado con PageView, ViewContent, InitiateCheckout y Purchase. El código usa pedido:purchase como eventID.
- Se consultó el evento de prueba anterior PY92167233:purchase: el servidor lo marca enviado y la respuesta de Meta contiene events_received=1. Esto comprueba recepción de ese evento del servidor, no deduplicación de navegador/servidor ni aptitud de la cuenta para anunciar.

## Prioridad antes de invertir
1. Publicar política de privacidad que describa pedido, entrega, WhatsApp, analítica y publicidad de Meta; explicar el uso de Pixel/CAPI y las opciones del visitante. Actualmente no existe un enlace de privacidad y el formulario afirma que los datos solo se usan para la entrega, lo que no refleja toda la medición instalada. La implementación de consentimiento debe definirse según el público y el marco aplicable.
2. Publicar condiciones de envío, cambios/devoluciones y atención: cobertura, tiempos reales, gestión de productos dañados/equivocados y procedimiento de contacto. No inventar plazos o garantías.
3. Identificar al vendedor: razón social/nombre comercial, datos comerciales y contacto verificables, domicilio de atención y correo de soporte. Hoy solo se muestra ZenVit Store y WhatsApp.
4. Revisar en Administrador de eventos el origen/dataset, permisos de la cuenta, diagnósticos, deduplicación, dominio y restricciones aplicables a salud/bienestar. La sesión disponible solicita iniciar sesión; no se pudo verificar esa configuración de cuenta. No se crearon anuncios ni se comprometió presupuesto.
5. Verificar con el proveedor la documentación y autorización de comercialización que corresponda al producto en Paraguay. Esta revisión visual/técnica no certifica su situación sanitaria ni la aprobación futura de Meta.

## Mejoras de conversión recomendadas
- Preguntas frecuentes visibles antes del pedido: entrega por zona, pago al recibir, contenido del combo, cambios y alergias.
- Video real corto del envase y su etiqueta; reseñas únicamente de compradores reales, con autorización.
- Metadatos Open Graph para la vista previa al compartir y un dominio propio como mejora de marca.
- Parámetros UTM por creativo para comparar anuncios; la página ya recoge la fuente/campaña y fbclid.
- Auditar Purchase por pedido contra entrega frente a ventas confirmadas/cobradas antes de interpretar ROAS como dinero cobrado.

## Política oficial consultada
Se leyó en navegador la versión «Hoy» de Salud y bienestar del Centro de transparencia de Meta. Incluye restricción de segmentación a mayores de 18 años para suplementos dietéticos y nutricionales, y restricciones a mensajes sobre apariencia física y afirmaciones sanitarias/sensacionalistas. Evitar afirmar atributos personales o resultados no respaldados.
https://transparency.meta.com/policies/ad-standards/restricted-goods-services/health-wellness/

## Límites de esta verificación
No se obtuvo acceso al Administrador de eventos ni al Administrador de anuncios. No se midieron Core Web Vitals de usuarios reales ni una puntuación Lighthouse. No se certificaron requisitos legales/sanitarios ni se garantiza la aprobación publicitaria.
