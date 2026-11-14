# Simpsonitos

Plantilla limpia de un sitio fan, con la estructura de un índice, una
sección de temporadas y una página para la película. No incluye episodios,
videos, imágenes ni enlaces a contenido con derechos.

El diseño es estilo Simpson y animado, hecho solo con CSS: cielo celeste,
nubes flotando, dona dibujada con CSS, cinta animada y tarjetas con bordes
gruesos. No usa ninguna imagen.

## Estructura

- `index.html` — portada.
- `Temporadas/index.html` — índice de temporadas, sin contenido.
- `La-Pelicula.html` — página de la película, sin reproductor ni enlaces.
- `404.html` — página de no encontrado.
- `assets/style.css` — estilos compartidos animados.

## Publicar con GitHub Pages

En el repositorio: Settings → Pages → Deploy from a branch → rama `main`,
carpeta `/ (root)`. La dirección queda como
`https://Redmith.github.io/Simpsonitos/`.

## Agregar contenido

Agregá solo material que tengas con derechos o que sea tuyo. Cada temporada
puede ser una página nueva dentro de `Temporadas/`, por ejemplo
`Temporadas/temporada-1.html`, enlazada desde `Temporadas/index.html`.
