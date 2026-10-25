# CANCHA — prototipo web estático

## Qué incluye
- Interfaz responsive en español, con estética oscura para deportes.
- Catálogo de canales por categorías, búsqueda y favoritos.
- Importación local de listas M3U y guía XMLTV `.xml`.
- Sin cuentas, base de datos, backend ni servidor de vídeo.

## Cómo probar
1. Descomprime el ZIP.
2. Abre `index.html` en Chrome, Edge o Firefox.
3. Pulsa **Importar lista** y selecciona tu `.m3u`.
4. Pulsa **Cargar guía XMLTV** y selecciona un XMLTV `.xml` sin comprimir.
5. Para publicarla gratis, sube `index.html` a GitHub Pages, Cloudflare Pages o Netlify.

## Limitaciones importantes
- El prototipo no reproduce directamente enlaces `acestream://`: los navegadores no entienden ese protocolo como una fuente de vídeo web estándar.
- No se incluye un proxy ni un servidor que convierta AceStream a HLS. Esa conversión requiere un proceso que esté funcionando en algún equipo/servidor y puede consumir ancho de banda; por tanto, no es realista prometer reproducción de AceStream desde cualquier navegador sin instalar nada y con coste cero de servidor.
- La guía solo muestra información que exista en el XMLTV importado y que corresponda a la hora actual. El prototipo no garantiza la correspondencia entre IDs de la lista y canales de la guía.
- Utiliza únicamente streams y logotipos que tengas derecho a usar. El prototipo no incorpora los hashes de AceStream: importa tu lista localmente en el navegador.
- Los XMLTV `.gz` comprimidos no se descomprimen en esta versión; selecciona una versión `.xml`.

## Para convertirlo en una web de producción
Haría falta confirmar fuentes de vídeo legales y compatibles con navegador (HLS/DASH), una fuente EPG fiable y sus condiciones de uso. Si solo alojas archivos estáticos, el coste de servidor puede ser 0 dentro de los límites gratuitos; alojar o retransmitir vídeo es otra cosa.
