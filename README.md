# Simpsonitos

Sitio de fans de Los Simpson: menú con las temporadas 1 a 33 y la lista de
los 103 capítulos de las temporadas 1 a 5 (título, fecha y miniatura de TMDB).
La película tiene su propia página (`La-Pelicula.html`).

No se aloja ningún video en este repo. Cada capítulo tiene un hueco para un
reproductor de Byse, vacío hasta que subas ese capítulo a tu propia cuenta.

## Cómo agregar un capítulo que subiste a Byse

1. Subí el capítulo a Byse (desde tu cuenta, como hacés con MI CINE) y esperá
   a que quede procesado.
2. Copiá el código del archivo. En el reproductor de Byse la URL es
   `https://bysesayeveum.com/e/CODIGO` — el código es la parte final.
3. Abrí `Temporadas/N/data.json` (N = temporada), buscá el capítulo por
   `enumber` y poné el código en `"byse"`. Ejemplo:
   ```json
   { "enumber": "1", "ename": "Especial de Navidad de los Simpson",
     "edate": "16-12-1989", "img": "...", "byse": "abc123def456" }
   ```
4. Guardá y publicá. La página del capítulo (`Temporadas/N/C1.html`) muestra
   el reproductor sola; si `"byse"` está vacío muestra "sin video todavía".

Para la película es igual, en `pelicula.json`, campo `"byse"`.

## Estructura

- `index.html` — menú, temporadas 1 a 33, episodio aleatorio.
- `Temporadas/N/N.html` — lista de capítulos de la temporada N.
- `Temporadas/N/Cm.html` — página del capítulo m, con el reproductor Byse.
- `Temporadas/N/data.json` — títulos, fechas, miniaturas y códigos Byse.
- `La-Pelicula.html` + `pelicula.json` — la película.
- `assets/style.css` — estilo Simpson que ya estaba en el repo (no tocar).
- `assets/simpsonitos.css` — estilos extra de temporadas, capítulos y reproductor.

## GitHub Pages

Settings → Pages → Deploy from a branch → `main` → `/ (root)`.
El sitio queda en `https://redmith.github.io/Simpsonitos/`
