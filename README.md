# MotoAhorro — sitio web estático

Preparado para GitHub Pages, responsive y en español.

## Archivos
- `index.html`: portada, pasos, imágenes de referencia, manual, instalación, FAQ y CTA de descarga pendiente.
- `styles.css`: diseño responsive.
- `script.js`: menú móvil, pestañas del manual y función de compartir.
- `assets/`: las dos imágenes de referencia y favicon.

## Activar descarga cuando el APK esté listo
En `index.html`, busca el bloque del botón `class="button disabled"`. Cambia `href="#descarga"` por la URL pública del APK, elimina `aria-disabled="true"` y cambia la clase `disabled` por una clase de botón activo. Sube el APK a GitHub Releases o a un alojamiento fiable.

## Publicar en GitHub Pages
1. Crea un repositorio público, por ejemplo `motoahorro-web`.
2. Sube el contenido de esta carpeta a la raíz del repositorio.
3. En GitHub entra en **Settings → Pages**.
4. Selecciona **Deploy from a branch**, rama `main`, carpeta `/(root)` y guarda.
5. La URL tendrá el formato `https://TU-USUARIO.github.io/motoahorro-web/`.

## Dominio propio
Puedes comprar un dominio como `motoahorro.com` o `motoahorro.co` si está disponible. En **Settings → Pages → Custom domain**, configúralo y crea en el panel DNS del registrador los registros exactos que GitHub indique. Para `www` suele utilizarse un CNAME hacia `TU-USUARIO.github.io`; para el dominio raíz, configura los registros A/AAAA que GitHub documente en ese momento. Cuando la DNS se propague, activa **Enforce HTTPS**. El dominio normalmente tiene un coste anual.

## Antes del lanzamiento
Las imágenes son referencias visuales. La tarifa de $4.000 COP y el flujo de cambio de tarifa aparecen como información de diseño facilitada para el proyecto; verifica textos y funciones en la versión final de la app antes de presentarlos como definitivos. El botón de descarga está desactivado deliberadamente hasta que exista un APK oficial.
