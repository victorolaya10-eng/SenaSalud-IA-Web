# SeñaSalud IA — versión web instalable (PWA)

## Contenido
- `index.html`: interfaz web original adaptada para cargar como sitio.
- `video_interprete_lsc.mp4`: video local del intérprete LSC.
- `manifest.webmanifest`, `service-worker.js` e `icons/`: soporte básico para instalación como app web.

## Publicación
Publica **todos** estos archivos manteniendo la estructura de carpetas en un alojamiento HTTPS estático. No cambies el nombre `video_interprete_lsc.mp4`.

## Instalar en iPhone
1. Abre la URL HTTPS publicada en Safari.
2. Pulsa Compartir.
3. Selecciona “Añadir a pantalla de inicio”.
4. Confirma con “Añadir”.

## Importante
- El sitio debe servirse por HTTPS para que el service worker funcione.
- La interfaz se guarda para acceso básico sin conexión, pero el video no se precarga sin conexión por su tamaño (aprox. 39 MB).
- Esta versión conserva el HTML existente; no convierte el proyecto Flutter a Flutter Web.
- Antes de usar con pacientes o publicar públicamente, revisa autenticación, privacidad y cualquier dato médico. No cargues datos reales de pacientes en una demo pública.
