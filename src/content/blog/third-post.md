---
title: "LC 1. Día 1: Java Reset y Primeros Problemas en LeetCode"
description: "Primera jornada de bootcamp intensivo: configuración del entorno, crash course de Java y 10 problemas Easy resueltos."
pubDate: 2026-03-09
updatedDate: 2026-03-09
heroImage: ../../assets/leetCodeIcon.png
author: jonmh
tags:
  - java
  - leetcode
  - algorithms
  - learning
---

Hoy ha arrancado el bootcamp más intenso que me he propuesto: 5 días para preparar una evaluación técnica para una pasantía de ingeniería de software. El objetivo es enviar la evaluación en el día 4 o 5, dedicando el máximo de horas posibles cada día. Sin red de seguridad, sin experiencia previa en LeetCode.

El repo con todos los problemas resueltos está en: [jonmazh/leetcode-grind](https://github.com/jonmazh/leetcode-grind).

### 1. Configuración del Entorno

Antes de escribir una sola línea de algoritmo, toca montar la base. He creado un proyecto Java en IntelliJ con la estructura de carpetas por tema (`arrays/`, `hashmaps/`, `trees/`...) y un template de clase con `main()` para probar soluciones localmente antes de subirlas a LeetCode.

El flujo de trabajo es: pensar en papel → codificar en IntelliJ → probar con `main()` → copiar solo la función a LeetCode → submit.

### 2. Java Crash Course

Java lleva tiempo oxidado, así que antes de los problemas toca recuperar exactamente lo que necesitas para LeetCode — nada más. Las estructuras críticas:

- **HashMap**: El patrón `getOrDefault` para contadores y búsquedas en O(1).
- **PriorityQueue**: Min-heap por defecto, max-heap con `(a, b) -> b - a`.
- **ArrayDeque**: Reemplaza a `Stack` (obsoleta) para pilas y colas.
- **StringBuilder**: Nunca concatenar Strings en un loop.
- **Comparator con lambdas**: `(a, b) -> a[0] - b[0]` en vez de la clase anónima verbosa.

La clave es escribirlo todo sin ayuda del autocompletado. La evaluación no tiene IDE hints.

### 3. Primeros 10 Problemas Easy

La primera toma de contacto real con LeetCode. Los problemas del día:

Two Sum, Reverse String, Valid Anagram, Best Time to Buy/Sell Stock, Contains Duplicate, Maximum Subarray, Move Zeroes, Plus One, Single Number, Palindrome Number.

Dos aprendizajes importantes del día:

- **Two Sum**: Mi primera solución fue O(n²) con doble bucle — funciona pero solo bate al 27%. La versión con HashMap lo resuelve en O(n) con un único pase.
- **Reverse String**: El truco es que la función es `void` — no devuelves nada, modificas el array en sitio con two pointers. Primer patrón de two pointers del bootcamp.

### Reglas del bootcamp que me estoy poniendo

Después del primer día ya hay cosas que quedan claras:

- **Easy sin resolver en 30 min** → miras la solución, la entiendes, la escribes de memoria, sigues.
- **Medium sin resolver en 45 min** → igual.
- **No usar IA para soluciones** mientras puedas razonarlo tú. El aprendizaje está en el bloqueo, no en la solución rápida.
- **Practicar también en LeetCode directamente**, sin IntelliJ, para acostumbrarse al editor básico de la evaluación real.

> "No necesitas resolver todos los problemas perfectamente. Necesitas demostrar proceso de pensamiento."

**Progreso del día:** 10 problemas Easy resueltos · Patrones vistos: Two Pointers, HashMap O(n). Mañana: HashMaps en profundidad, Linked Lists y Binary Search.