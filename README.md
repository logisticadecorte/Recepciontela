# Recepción de Tela — URA Industries

Prototipo web para la recepción de tela por lector de código de barras.
Este archivo es **estático** (no tiene servidor propio) — todo corre en el
navegador, y los datos del histórico están incrustados dentro del mismo
`index.html`.

## Cómo publicarlo en GitHub Pages (paso a paso, sin terminal)

1. Entra a [github.com](https://github.com) e inicia sesión (o crea una cuenta gratis).
2. Arriba a la derecha, clic en el **+** → **New repository**.
3. Ponle un nombre, por ejemplo `recepcion-tela-ura`. Puede ser **privado**
   (recomendado, ya que trae datos internos de URA) o público — tú decides.
4. Clic en **Create repository**.
5. En la página del repo recién creado, busca el enlace **"uploading an existing file"**
   (o el botón **Add file → Upload files**).
6. Arrastra el archivo `index.html` de esta carpeta y dale **Commit changes**.
7. Ve a la pestaña **Settings** del repositorio → en el menú lateral, **Pages**.
8. En "Branch", selecciona `main` (o `master`) y carpeta `/ (root)` → **Save**.
9. Espera 1-2 minutos. GitHub te va a mostrar un enlace tipo:
   `https://TU-USUARIO.github.io/recepcion-tela-ura/`
   Ese es el link que puedes compartir con tu equipo — abre directo el prototipo,
   sin que nadie tenga que descargar nada.

> Nota si el repositorio es **privado**: GitHub Pages en repos privados solo
> está disponible en planes de pago (GitHub Pro/Team/Enterprise). Si tu cuenta
> es gratuita y el repo es privado, Pages no se activará — en ese caso hazlo
> público, o usa un servicio alterno como Netlify/Vercel (arrastras el mismo
> `index.html` y listo, sin necesidad de cuenta de GitHub).

## Cosas importantes que debes saber antes de compartir el link

- **Los datos quedan "congelados" el día que subas el archivo.** Este
  `index.html` no se conecta en vivo a tu Excel de OneDrive — trae los datos
  de la última vez que actualizamos el prototipo (hoy, hasta el 06/08/2026).
  Para traer fechas nuevas, tienes que repetir este mismo proceso: pídeme el
  archivo actualizado, y vuelves a subir el `index.html` nuevo a GitHub
  (Add file → Upload files, reemplaza el anterior).
- **El historial de recepciones cerradas vive en el navegador de cada
  persona**, no en GitHub ni en la nube — si dos personas abren el mismo link
  desde dos computadores distintos, cada quien ve su propio historial, no el
  del otro. Esto es igual a como funciona hoy, GitHub solo cambia *dónde* se
  aloja el archivo, no *cómo* funciona por dentro.
- Este sigue siendo el mismo prototipo de siempre — GitHub Pages es solo una
  forma más cómoda de compartir el link en vez de mandar el archivo por chat.
  La conexión en tiempo real con SharePoint (que dejamos pendiente) sigue
  siendo el cambio que de verdad resuelve lo de "datos siempre actualizados"
  y "todos ven lo mismo".
