# Blog de Ingeniería Mecánica — Jekyll + GitHub Pages

## Cómo agregar un post nuevo

Creá un archivo `.md` en `_posts/` con formato `YYYY-MM-DD-titulo.md`:

```markdown
---
title: "Mi nuevo artículo técnico"
date: 2026-02-16
tags: [HVAC, Ejemplo]
---

Contenido en Markdown normal.
```

## Cómo agregar un proyecto

Creá un archivo `.md` en `_projects/`:

```markdown
---
title: "Nombre del proyecto"
status: active
description: "Descripción corta."
tags: [Tag1, Tag2]
order: 4
---

Contenido del proyecto.
```

## Estructura

```
_config.yml        ← Configuración
_includes/         ← nav.html, footer.html
_layouts/          ← Templates
_posts/            ← Posts del blog (Markdown)
_projects/         ← Proyectos (Markdown)
assets/css/        ← Estilos
index.html         ← Homepage
```
