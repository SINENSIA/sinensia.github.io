# Sinensia AgentOps

Sitio estático publicado en [sinensia.github.io](https://sinensia.github.io) usando GitHub Pages y el tema Jekyll [Cayman](https://github.com/pages-themes/cayman). Aquí documentamos el curso **AgentOps: Orquestación Cognitiva de Agentes de IA** y compartimos recursos multimedia.

## Requisitos locales

- Ruby 3.x con cabeceras (`ruby-dev` o equivalente) y `bundler`
- NodeJS opcional para soporte de `execjs`

## Puesta en marcha

```bash
bundle install
bundle exec jekyll serve
```

El comando anterior deja el sitio disponible en `http://127.0.0.1:4000` con *live reload*.

## Estructura

- `index.md`: portada con resumen del programa y enlaces rápidos.
- `docs/curso-agentops.md`: temario completo del curso (incluye reproductor del podcast).
- `docs/podcasts/`: recursos de audio servidos como estáticos.

Las contribuciones pueden hacerse mediante *pull requests*. Añade nuevos contenidos dentro de `docs/` y enlázalos desde la portada.
