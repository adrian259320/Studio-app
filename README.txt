# Estudio — primera versión funcional

## Incluye
- Cursos y temas, con enlaces de YouTube y otras páginas.
- Subtemas marcables como terminados.
- Notas, imágenes (máximo 2 MB por imagen), preguntas y respuestas de repaso.
- Temporizador configurable de estudio y descanso.
- Progreso por curso y estadísticas básicas.
- Tema claro/oscuro.
- Exportación/importación de copia JSON y exportación de apuntes TXT.
- Archivos PWA para preparar instalación en Android.

## Probar
Abrí `index.html` en un navegador moderno. Para instalar como PWA, el proyecto debe publicarse en un hosting HTTPS (o ejecutarse en localhost). En Android, abrí el sitio publicado en Chrome y usá el menú ⋮ → Instalar aplicación / Agregar a pantalla principal.

## Importante: límites de esta versión
- Los datos se guardan localmente en el navegador del dispositivo.
- La sincronización automática en la nube todavía no está conectada; usá Exportar copia para hacer respaldos.
- Los videos locales no se copian a la aplicación; se pueden abrir desde el almacenamiento del teléfono, pero esta versión solo guarda enlaces.
- Las imágenes se guardan dentro de los datos locales del navegador. Exportar una copia JSON también incluirá imágenes y puede generar un archivo grande.
- Para una versión de producción conviene usar IndexedDB para medios, sincronización en la nube con autenticación, y pruebas en varios teléfonos.

## Publicar
Subí los archivos manteniendo la estructura a un hosting estático con HTTPS (por ejemplo, GitHub Pages, Netlify o similar). El service worker funciona únicamente en HTTPS o localhost.
