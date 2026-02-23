# Cambios a Aplicar: Unidad 03 Teórica — Repetición Simple (repeat)

**Versión:** 1 (inicial)  
**Fecha:** 2026-02-11  
**Archivo a modificar:** `Teórica/Unidad 03 Repeat - Teórica.docx`  
**Basado en:** `Informes/Unidad_03/Informe_Unidad03_v1.md`

---

## Cambios propuestos

### CAMBIO #1 — Prioridad: ALTA

#### Definir "estructura de control"

**Ubicación:** Sección "¿Qué es la repetición simple?", donde dice:
> "usamos la estructura de control 1 repeat"

**Texto propuesto (reemplazar la oración):**

> En Gobstones, usamos la **estructura de control** `repeat` para realizar estas repeticiones de forma eficiente. Una estructura de control es una instrucción especial que **modifica el flujo de ejecución** del programa. Hasta ahora, nuestros programas se ejecutaban línea a línea de arriba hacia abajo (flujo secuencial). Con `repeat`, le indicamos a la computadora que vuelva a ejecutar un bloque de código varias veces antes de continuar.

---

### CAMBIO #2 — Prioridad: MEDIA

#### Introducir el tipo Número

**Ubicación:** Sección "Definición y sintaxis de repeat", después de:
> "n es un valor entero positivo que indica cuántas veces se repetirá el bloque."

**Texto a agregar:**

> Recordemos que en la Unidad 1 vimos que los valores se agrupan en **tipos**. Hasta ahora conocíamos Colores y Direcciones. Ahora aparece un nuevo tipo: los **Números**. El valor `n` que recibe `repeat` es un número entero positivo. Así, nuestro sistema de tipos crece:
>
> | Tipo | Valores posibles | Ejemplo de uso |
> |------|-----------------|----------------|
> | Direcciones | Norte, Este, Sur, Oeste | `Mover(Norte)` |
> | Colores | Azul, Negro, Rojo, Verde | `Poner(Azul)` |
> | Números | 0, 1, 2, 3, ... | `repeat(5)` |

---

### CAMBIO #3 — Prioridad: MEDIA

#### Corregir "identación" → "indentación"

**Ubicación:** Aparece dos veces en el documento:
1. Sección "Definición y sintaxis de repeat": "Observen la identación"
2. Sección "Buenas prácticas con repeat": "Identación:"

**Texto actual:** `identación` / `Identación`  
**Texto corregido:** `indentación` / `Indentación`

---

### CAMBIO #4 — Prioridad: BAJA

#### Conectar subtarea repetida con efecto (Unidad 2)

**Ubicación:** Sección "Repetición dentro de procedimientos", después de:
> "Definamos un procedimiento con el programa anterior"

**Texto a agregar:**

> Observá que lo que se repite dentro del `repeat` es una **subtarea**: poner una bolita y mover el cabezal. Al encapsular esto en un procedimiento, estamos dando nombre a un efecto que se repite. El procedimiento `DibujarLineaAzulDe5Celdas` tiene como **efecto** dibujar una línea de 5 bolitas azules, y ese efecto se logra repitiendo una subtarea más simple.

---

## Resumen de cambios v1

| # | Prioridad | Tipo | Ubicación | Descripción |
|---|-----------|------|-----------|-------------|
| 1 | Alta | Agregar/Modificar | "¿Qué es la repetición simple?" | Definir "estructura de control" |
| 2 | Media | Agregar | "Definición y sintaxis de repeat" | Introducir tipo Número |
| 3 | Media | Corregir | Dos ubicaciones | "identación" → "indentación" |
| 4 | Baja | Agregar | "Repetición dentro de procedimientos" | Conectar subtarea con efecto |

---

## Correcciones en Práctica 03

### Ejercicio 5 (posible copy-paste)
Dice "Define un procedimiento llamado DibujarLineaAzulDeTres()" pero pide "Dibujar un cuadrado 3x3". El nombre no coincide con la consigna.

**Acción sugerida:** Cambiar el nombre del procedimiento a `DibujarCuadrado3x3()` o similar.

### Ejercicio 9 (posible desajuste de unidad)
Pide "MoverHastaElBordeNorte" con `repeat`, pero esto requiere conocer el tamaño del tablero. 

**Acción sugerida:** ¿Es intencional para mostrar la limitación de `repeat`? ¿O debería moverse a la unidad de `while`?

---

## Preguntas pendientes para el docente

1. **¿Introducir el tipo Número formalmente?** (Cambio #2)
2. **¿Corregir Ejercicio 5 de Práctica 03?** (copy-paste de Ejercicio 4)
3. **¿Ejercicio 9 es intencional?** (limitación de repeat vs while)

---

**Fin del documento de cambios v1.**
