# WareIQ · Piloto de inventarios — GitHub Pages

## Publicación prevista

Dirección propuesta: https://piloto.wareiqconsulting.es
El archivo CNAME ya contiene ese subdominio. Su inclusión no lo publica ni cambia DNS.
Este paquete está preparado para servirse en la raíz de ese subdominio.

## 1. Crear el repositorio del piloto

Crear un repositorio separado, por ejemplo wareiq-piloto-auditores.
No cargar estos archivos sobre el repositorio de la página principal.
Con GitHub Free, normalmente se usa un repositorio público para Pages.
La publicación estándar es pública: no incorpora restricción por correo de Wilmer.
Los perfiles dentro de esta app son simulados, no una autenticación real.

## 2. Cargar los archivos

Extraer este ZIP en la computadora.
En el repositorio nuevo: Add file > Upload files.
Subir los archivos extraídos y la carpeta assets, manteniendo su estructura.
No subir el ZIP como único archivo ni una carpeta contenedora extra.
index.html, app.js, style.css, sw.js, manifest.webmanifest, icon.svg y CNAME
 deben quedar directamente en la raíz del repositorio; assets debe quedar a su lado.
También se incluye .nojekyll (archivo vacío). Si Windows no lo muestra,
puede crearse desde Add file > Create new file, nombre .nojekyll.
Confirmar la carga con Commit changes.
No se necesitan npm, Node.js, compilación ni servidor adicional.

## 3. Activar Pages

Abrir Settings > Pages > Build and deployment.
En Source: Deploy from a branch.
Elegir la rama que contiene los archivos (habitualmente main) y carpeta / (root).
Guardar. En Custom domain escribir piloto.wareiqconsulting.es y guardar.
Conservar siempre CNAME al actualizar los archivos.
Si Pages no permite activar la publicación, revisar el plan y la visibilidad
 del repositorio antes de contratar un servicio adicional.

## 4. Conectar el subdominio en Hostinger

Si los DNS siguen administrándose en Hostinger:
Dominios > wareiqconsulting.es > DNS/Nameservers > administrar registros.
Agregar:
- Tipo: CNAME
- Nombre: piloto
- Destino: USUARIO-O-ORGANIZACION.github.io
- TTL: valor predeterminado

Sustituir USUARIO-O-ORGANIZACION por el nombre real de la cuenta u organización
propietaria del repositorio. No usar el correo ni agregar la ruta del repositorio.
No copiar literalmente el marcador USUARIO-O-ORGANIZACION.
Si ya existe un registro para piloto, revisarlo antes de modificarlo.
Conservar los registros de @, www, correo y los nameservers existentes.
Si los DNS están administrados en otro proveedor, agregar allí el registro.
No hace falta contratar alojamiento web en Hostinger para esta publicación.

## 5. Activar HTTPS y comprobar

Esperar a que GitHub valide DNS y emita el certificado. No siempre es inmediato.
En Settings > Pages activar Enforce HTTPS cuando esté disponible.
Abrir https://piloto.wareiqconsulting.es desde computadora y Chrome de Android.
No usar la dirección temporal usuario.github.io/repositorio para probar este
paquete: sus recursos usan rutas desde la raíz del subdominio personalizado.
Si faltan estilos o imágenes, verificar el dominio personalizado y que los
archivos estén en la raíz y assets en su carpeta original.

## 6. Prueba con Wilmer

Compartir el enlace HTTPS definitivo después de comprobarlo.
Abrir Chrome > menú de tres puntos > Añadir a pantalla de inicio / Instalar,
según la opción que ofrezca el dispositivo.
Crear una prueba ficticia, cerrar y reabrir en el mismo navegador.
Verificar validaciones, COI en Resultados, activos adicionales, firma,
correcciones y eliminación de pruebas.
Con internet, esperar a que la app indique que los recursos están preparados
sin conexión. Después probar borrador y reapertura en modo avión en ese celular.
La instalación, apertura sin conexión y firma táctil requieren comprobación
real en el dispositivo; este paquete no certifica esa prueba física.
Google Maps necesita conexión.

## Alcance y conservación de información

Cada navegador/dispositivo guarda sus propios registros. Sergio y Wilmer
no verán automáticamente los registros del otro.
Todavía no hay base central, asignación real, autenticación por rol,
sincronización entre equipos ni actualización automática de Power BI/Excel.
El cambio de dirección no copia los registros del piloto anterior: descargar
un respaldo allí si se desea conservarlos. Este paquete no incluye registros
capturados, firmas reales, contraseñas ni las bases Excel internas.
Las tres agencias y sus activos corresponden al catálogo de demostración
proporcionado; los auditores son ficticios.
No borrar datos del navegador ni usar incógnito para una prueba persistente.
Descargar respaldos desde la app antes de mover o limpiar sus datos.

## Actualizaciones

Reemplazar los archivos del piloto dentro del mismo repositorio y mantener
el dominio, la carpeta assets y el archivo CNAME. Mantener la clave de
almacenamiento para conservar registros en el mismo navegador.
Si se modifica el código, incrementar la versión de caché en sw.js.
No cargar respaldos de registros o firmas al repositorio público.

## Documentación oficial

https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
