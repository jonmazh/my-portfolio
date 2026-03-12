---
title: "LC 3. Día 3: UADE, Primer Clase de Ingeniería del Software y Binary Search"
description: "Tercer jornada del bootcamp: primer día en la universidad, formación de equipo para los TPOs y problemas de Binary Search en LeetCode."
pubDate: 2026-03-11
updatedDate: 2026-03-11
heroImage: ../../assets/leetCodeIcon.png
author: jonmh
tags:
  - java
  - leetcode
  - algorithms
  - learning
  - uade
---

Día distinto. La mañana no fue de leetcode sino de universidad: primer día de **Ingeniería del Software** en la UADE. La tarde intentó ser productiva, pero el cansancio tuvo más que decir que yo.

El repo con todos los problemas resueltos está en: [jonmazh/leetcode-grind](https://github.com/jonmazh/leetcode-grind).

### 1. Ingeniería del Software — Primera Clase

La mañana arrancó temprano con el primer encuentro de la materia. La clase sirvió principalmente para romper el hielo: repaso del programa, metodologías que vamos a ver durante el cuatrimestre y una primera lectura del tipo de trabajos que hay que entregar.

Lo más importante del día en la facultad fue **armar el equipo**. Coincidí con tres chicos argentinos y quedamos juntos para los TPOs. Buena onda desde el principio, que ya es mucho. El trabajo grupal en esta materia va a ser una parte importante de la nota, así que empezar con buen pie con el equipo no es menor.

La dinámica de la clase fue bastante accesible para ser el primer día. No se entró en profundidad técnica todavía, pero quedó claro el volumen de trabajo que viene.

### 2. Binary Search — Los Clásicos

Por la tarde, de vuelta al grind. El bloque de hoy: **Binary Search**. Dos problemas del núcleo duro de este patrón:

**Binary Search clásico**, **Search in Rotated Sorted Array**.

- **Binary Search clásico**: La base. El truco que siempre hay que recordar es el cálculo del `mid` para evitar overflow: `mid = left + (right - left) / 2` en vez de `(left + right) / 2`. El resto es condición de parada y ajuste de punteros. Más fácil de codear que de explicar sin errores de índice.

- **Search in Rotated Sorted Array**: Aquí la cosa se complica. El array está ordenado pero rotado en algún punto desconocido, y hay que encontrar el target en O(log n). La clave es darse cuenta de que **siempre hay una mitad del array que está completamente ordenada**. Identificar cuál es esa mitad y decidir si el target cae dentro de ella es lo que define hacia dónde mover los punteros.

El patrón del día en Binary Search: **no buscas el target directamente, sino que en cada iteración determinas en qué mitad puede estar**.

### 3. La tarde se torció

Intenté continuar con más problemas. Los siguientes en la lista eran **Find Peak Element** y **Find Minimum in Rotated Sorted Array**, pero el cansancio acumulado de madrugar para la facultad cobró factura. La concentración no daba.

Cambié de registro y aproveché para trabajar en el perfil de LinkedIn: optimización de secciones, búsqueda de empresas que me parecen interesantes de cara al futuro, y un repaso general de cómo está quedando el perfil. Trabajo menos exigente cognitivamente, pero igual necesario.

Find Peak Element y Find Minimum in Rotated Sorted Array quedan pendientes para mañana con la cabeza fresca. No tiene sentido forzar Binary Search con niebla mental, es exactamente el tipo de problema donde un detalle de índice mal puesto te hace perder 40 minutos.

Temprano a la cama. Mañana hay que madrugar otra vez.

### Estado del bootcamp

Día irregular pero con dos frentes abiertos: la universidad empieza a rodar y el grind de algoritmos avanza, aunque más despacio de lo que me gustaría. El equipo en la UADE es una buena noticia.

> "Hay días que el mejor movimiento es parar, hacer algo útil pero ligero, y guardar energía para mañana."

**Progreso del día:** 2 problemas resueltos (Binary Search) · Patrones vistos: Binary Search clásico, Rotated Array Search · Pendientes: Find Peak Element, Find Minimum in Rotated Sorted Array · Universidad: equipo formado para TPOs de Ingeniería del Software.