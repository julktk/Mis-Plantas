# Mis plantas

Registro de riegos, calendario, avisos y guías de cuidado para mis plantas de interior.

## Publicar en GitHub Pages

1. En GitHub, crea un repositorio nuevo, por ejemplo `mis-plantas`. En el plan gratuito tiene que ser **público** para usar Pages.
2. Sube `index.html` (y este README si quieres). El archivo `google-apps-script.gs` no hace falta subirlo: es para Google Sheets.
3. En el repositorio: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, rama `main`, carpeta `/ (root)` → **Save**.
4. En uno o dos minutos la app estará en `https://TU-USUARIO.github.io/mis-plantas/`.
5. Ábrela en el móvil y usa **Añadir a pantalla de inicio**.

Tus registros y fotos no van al repositorio: se guardan en tu navegador (y en tu Google Sheets si lo conectas).

## Primeros pasos en la app

- Abre cada planta y anota cuándo la regaste por última vez.
- En **Ajustes de la planta** puedes añadir una foto.
- En **Ajustes → Copia de seguridad**, exporta una copia de vez en cuando.

## Conectar Google Sheets (opcional)

1. Crea una hoja nueva en Google Sheets, por ejemplo «Mis plantas».
2. **Extensiones → Apps Script**. Borra el contenido y pega `google-apps-script.gs`.
3. Cambia `cambia-esta-clave` en la primera línea por una clave tuya y guarda.
4. **Implementar → Nueva implementación**. Tipo: **Aplicación web**. Ejecutar como: **Yo**. Quién tiene acceso: **Cualquier usuario**. Autoriza los permisos (Google avisará de que la app no está verificada: es tu propio script, pulsa *Configuración avanzada → Ir a…*).
5. Copia la URL que termina en `/exec`. Si la abres en el navegador debe decir que el script funciona.
6. En la app: **Ajustes → Google Sheets**, pega la URL y tu clave y pulsa **Guardar y sincronizar**. Repite este paso en cada dispositivo.

La hoja tendrá dos pestañas: **Plantas** y **Registros**. Puedes consultarlas, pero es mejor hacer los cambios desde la app.
