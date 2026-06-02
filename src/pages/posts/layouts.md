---
title: "Layouts en Astro"
date: 2026-04-20
description: "Cómo usar layouts para organizar tus páginas en Astro"


---

# Layouts en Astro

Un **layout** es como una plantilla que se usa para dar formato a varias páginas. Así no tienes que repetir el mismo código (por ejemplo, el menú de navegación o el footer) en cada archivo.

## Ejemplo básico de un layout

Crea un archivo en `src/layouts/BaseLayout.astro`:


```astro
---
const { pageTitle } = Astro.props;
---

<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <title>{pageTitle}</title>
  </head>
  <body class="bg-gray-100 text-black">
    <header class="p-4 bg-green-200">
      <h1 class="text-2xl font-bold">{pageTitle}</h1>
      