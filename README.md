# Software Engineer — Edición esencial en español

Manual de estudio estático (sin build, sin dependencias) para recorrer la carrera de ingeniería de software con criterio.
Alineado temáticamente con *The Software Engineer's Guidebook*, de Gergely Orosz, pero con texto y diagramas originales.

## Qué incluye

- **108 páginas** en **27 módulos** (3 lecciones y 1 evaluación por módulo).
- Lectura continua: botón «Completar y seguir», navegación con ← y →, temario lateral siempre disponible.
- **27 evaluaciones** de 3 preguntas con explicaciones y **81 ejercicios** aplicados.
- Progreso guardado en `localStorage`, glosario con buscador y modo claro/oscuro.
- Buscador global con atajo `⌘K` / `Ctrl+K`.
- **81 diagramas originales** en SVG.
- Manual en PDF: `Software-Engineer-Esencial.pdf`.
- Tipografías locales (Fraunces + Inter), sin depender de Google Fonts.

## Estructura

```
index.html                 Portada y temario completo
se1l1.html … se27q.html      Lecciones y evaluaciones
glosario.html              Glosario con búsqueda
progreso.html              Progreso por módulo
css/curso.css              Diseño editorial responsive
js/curso.js                Navegación, progreso, búsqueda y quizzes
assets/fonts/              Tipografías locales
Software-Engineer-Esencial.pdf
```

## Ver en línea

- Sitio: https://joelelizalde.github.io/software-engineer-esencial/
- Repositorio: https://github.com/joelelizalde/software-engineer-esencial
- PDF: https://raw.githubusercontent.com/joelelizalde/software-engineer-esencial/main/Software-Engineer-Esencial.pdf

## Publicar en GitHub Pages

El sitio se publica desde la rama `main`, carpeta raíz. Para actualizarlo:

```bash
cd software-engineer-esencial
git add .
git commit -m "Actualiza el manual"
git push origin main
```

Para publicarlo desde cero en otra cuenta: **Settings → Pages → Deploy from a branch → main → / (root)**.

## Regenerar

```bash
python3 build_site.py          # solo el sitio
python3 build_site.py --pdf    # sitio + manual en PDF
```

El PDF se compone con WeasyPrint a partir del mismo contenido.

## Atajos

| Tecla | Acción |
|---|---|
| `←` / `→` | Lección anterior / siguiente |
| `C` | Marcar la lección actual como completada |
| `/` o `⌘K` | Abrir el buscador |
| `Esc` | Cerrar buscador o menú |
| `?` | Recordatorio de atajos |

## Créditos

Manual original de estudio en español, alineado con los temas de *The Software Engineer's Guidebook*, de Gergely Orosz.
No reproduce el texto ni las figuras del libro. Uso educativo.
