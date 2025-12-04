# Curso Model Context Protocol (MCP)

Este documento acompaña al episodio del podcast **“MCP: el USB para orquestar la IA”** (`MCP_el_USB_para_orquestar_la_IA.m4a`) y sirve como guía rápida para el **Curso Model Context Protocol (MCP)** y sus ejercicios prácticos.

El código del curso está en el repositorio:

- Repositorio de ejercicios: https://github.com/scops/curso-mcp

Cada carpeta del repo incluye su propio `README.md` con instrucciones detalladas. Aquí tienes solo el mapa general y cómo preparar el entorno.

---

## 1. Preparar el entorno

1. Clona el repositorio del curso:
   ```bash
   git clone https://github.com/scops/curso-mcp.git
   cd curso-mcp
   ```
2. Instala **uv** (solo una vez):
   - macOS / Linux:
     ```bash
     curl -LsSf https://astral.sh/uv/install.sh | sh
     ```
   - Windows (PowerShell):
     ```powershell
     irm https://astral.sh/uv/install.ps1 | iex
     ```
3. Sincroniza dependencias y crea el entorno virtual compartido:
   ```bash
   uv sync
   ```
4. Crea un fichero `.env` en la raíz del repo con tus claves y credenciales (OpenAI, Anthropic, OMDb, sakila, etc.), según se pide en los distintos ejercicios.

A partir de aquí, ejecuta siempre los ejemplos con `uv run ...` desde la raíz del repo.

---

## 2. Mapa de ejercicios del curso

En la carpeta `mcp/` del repo encontrarás los ejercicios numerados. De forma resumida:

| Carpeta | Ejercicios | Qué construyes | Qué practicas en MCP |
| --- | --- | --- | --- |
| `ej1_first_chatbot/` | Ejercicio 1 | Cliente + servidor MCP mínimo por STDIO. | Tools sencillas, estado cliente/servidor, tests básicos. |
| `ej2_4_chatbot_arxiv/` | Ejercicios 2–4 | Chatbot arXiv (sin MCP, con MCP y cliente OpenAI). | Diseño de tools reales, prompts MCP reutilizables, `ClientSession`. |
| `ej5_6_chatbot_omdb/` | Ejercicios 5–6 | Servidor MCP HTTP (OMDb) + cliente Streamlit/Inspector. | `streamable-http`, acceso a APIs externas vía MCP. |
| `ej7_mcp_rag_db/` | Ejercicio 7 | RAG sobre incidencias + servidor MCP con resources y memoria. | Resources, memoria persistente, feedback. |
| `ej8_sakila_streaming/` | Ejercicio 8 | Agente “plataforma de streaming” (sakila + OMDb). | Lectura/escritura en BD, coordinación de varios servidores. |
| `ej9_orquestador/` | Ejercicio 9 | Servidor MCP orquestador que llama a otros MCP. | Orquestación MCP→MCP y tools de alto nivel. |
| `ej10_reto/` | Ejercicio 10 | Reto final: servidor MCP propio. | Diseño completo de un servidor MCP para una API elegida. |

En cada carpeta encontrarás un `README.md` con los pasos detallados, objetivos y mini‑ejercicios.

---

## 3. Relación con el podcast “MCP: el USB para orquestar la IA”

En el episodio del podcast asociado a este documento comentamos:

- La idea de MCP como “USB” o estándar para conectar modelos con tools, datos y servicios.
- Cómo un único cliente (el LLM / agente) puede hablar con múltiples servidores MCP.
- Ejemplos de orquestación entre servidores (como en `ej8_sakila_streaming/` y `ej9_orquestador/`).
- Buenas prácticas para diseñar tools útiles y auto‑descubribles para el modelo.

Si quieres seguir el curso mientras escuchas el episodio:

1. Ten abierto el repo `curso-mcp` en tu editor.
2. Revisa el mapa de ejercicios (sección anterior).
3. Ve abriendo los `README.md` de cada carpeta según vayan saliendo ejemplos en el podcast.

---

## 4. Cómo estudiar y practicar

- Empieza por `ej1_first_chatbot/` para entender la estructura mínima de un servidor MCP.
- Avanza por orden: cada bloque reutiliza conceptos del anterior y añade uno nuevo (HTTP, resources, RAG, orquestación…).
- Intenta siempre añadir **al menos una tool propia** en cada ejercicio.
- Usa MCP Inspector y clientes alternativos (cuando se proponga) para probar tus servidores MCP.

Cuando termines, el reto final (`ej10_reto/`) consiste en diseñar tu propio servidor MCP sobre una API o dominio que te interese, aprovechando todos los patrones de los ejercicios anteriores.

---

## 5. Tests y verificación

El repo incluye tests para muchos de los ejercicios. Desde la raíz:

```bash
uv run python -m unittest
```

También puedes lanzar tests por ejercicio (explicado en el `README.md` principal del repo). Esto te ayudará a comprobar que tus soluciones son correctas y a experimentar con cambios de forma segura.

