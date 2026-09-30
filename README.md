# pablombarral.github.io

Sitio personal: CV y blog. Jekyll, construido por GitHub Pages sin
configuración adicional.

## Qué hay dónde

| Para cambiar | Editar |
|---|---|
| El CV | `_data/cv.yml` (fuente única; la página `/cv/` se arma sola) |
| El texto del inicio | `index.html` |
| Perfiles (ORCID, Scholar, GitHub, LinkedIn) y mail | `_config.yml` |
| Estilos | `assets/css/main.css` |
| El diagrama de Mollier | `_includes/hs-diagram.svg` |

## Publicar una nota

1. Copiar `_drafts/plantilla.md` a `_posts/AAAA-MM-DD-titulo-corto.md`.
2. Escribir en Markdown. Si lleva ecuaciones, poner `math: true` en el encabezado.
3. `git add`, `git commit`, `git push`. En uno o dos minutos está en línea.

Los borradores que queden en `_drafts/` no se publican.

## Vista local (opcional)

Requiere Ruby. `bundle install` una vez y después `bundle exec jekyll serve`;
el sitio queda en <http://localhost:4000>. Para ver también los borradores:
`bundle exec jekyll serve --drafts`.
