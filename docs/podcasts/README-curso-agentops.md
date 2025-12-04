# Curso AgentOps – Guía rápida para alumnos

Este documento acompaña al episodio del podcast **“El salto de DevOps a la Orquestación Cognitiva”** (`AgentOps_El_Salto_de_DevOps_a_la_Orquestación_Cognitiva.m4a`) y sirve como guía práctica del curso:

> **AgentOps: Orquestación Cognitiva de Agentes de IA en Ciclos de Desarrollo de Software**

El programa completo y oficial del curso está aquí:

- Programa detallado: `docs/curso-agentops.md` (versión web en `https://sinensia.github.io/curso-agentops/`)

Aquí encontrarás una versión resumida pensada para compartir con alumnos.

---

## 1. Visión general del curso

AgentOps es la evolución natural de DevOps: en lugar de automatizar solo *pipelines*, aprendemos a **orquestar recursos cognitivos**, es decir, agentes de IA capaces de pensar, razonar y colaborar dentro del ciclo de vida del software.

Al final del curso habrás construido un **proyecto real de principio a fin**, integrando:

- Diseño dirigido por especificaciones y agentes.
- Desarrollo y tests asistidos por agentes.
- CI/CD cognitivo.
- Orquestación de tareas con n8n y protocolos como MCP.
- Memoria agentic (grafo + RAG).
- Observabilidad de agentes y despliegue final.

---

## 2. Requisitos y entorno

Perfil recomendado:

- Ingenieros de software, DevOps, MLOps, SecOps, arquitectos y equipos de innovación.
- Experiencia previa con Git y GitHub.
- Manejo básico de Docker/Docker Desktop.
- Python o NodeJS a nivel intermedio (lectura y pequeñas adaptaciones).

Herramientas que usaremos (algunas en modalidad gratuita):

- GitHub (repos y GitHub Actions).
- OpenAI API (o proveedor equivalente).
- Figma (para parte de diseño).
- Neo4j AuraDB (Graphiti).
- Cloudflare (Workers / despliegues ligeros).
- n8n, SonarQube, LangGraph / LangSmith / LangFuse, etc.

Los repositorios concretos y plantillas se comparten durante el curso, vinculados a cada bloque práctico.

---

## 3. Mapa de bloques (lo que vas a construir)

El curso se estructura en grandes bloques temáticos, cada uno con un hito práctico:

| Bloque | Qué trabajas | Hito principal |
| --- | --- | --- |
| **1. Diseño Cognitivo** | Introducción a AgentOps y *Spec-Driven Development* con GitHub Spec-Kit y Figma MCP. | Repositorio inicial generado por agente. |
| **2. Seguridad Asistida** | *Security-by-Design* guiado por LLM; checklist OWASP y validaciones. | Documento de requisitos de seguridad. |
| **3. Desarrollo Agentic** | Agente desarrollador (Codex/LLM), herramientas como Serena/Chrome DevTools, Playwright Agents. | Funcionalidad mínima + primeros tests generados por agentes. |
| **4. CI/CD Cognitivo** | GitHub Actions, ghcr.io, SonarQube, SAST/DAST aumentados por IA, PR review automática. | Pipeline que construye, testea y analiza seguridad. |
| **5. Orquestación Operativa** | n8n como columna vertebral, MCP / A2A / ACP, flujos *human-in-the-loop*. | Flujo n8n que reacciona a un push y dispara agentes. |
| **6. Memoria Agentic y RAG** | Graphiti + Neo4j como memoria viva, LangChain + Graphiti. | Agente que responde con contexto desde el grafo. |
| **7. Observabilidad** | LangGraph / LangSmith / LangFuse para trazas, costes y *replay*. | Dashboard de observabilidad con runs reales. |
| **8. Despliegue** | Dockerización, despliegue ligero (Cloudflare Workers / Replit), gestión de secretos y costes. | Demo end‑to‑end funcionando. |

Cada bloque combina una breve introducción conceptual con laboratorio guiado.

---

## 4. Relación con el podcast

El episodio **“El salto de DevOps a la Orquestación Cognitiva”** resume las ideas clave del curso:

- Por qué AgentOps es un siguiente paso natural a DevOps.
- Qué significa orquestar **agentes** en lugar de solo contenedores o jobs.
- Ejemplos de flujos donde varios agentes colaboran (codificación, testing, seguridad, despliegue…).
- Cómo encajan herramientas como MCP, n8n o Graphiti en este nuevo modelo.

Para aprovechar mejor el episodio:

1. Ten a mano este README y el programa detallado (`docs/curso-agentops.md`).
2. Fíjate en qué bloque del curso se alinea con cada parte del audio.
3. Anota dudas o ideas de automatización que quieras explorar en los laboratorios.

---

## 5. Cómo estudiar y sacarle partido

- **No te quedes en la demo**: adapta los ejemplos a un proyecto tuyo (real o simulado).
- **Crea tus propios agentes**: en cada bloque, intenta añadir al menos una tool o flujo nuevo.
- **Itera sobre la seguridad**: usa los agentes no solo para escribir código, también para revisar arquitectura y riesgos.
- **Piensa en el pipeline completo**: diseña tus agentes como si fueran miembros del equipo DevOps.

Al finalizar, tendrás una arquitectura de referencia y un conjunto de patrones reutilizables para aplicar AgentOps en tus propios proyectos.

