---
layout: default
title: "Curso Model Context Protocol (MCP)"
permalink: /curso-mcp/
description: Programa del curso Model Context Protocol (MCP) de Sinensia IT Solutions
---

# 🧩 Curso Model Context Protocol (MCP)

Duración total: **16 horas**.

Este curso introduce MCP como el “USB-C para la IA”: un estándar para conectar modelos con herramientas, datos y servicios externos de forma segura y observable.

Guía rápida y mapa de ejercicios prácticos: `docs/podcasts/README-curso-mcp.md` (en este mismo repositorio) y código de los laboratorios en `https://github.com/scops/curso-mcp`.

---

## Estructura del curso (módulos)

### Módulo 1

- Tema técnico: Aislamiento de los LLMs, problema N × M, visión general de MCP como "USB-C para la IA".
- Enfoque práctico: Debate sobre casos reales donde un asistente necesita acceso a datos externos.

### Módulo 2

- Tema técnico: Host, cliente MCP, servidor MCP, transporte JSON-RPC/STDIO-HTTP.
- Beneficio pedagógico: Ver el flujo solicitud/respuesta y la simplicidad del protocolo.

### Módulo 3

- Tema técnico: SDKs oficiales, instalación, herramientas de inspección.
- Enfoque práctico: Ejecutar la primera petición MCP con la CLI.

### Módulo 4

- Tema técnico: Diferencia entre tools y resources; diseño.
- Beneficio pedagógico: Primer contacto con IO real y manejo de errores.

### Módulo 5

- Tema técnico: Prompting, tamaño de contexto, iteración IA-herramienta.
- Enfoque práctico: Simular la decisión del LLM y verificar la respuesta.

### Módulo 6

- Tema técnico: Integrar un LLM (API o local) para categorizar archivos mediante las herramientas MCP.
- Beneficio pedagógico: Ver en acción la sinergia IA + protocolo estándar.

### Módulo 7

- Tema técnico: Buenas prácticas y seguridad; límite de permisos, validación de rutas, gestión de errores y logs.
- Enfoque práctico: Simular ataques (lectura de ruta prohibida) y comprobar defensas.

### Módulo 8

- Tema técnico: Integraciones en pipelines con LangChain y evolución futura de MCP.
- Beneficio pedagógico: Entender cómo encajar MCP en arquitecturas modernas de agentes y proyectar su evolución en el ecosistema.
