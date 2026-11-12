# David Feng Wu | Portafolio Full Stack

Portafolio personal de proyectos web, aplicaciones móviles, APIs y conectores MCP. Desarrollado con HTML, CSS y JavaScript, con contenido en español e inglés.

**Dirección de GitHub Pages:** [thedavidfw.github.io](https://thedavidfw.github.io/)

## Proyectos

| Proyecto | Descripción | Tecnologías principales | Sitio |
| --- | --- | --- | --- |
| Radiadores THT | Sitio corporativo, catálogo autenticado y administración de productos, clientes y accesos. | React, Vite, FastAPI, Supabase, Cloudinary, Docker, Oracle Cloud y Caddy. | [radiadorestht.com](https://www.radiadorestht.com/) |
| FitChat MCP | Conector remoto para consultar datos deportivos de Garmin y Strava desde asistentes compatibles con MCP. | React, TypeScript, Node.js, MCP y Supabase. | [fitchat-mcp.com](https://www.fitchat-mcp.com/) |
| Outfit Planner App | Aplicación móvil para gestionar prendas, crear conjuntos y planificar el calendario. | React Native, Expo, TypeScript y Stripe. | — |
| Outfit Planner Web | Aplicación web con autenticación, panel, perfil y membresías. | React, Vite, Tailwind CSS y Axios. | — |
| Outfit Planner API | Backend para usuarios, prendas, conjuntos, suscripciones y procesamiento de imágenes. | FastAPI, PostgreSQL, SQLAlchemy, Docker, Stripe y Cloudinary. | — |

## Funciones

- Selector ES/EN en el encabezado, con preferencia guardada en `localStorage`.
- Detección del idioma del navegador cuando no existe una selección guardada.
- Traducción de navegación, descripciones, fichas y vistas previas.
- Filtros por web, API, móvil y conectores.
- Vista detallada de cada proyecto y enlaces a los sitios publicados.
- Diseño adaptable, animación de escritura y transiciones al desplazarse.
- Compatibilidad con la preferencia de movimiento reducido del sistema.

Las vistas previas son representaciones resumidas de los proyectos; los enlaces externos abren sus sitios publicados.

## Estructura

```text
.
|-- index.html
|-- README.md
`-- assets/
    |-- i18n.js
    |-- fitchat-mcp-logo.svg
    |-- outfitplanner-armario.webp
    |-- outfitplanner-logo.png
    `-- radiadores-logo.png
```

- `index.html`: estructura, estilos, datos de proyectos y lógica de interacción.
- `assets/i18n.js`: traducciones al español, selección inicial del idioma y funciones de traducción.
- `assets/`: imágenes y logotipos utilizados por el portafolio.

## Abrir en local

Abre `index.html` directamente en el navegador. No requiere instalar dependencias, compilar ni iniciar un servidor.

La fuente JetBrains Mono se carga desde Google Fonts. Sin conexión se utiliza la fuente monoespaciada alternativa del sistema.

## Actualizar contenido

### Proyectos

Edita el arreglo `projects` en `index.html`. Cada entrada contiene el nombre, categoría, descripción, tecnologías, características y metadatos del proyecto.

Para un proyecto publicado, configura `url` y `website`; estos campos muestran su enlace en la ficha. Las vistas previas se definen en las funciones `preview...` y se seleccionan mediante `renderPreview`.


### Estilos e imágenes

Los estilos están en el bloque `<style>` de `index.html`. Las variables de color, tipografía y bordes están en `:root`. Guarda nuevas imágenes en `assets/` y utiliza rutas relativas.

## GitHub Pages

El repositorio contiene un sitio estático listo para GitHub Pages. Para publicarlo desde una rama:

1. Sube `index.html`, `assets/` y `README.md` al repositorio.
2. En **Settings > Pages**, selecciona **Deploy from a branch**.
3. Selecciona la rama `main` y la carpeta raíz `/ (root)`.
4. Guarda la configuración y consulta el estado del despliegue en GitHub.

Mantén `index.html` en la raíz para que sea la página de entrada. La publicación depende de la configuración de GitHub Pages del repositorio.
