# Cambios a Aplicar: Unidad 02 Teórica — Procedimientos

**Versión:** 1 (inicial)  
**Fecha:** 2026-02-04  
**Archivo a modificar:** `Teórica/Unidad 02 Procedimientos - Teórica.docx`  
**Basado en:** `Informes/Unidad_02/Informe_Unidad02_v1.md`

---

## Cambios propuestos

### CAMBIO #1 — Prioridad: ALTA

#### Agregar definición formal de procedimiento

**Ubicación:** Sección "¿Qué es un procedimiento?", al inicio.

**Texto actual:**
> Un procedimiento es una herramienta que nos brinda una forma de encapsular parte del código...

**Texto propuesto (insertar ANTES del texto actual):**

> Un procedimiento es una **acción definida por el programador**. Así como en la Unidad 1 usamos comandos nativos como `Mover` y `Poner` (acciones que ya vienen con Gobstones), ahora aprenderemos a crear nuestras propias acciones.

Luego continúa con el texto existente.

---

### CAMBIO #2 — Prioridad: ALTA

#### Introducir el concepto de "efecto"

**Ubicación:** Después del párrafo que dice:
> "La principal condición o característica de los procedimientos es que siempre modifican el tablero y tienen como objetivo resolver un problema específico."

**Texto a agregar:**

> A este cambio que produce el procedimiento en el tablero lo llamamos **efecto**. Todo procedimiento tiene un efecto: puede poner bolitas, moverlas, sacarlas, o una combinación de estas acciones. Cuando documentamos un procedimiento, el "propósito" describe precisamente cuál es su efecto.

---

### CAMBIO #3 — Prioridad: MEDIA

#### Conectar "precondición" con Unidad 1

**Ubicación:** Sección "Documentación y buenas prácticas", en la definición de Precondición.

**Texto actual:**
> Precondición: ¿Qué necesita para ejecutarse correctamente, sin explotar?

**Texto propuesto:**

> **Precondición:** ¿Qué necesita para ejecutarse correctamente, sin explotar? Recordá que en la Unidad 1 vimos que algunas operaciones son **parciales** (como `Mover` o `Sacar`) y requieren que se cumpla una condición. Si tu procedimiento usa operaciones parciales, su precondición debe reflejar esas restricciones.

---

### CAMBIO #4 — Prioridad: MEDIA

#### Aclarar que los procedimientos NO retornan valores

**Ubicación:** Al final de la sección "¿Qué es un procedimiento?", antes de "Definición de un procedimiento".

**Texto a agregar:**

> **Importante:** Los procedimientos solo producen efectos en el tablero, pero **no devuelven valores**. Si necesitamos obtener información del tablero (por ejemplo, saber cuántas bolitas hay), usaremos **funciones**, que veremos en la Unidad 7.

---

### CAMBIO #5 — Prioridad: BAJA

#### Conexión pedagógica con Unidad 1

**Ubicación:** Introducción, después de "Aquí es donde entran los procedimientos..."

**Texto a agregar:**

> En otras palabras, crear un procedimiento es como **crear nuestro propio comando**. Así como `Mover(Norte)` es un comando que mueve el cabezal, podemos crear `MoverTresAlNorte()` que haga exactamente lo que su nombre indica.

---

## Resumen de cambios v1

| # | Prioridad | Tipo | Ubicación | Descripción |
|---|-----------|------|-----------|-------------|
| 1 | Alta | Agregar | "¿Qué es un procedimiento?" | Definición formal: "acción definida por el programador" |
| 2 | Alta | Agregar | Después de "modifican el tablero" | Concepto de "efecto" |
| 3 | Media | Modificar | "Documentación y buenas prácticas" | Conectar precondición con Unidad 1 |
| 4 | Media | Agregar | Final de "¿Qué es un procedimiento?" | Aclarar que no retornan valores |
| 5 | Baja | Agregar | Introducción | Conexión pedagógica "crear nuestro propio comando" |

---

## Corrección en Práctica 02 (posible typo)

**Ejercicio 11:** Dice "Poner_8_Azules que ponga **5** bolitas". 

**Acción sugerida:** Verificar si debería ser:
- "Poner_8_Azules que ponga **8** bolitas", o
- "Poner_5_Azules que ponga **5** bolitas"

---

## Preguntas pendientes para el docente

Antes de aplicar los cambios, necesito tu decisión sobre:

1. **¿Introducir "efecto" formalmente?** (Cambio #2)
2. **¿Conectar precondición con Unidad 1?** (Cambio #3)
3. **¿Corregir el typo en Práctica 02?** (Ejercicio 11)

---

**Fin del documento de cambios v1.**
