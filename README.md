# Implementación de Lazy Load en Shopify

Este script permite implementar la técnica de Lazy Load en las imágenes de tu tienda Shopify. El Lazy Load retrasa la carga de imágenes hasta que estén en el punto de vista del usuario, lo que puede mejorar la velocidad de carga de la página y la experiencia del usuario.

## ¿Cómo funciona?

1. **Modificación de imágenes**: El script busca todas las imágenes en la página y modifica las etiquetas de imagen para usar `data-src` en lugar de `src`. Esto evita que la imagen se cargue inmediatamente al cargar la página.

2. **Implementación del Lazy Load**: El script utiliza la API `IntersectionObserver` para detectar cuándo las imágenes entran en el viewport y cargarlas en ese momento. Si el navegador no soporta `IntersectionObserver`, el script cargará las imágenes inmediatamente como un fallback.

## ¿Cómo implementarlo?

1. Copia el código JavaScript proporcionado.
2. Pega el código al final de tu archivo `theme.liquid` antes del cierre de la etiqueta `</body>`.
3. Guarda los cambios y prueba tu tienda para asegurarte de que el Lazy Load esté funcionando correctamente.

## Notas

- Asegúrate de hacer una copia de seguridad de tu tema antes de realizar cualquier modificación.
- Si experimentas problemas o comportamientos inesperados, considera contactar a un desarrollador o experto en Shopify para obtener asistencia.
