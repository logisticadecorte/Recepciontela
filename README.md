# Recepción de Tela — URA Industries

Prototipo web para la recepción de tela por lector de código de barras.
Este archivo es **estático** (no tiene servidor propio) — todo corre en el
navegador. Trae datos de ejemplo incrustados, pero ahora **cualquiera que lo
abra puede actualizar esos datos adjuntando el Excel directamente**, sin
pedírselo a nadie.

## Cómo publicarlo en GitHub Pages (paso a paso, sin terminal)

1. Entra a github.com e inicia sesión (o crea una cuenta gratis).
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

## Cómo actualizar los datos (nuevo — ya no depende de Claude)

En la pantalla "Nueva recepción" hay un cuadro **"Actualizar datos desde
Excel"**. Cualquiera que use la página puede:

1. Descargar/exportar el Excel del histórico desde OneDrive (hoja llamada
   "Historico" o "Historico RIT").
2. Adjuntarlo ahí mismo con el botón de subir archivo.
3. La página lee el archivo **dentro del propio navegador** (usando la
   librería SheetJS que ya viene incluida) — el archivo nunca sale de tu
   computador ni pasa por ningún servidor externo.
4. En segundos aparecen las fechas nuevas en el selector, listas para usar.

Esto reemplaza el proceso anterior de "súbeme el Excel al chat y te regenero
el archivo" — ahora cada persona puede refrescar los datos ella misma, cuantas
veces quiera, directamente desde la página publicada en GitHub.

**Limitación que sigue existiendo:** esto sigue siendo "cada quien actualiza
su propia copia abierta en su navegador" — si tú subes un Excel nuevo en tu
computador, tu compañero en el suyo no lo ve automáticamente; cada quien debe
adjuntar el archivo en su propia sesión. Eso —que todos vean lo mismo sin que
nadie tenga que adjuntar nada— sigue siendo lo que resuelve la conexión real
con SharePoint que dejamos pendiente.

## Qué NO cambia

- **El historial de recepciones cerradas vive en el navegador de cada
  persona**, no en GitHub ni en la nube — sigue sin compartirse entre equipos.
- Este sigue siendo el mismo prototipo de siempre — GitHub Pages es solo una
  forma más cómoda de compartir el link en vez de mandar el archivo por chat.
