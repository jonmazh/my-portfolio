---
title: "LC 2. Día 2: HashMaps en Profundidad y Linked Lists"
description: "Segunda jornada del bootcamp: 8 problemas resueltos entre Maps y Linked Lists, patrones clave de HashMap y técnicas de manipulación de listas enlazadas."
pubDate: 2026-03-10
updatedDate: 2026-03-10
heroImage: ../../assets/leetCodeIcon.png
author: jonmh
tags:
  - java
  - leetcode
  - algorithms
  - learning
---

Segundo día del bootcamp y el volumen sube. Hoy el foco ha estado en dos áreas que van a aparecer sí o sí en cualquier evaluación técnica: **HashMaps** y **Linked Lists**. 8 problemas resueltos, varios de ellos Medium.

El repo con todos los problemas resueltos está en: [jonmazh/leetcode-grind](https://github.com/jonmazh/leetcode-grind).

### 1. HashMaps en Profundidad

Si ayer el HashMap apareció como herramienta para Two Sum, hoy es el protagonista. Los problemas del bloque `maps/`:

**Group Anagram**, **Isomorphic Strings**, **Longest Consecutive Sequence**, **Top K Frequent Elements**, **Word Pattern**, **LRU Cache**.

Los aprendizajes importantes del bloque:

- **Group Anagram**: El truco es usar un array de 26 enteros como clave del mapa (frecuencia de letras), en vez de ordenar el string. `Arrays.toString(count)` convierte ese array en una clave válida para el HashMap. Más eficiente que la versión con `Arrays.sort()`.
- **Longest Consecutive Sequence**: La solución O(n log n) con ordenación es intuitiva, pero la O(n) con HashSet es la que piden. La clave: solo empiezas a contar desde un número si `n-1` no está en el set. Así cada secuencia se recorre una sola vez.
- **Top K Frequent Elements**: Dos enfoques válidos — `PriorityQueue` (min-heap de tamaño k) o **bucket sort** por frecuencia. El bucket sort es O(n) y evita el heap, pero requiere pensar en frecuencia como índice del array.
- **LRU Cache**: El problema más exigente del día. La solución óptima combina `HashMap` con una **doubly linked list** para conseguir O(1) en `get` y `put`. En Java, `LinkedHashMap` con `accessOrder=true` lo da casi gratis, pero entender la implementación manual es lo que importa.

El patrón del día en maps: **cuando necesitas agrupar o contar, piensa primero en qué usas como clave**.

### 2. Linked Lists

Dos problemas clásicos que cubren los patrones fundamentales de listas enlazadas:

**Merge Two Sorted Lists**, **Reverse Linked List**.

- **Merge Two Sorted Lists**: El enfoque iterativo con un nodo dummy es más limpio que el recursivo. Se avanza comparando cabezas de ambas listas y encadenando el menor. El nodo dummy elimina el caso especial del primer nodo.
- **Reverse Linked List** (`rvrsLL`): Patrón de tres punteros — `prev`, `curr`, `next`. Se itera una sola vez invirtiendo los punteros sobre la marcha. El patrón aparece en variaciones más complejas (reverse in groups, reverse between positions), así que vale la pena interiorizar el movimiento.

### Estado del bootcamp

Quedan 3 días. La evaluación puede llegar en cualquier momento del día 4 o 5. El ritmo es sostenible por ahora, pero los problemas Medium empiezan a pedir más tiempo de lo esperado en algunos casos.

> "El LRU Cache es uno de esos problemas que cuando lo entiendes de verdad, entiendes por qué importan las estructuras de datos."

**Progreso del día:** 8 problemas resueltos (Maps + Linked Lists) · Patrones vistos: HashMap como agrupador, Bucket Sort, Two Pointers en LL, Dummy Node. Mañana: Binary Search y Trees.