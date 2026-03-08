---
title: "Fundamentos de JavaScript: Variables y Strings en FreeCodeCamp"
description: "Resumen de mi aprendizaje de hoy repasando los pilares de JS a través de la plataforma FreeCodeCamp."
pubDate: 2026-03-07
updatedDate: 2026-03-07
heroImage: ../../assets/blog-placeholder-2.png
author: jonmh
tags:
  - javascript
  - learning
  - freecodecamp
---

Hoy he dedicado la sesión de estudio a consolidar los cimientos de **JavaScript** mediante los desafíos de FreeCodeCamp. Aunque parecen conceptos básicos, entender cómo el motor de JS maneja la memoria y las cadenas de texto es vital para evitar bugs en el futuro.

Todo este proceso y mis notas detalladas las estoy centralizando en mi repositorio de GitHub: [jonmazh/fcc-javascript-notes](https://github.com/jonmazh/fcc-javascript-notes).

### 1. Gestión de Variables: var, let y const
Uno de los puntos clave del repaso ha sido la diferencia de *scope* y la mutabilidad.
- **`const`**: Para valores que no deben cambiar. Es mi opción por defecto para mantener el código predecible.
- **`let`**: Cuando necesito reasignar valores (como en contadores de bucles).
- **`var`**: Un vistazo al pasado. Entender por qué ya no se recomienda debido al *hoisting* y al ámbito de función vs. ámbito de bloque.

### 2. Manipulación de Strings
JavaScript ofrece una versatilidad increíble para trabajar con texto. He profundizado en:
- **Concatenación vs. Template Literals**: Cómo las *backticks* (`` ` ``) hacen que el código sea mucho más legible al interpolar variables.
- **Inmutabilidad**: Recordar que no puedes cambiar un carácter individual de un string mediante su índice; hay que reasignar la variable completa.
- **Métodos esenciales**: Uso de `.length` y acceso a caracteres mediante corchetes `[]`.

### Reflexión del día
Como estudiante de **Ingeniería Informática (GII + GIS)**, a veces tendemos a querer saltar directamente a la arquitectura compleja. Sin embargo, este repaso en FreeCodeCamp me recuerda que la elegancia de un sistema nace de entender perfectamente sus piezas más pequeñas.

> "La programación no se trata de lo que sabes; se trata de lo que puedes descifrar."

Seguiré actualizando mis notas en el repositorio a medida que avance en los módulos de estructuras de datos y algoritmos.