# Cambios a Aplicar: Unidad 01 Teórica

**Fecha:** 2026-02-04  
**Archivo a modificar:** `Teórica/Unidad 01 Teórica.docx`  
**Basado en:** `Informes/Informe_Unidad01.md`

---

## Instrucciones de uso

Este documento contiene el texto a **agregar o modificar** en la guía teórica de Unidad 01. Cada cambio indica:
- **Ubicación exacta** en el documento original
- **Texto a insertar** (listo para copiar y pegar)
- **Prioridad** del cambio

---

## CAMBIO #1 — Prioridad: ALTA

### Agregar definición formal de "valor" y "tipo de valor"

**Ubicación:** Después del párrafo que dice *"A los valores que van dentro de los paréntesis los llamamos argumentos..."* y ANTES de *"En principio vamos a trabajar con dos Tipos de Valores..."*

**Texto a insertar:**

---

> ### ¿Qué es un valor?
> 
> Un **valor** es un dato concreto que usamos en nuestros programas. Por ejemplo, `Norte`, `Azul`, `3` son todos valores. Los valores representan información que el programa puede manipular.
> 
> Los valores se agrupan en **tipos de valores**. Un tipo de valor es una categoría que agrupa valores que comparten características similares. Por ejemplo:
> - El tipo **Direcciones** agrupa los valores: `Norte`, `Este`, `Sur`, `Oeste`
> - El tipo **Colores** agrupa los valores: `Azul`, `Negro`, `Rojo`, `Verde`
> 
> Cada comando espera recibir argumentos de un tipo específico. Por eso `Mover(Norte)` funciona (Norte es una Dirección), pero `Mover(Azul)` falla (Azul es un Color, no una Dirección). Esto se llama **error de tipo**: cuando pasamos un valor de un tipo incorrecto.

---

## CAMBIO #2 — Prioridad: ALTA

### Agregar comando `Sacar` y conceptos de operación total/parcial y precondición

**Ubicación:** Después de la tabla de comandos (`Mover`/`Poner`) y sus ejemplos, ANTES de la sección de valores posibles por tipo.

**Modificar la tabla de comandos** para que quede así:

---

> | Comando | Tipo de Valor | Valores posibles |
> |---------|---------------|------------------|
> | Mover(dirección) | Direcciones | Norte, Este, Sur, Oeste |
> | Poner(color) | Colores | Azul, Negro, Rojo, Verde |
> | Sacar(color) | Colores | Azul, Negro, Rojo, Verde |

**Agregar después de la tabla:**

> ### El comando Sacar
> 
> Además de `Poner`, existe el comando `Sacar(color)` que **saca una bolita** del color indicado de la celda actual.
> 
> Ejemplo:
> ```
> Sacar(Rojo)   -- Saca una bolita roja de la celda actual
> ```
> 
> Pero ¡atención! ¿Qué pasa si intentamos sacar una bolita que no existe? El programa falla. Esto nos lleva a un concepto importante.
> 
> ### Operaciones totales y parciales
> 
> No todos los comandos pueden ejecutarse siempre. Algunos tienen **requisitos** que deben cumplirse:
> 
> - **Operación total:** Se puede ejecutar siempre, sin requisitos. Ejemplo: `Poner(Azul)` siempre funciona, podemos poner bolitas sin límite.
> 
> - **Operación parcial:** Solo se puede ejecutar si se cumple cierta condición. Si la condición no se cumple, el programa falla.
> 
> La condición que debe cumplirse para que una operación parcial funcione se llama **precondición**.
> 
> **Ejemplos:**
> 
> | Comando | Tipo de operación | Precondición |
> |---------|-------------------|--------------|
> | `Poner(color)` | Total | Ninguna (siempre funciona) |
> | `Sacar(color)` | Parcial | Debe haber al menos una bolita del color indicado en la celda actual |
> | `Mover(dir)` | Parcial | Debe existir una celda en la dirección indicada (no estar en el borde) |
> 
> Cuando una operación parcial falla porque no se cumple su precondición, decimos que el programa **"explota"** o produce un error en tiempo de ejecución.

---

## CAMBIO #3 — Prioridad: MEDIA

### Aclarar que el argumento determina el resultado del comando

**Ubicación:** Después del párrafo que dice:
> *"A los valores que van dentro de los paréntesis los llamamos argumentos. Entonces para ser más claros los comandos pueden recibir argumentos."*

Insertar ANTES del párrafo que dice:
> *"Estos Valores pueden ser agrupados en diferentes grupos llamados Tipos de Valores."*

**Texto a insertar:**

---

> El **argumento** que pasamos al comando determina exactamente qué acción se realiza:
> - `Poner(Azul)` pone una bolita **azul** porque el argumento es `Azul`
> - `Poner(Rojo)` pone una bolita **roja** porque el argumento es `Rojo`
> - `Mover(Norte)` mueve hacia el **norte** porque el argumento es `Norte`
> 
> Es decir, el comando indica *qué tipo de acción* (poner, mover, sacar) y el argumento indica *los detalles específicos* de esa acción (qué color, qué dirección).

---

## CAMBIO #4 — Prioridad: BAJA

### Mencionar otros comandos nativos que veremos más adelante

**Ubicación:** Al final de la sección de comandos, antes de "Flujo de un programa", o como nota al pie.

**Texto a insertar:**

---

> **Nota:** Gobstones tiene otros comandos nativos como `IrAlBorde(dir)` y `VaciarTablero()` que veremos en unidades posteriores cuando los necesitemos.

---

## CAMBIO #5 — Prioridad: BAJA

### Explicar qué es un "error de tipo" en la sección de errores

**Ubicación:** En la sección "Errores de tipeo y/o de tipos", después de mencionar `Mover(Azul)`.

**Texto a agregar o reformular:**

---

> Cuando escribimos `Mover(Azul)`, estamos cometiendo un **error de tipo**: el comando `Mover` espera un argumento de tipo Dirección (`Norte`, `Este`, `Sur`, `Oeste`), pero le estamos pasando un Color (`Azul`). Gobstones detecta esta incompatibilidad y nos avisa antes de ejecutar el programa.
> 
> De manera similar, `Poner(Norte)` es un error de tipo porque `Poner` espera un Color, no una Dirección.

---

## Resumen de cambios

| # | Prioridad | Tipo | Ubicación | Descripción |
|---|-----------|------|-----------|-------------|
| 1 | Alta | Agregar | Después de "argumentos", antes de "Tipos de Valores" | Definición formal de "valor" y "tipo de valor" |
| 2 | Alta | Agregar | Después de tabla de comandos | Comando `Sacar`, operaciones totales/parciales, precondición |
| 3 | Media | Aclarar | Después de ejemplos de comandos | El argumento determina el resultado específico |
| 4 | Baja | Agregar | Final de sección comandos | Mención de `IrAlBorde`, `VaciarTablero` |
| 5 | Baja | Aclarar | Sección "Errores de tipeo y/o de tipos" | Explicar qué es un error de tipo |

---

## Verificación de coherencia con Práctica 01

- [x] Práctica usa `Mover` y `Poner` → Teórica los cubre
- [x] Práctica pregunta "¿cómo decide Gobstones el tipo de bolita?" → Cambio #3 lo responde
- [x] Práctica menciona errores por salir del tablero → Teórica lo cubre + ahora explica precondición
- [ ] Práctica NO usa `Sacar` → No hay conflicto, `Sacar` se introduce como concepto pero no se exige en práctica

**Conclusión:** No es necesario modificar `Práctica 01 Introducción a Gobstones_.docx`. Los cambios en la teórica mejoran la base conceptual sin generar desajustes.

---

## Cambios NO aplicados

Ninguno. Todas las preguntas abiertas fueron respondidas por el docente.

---

**Fin del documento de cambios.**
