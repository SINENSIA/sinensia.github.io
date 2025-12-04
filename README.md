# Sinensia – Cursos y recursos AgentOps / MCP

Sitio estático publicado en [sinensia.github.io](https://sinensia.github.io) usando GitHub Pages y el tema Jekyll [Cayman](https://github.com/pages-themes/cayman). Aquí documentamos el curso **AgentOps: Orquestación Cognitiva de Agentes de IA**, el **Curso Model Context Protocol (MCP)** y compartimos recursos multimedia.

## Cursos principales

- **AgentOps: Orquestación Cognitiva de Agentes de IA**
  - Programa completo: `docs/curso-agentops.md` (web: `https://sinensia.github.io/curso-agentops/`)
  - Podcast asociado: `docs/podcasts/AgentOps_El_Salto_de_DevOps_a_la_Orquestación_Cognitiva.m4a`
  - Guía rápida para alumnos: `docs/podcasts/README-curso-agentops.md`

- **Curso Model Context Protocol (MCP)**
  - Repositorio de ejercicios: `../mcp/` (GitHub: `https://github.com/scops/curso-mcp`)
  - Podcast asociado: `docs/podcasts/MCP_el_USB_para_orquestar_la_IA.m4a`
  - Guía rápida para alumnos: `docs/podcasts/README-curso-mcp.md`

## Requisitos locales (para trabajar con este sitio)

- Ruby 3.x con cabeceras (`ruby-dev` o equivalente) y `bundler`
- NodeJS opcional para soporte de `execjs`

## Puesta en marcha del sitio

```bash
bundle install
bundle exec jekyll serve
```

El comando anterior deja el sitio disponible en `http://127.0.0.1:4000` con *live reload*.

## Estructura del sitio

- `index.md`: portada con resumen del programa AgentOps y enlaces rápidos.
- `docs/curso-agentops.md`: temario completo del curso AgentOps (incluye reproductor del podcast).
- `docs/podcasts/`: recursos de audio servidos como estáticos y guías rápidas de cursos (AgentOps, MCP).

Las contribuciones pueden hacerse mediante *pull requests*. Añade nuevos contenidos dentro de `docs/` y enlázalos desde la portada.
