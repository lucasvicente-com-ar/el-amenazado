# El amenazado

Un sitio de una sola página dedicado a **«El amenazado»**, poema de Jorge Luis Borges publicado en *El oro de los tigres* (1972).

👉 **Ver el sitio:** https://lucasvicente-com-ar.github.io/el-amenazado/

![Vista previa](el-amenazado.png)

## Qué contiene

- **Hero a pantalla completa** con la ilustración de portada — se muestra completa (sin recortes, `object-fit: contain`) sobre un fondo desenfocado de la misma imagen para llenar el encuadre en cualquier tamaño de pantalla.
- **El poema completo**, con capitular decorativa y versos que aparecen suavemente al hacer scroll (`IntersectionObserver`).
- **Dos notas de lectura**, escritas como acompañamiento del poema y la imagen:
  - *Sobre la imagen* — una lectura simbólica de cada elemento de la ilustración (el hombre, la biblioteca, la máscara, el cántaro roto, la figura femenina, los ejércitos, el ave, la oscuridad).
  - *Sobre el poema* — un análisis de «El amenazado» como el amor vivido no como refugio, sino como una fuerza que desarma la identidad.
- **Firma** al pie de página, con la fecha de escritura de los textos y una dedicatoria.
- Diseño editorial oscuro (tipografía Cormorant Garamond + Cinzel, acentos dorados), parallax sutil en el fondo del hero, grano fotográfico y animaciones de aparición al hacer scroll. Totalmente responsive — probado en mobile.

## Estructura

```
.
├── index.html          # el sitio completo: HTML + CSS + JS inline, sin build ni dependencias
│                        #   (solo carga Google Fonts vía CDN)
├── el-amenazado.png     # ilustración de portada
├── el amenazado.txt     # texto del poema en bruto, fuente original
└── README.md
```

## Desarrollo local

No requiere instalación ni build. Alcanza con abrir `index.html` en el navegador, o servir la carpeta con cualquier servidor estático:

```bash
python -m http.server 8000
```

y visitar `http://localhost:8000`.

## Publicación

El sitio se sirve con **GitHub Pages** desde la rama `master`, raíz del repositorio (`/`). Cualquier `git push` a `master` se refleja automáticamente en unos minutos en:

https://lucasvicente-com-ar.github.io/el-amenazado/

## Créditos

«El amenazado», Jorge Luis Borges, de *El oro de los tigres* (1972).
