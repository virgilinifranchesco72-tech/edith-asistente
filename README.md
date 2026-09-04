# EDITH — asistente personal estático

Página estática de demostración para el señor Franchesco Virgilini. Está preparada para GitHub Pages y utiliza HTML, CSS, JavaScript, Web Speech API, SpeechSynthesis y LocalStorage.

## Prueba local

Abrir `index.html` funciona para la interfaz y el modo demo. Para probar el micrófono, es preferible publicar el sitio mediante HTTPS (GitHub Pages) o usar un servidor local que entregue HTTPS.

## Publicación en GitHub Pages

1. Cree o abra un repositorio en GitHub.
2. Suba `index.html`, `style.css`, `script.js` y `README.md`.
3. Entre en **Settings → Pages**.
4. En **Build and deployment**, seleccione **Deploy from a branch**.
5. Seleccione la rama `main` y la carpeta `/ (root)`.
6. Pulse **Save**.
7. Espere la publicación y copie la URL que GitHub muestre en esa misma pantalla. No se debe adivinar la dirección.

## Seguridad de la IA

Esta versión responde en modo demostración y no contiene claves. Nunca coloque una clave de API en estos archivos ni en un repositorio público. Para conectar una IA real, agregue un backend serverless separado —por ejemplo Cloudflare Workers, Netlify Functions o Vercel Functions— y guarde la clave como variable de entorno en ese proveedor. El navegador llamará al backend, y el backend llamará a la API.

## Privacidad

El historial y la configuración se guardan en LocalStorage del navegador. El botón **Borrar historial** elimina la conversación guardada. Borrar los datos del navegador también elimina esta información.

## Compatibilidad

El reconocimiento de voz funciona preferentemente en Chrome y Edge. Otros navegadores pueden no implementarlo o requerir permisos adicionales. La escritura y la lectura en voz alta permanecen disponibles cuando el micrófono no es compatible.
