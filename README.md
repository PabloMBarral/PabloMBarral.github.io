# Blog de Ingeniería Mecánica — Jekyll + GitHub Pages

## Deploy rápido

1. Creá un repo en GitHub llamado `tu-usuario.github.io`
2. Subí **todo el contenido** de esta carpeta al repo
3. En **Settings → Pages**, seleccioná rama `main` y carpeta `/ (root)`
4. GitHub detecta Jekyll automáticamente y hace el build solo

Tu sitio va a estar en `https://tu-usuario.github.io` en ~2 minutos.

## Cómo agregar un post nuevo

Creá un archivo `.md` en la carpeta `_posts/` con este formato de nombre:

```
_posts/YYYY-MM-DD-titulo-del-post.md
```

Ejemplo: `_posts/2026-02-16-nuevo-articulo.md`

El archivo arranca con un encabezado YAML y después Markdown normal:

```markdown
---
title: "Mi nuevo artículo técnico"
date: 2026-02-16
tags: [HVAC, Ejemplo]
---

Acá va el contenido del post en Markdown normal.

## Podés usar subtítulos

Y código:

​```python
print("hola mundo")
​```

Y **negritas**, *itálicas*, [links](https://ejemplo.com), imágenes, etc.
```

Guardá el archivo, hacé commit, y el post aparece automáticamente en el blog.

## Cómo agregar un proyecto nuevo

Igual que los posts pero en `_projects/`:

```markdown
---
title: "Nombre del proyecto"
status: active          # active o completed
description: "Descripción corta que aparece en la tarjeta de la home."
tags: [Tag1, Tag2]
order: 4
---

Contenido detallado del proyecto en Markdown.
```

## Estructura del sitio

```
├── _config.yml          ← Configuración general (título, URL, etc.)
├── _includes/
│   ├── nav.html         ← Barra de navegación
│   └── footer.html      ← Pie de página (editar links acá)
├── _layouts/
│   ├── default.html     ← Layout base
│   ├── post.html        ← Layout de posts del blog
│   └── project.html     ← Layout de proyectos
├── _posts/              ← ✏️ TUS POSTS VAN ACÁ
│   ├── 2025-11-18-cascadas-de-presion-salas-limpias.md
│   ├── 2025-09-03-verificacion-rendimiento-calderas-abma.md
│   └── ...
├── _projects/           ← ✏️ TUS PROYECTOS VAN ACÁ
│   ├── rmb-planta-farmaceutica.md
│   └── ...
├── assets/css/
│   └── style.css        ← Estilos (no necesitás tocarlo)
├── index.html           ← Homepage
└── README.md            ← Este archivo
```

## Editar contenido existente

- **Bio / Sobre mí:** Editar directamente en `index.html`
- **Docencia / Publicaciones:** Editar directamente en `index.html`
- **Links del footer:** Editar `_includes/footer.html`
- **Título del sitio:** Editar `_config.yml`

## Tips

- No necesitás instalar nada en tu máquina — GitHub hace el build de Jekyll
- Para editar desde el navegador: abrí tu repo y apretá `.` para abrir GitHub.dev
- Los posts se ordenan automáticamente por fecha (más reciente primero)
- Markdown soporta código, ecuaciones, imágenes, tablas y más
