---
title: "Fundamentos Básicos de Astro"
date: 2026-04-23
description: "Conceptos esenciales para entender cómo funciona Astro"
---

# Fundamentos Básicos de Astro

Astro es un framework moderno para construir sitios web estáticos y dinámicos, optimizado para velocidad y simplicidad. Sus fundamentos básicos son los siguientes:

## 1. Filosofía de Astro
- **Menos JavaScript en el cliente**: Astro envía HTML estático por defecto, reduciendo el peso de la página.
- **Islas de interactividad**: Solo los componentes que necesitan JavaScript lo reciben, el resto es HTML puro.
- **Compatibilidad universal**: Puedes usar React, Vue, Svelte, Solid y otros frameworks dentro de Astro.

## 2. Estructura de un proyecto
- `src/pages/` → Cada archivo `.astro` aquí se convierte en una ruta de tu sitio.
- `src/layouts/` → Plantillas reutilizables para dar formato a varias páginas.
- `src/components/` → Elementos pequeños y reutilizables (ejemplo: navegación, footer).
- `public/` → Archivos estáticos como imágenes, íconos o fuentes.

## 3. Sintaxis de archivos `.astro`
Un archivo `.astro` combina **HTML + JavaScript + CSS** en un solo lugar:

```astro
---
const nombre = "Astro";
---

<html>
  <body>
    <h1>Bienvenido a {nombre}</h1>
    <p>Este es un ejemplo básico de sintaxis en Astro.</p>
  </body>
</html>
