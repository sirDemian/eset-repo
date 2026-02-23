# Cambios a Aplicar: Unidad 05 Teórica — Condicional Simple (if-else)

**Versión:** 1 (inicial)  
**Fecha:** 2026-02-15  
**Archivo a modificar:** `Teórica/Unidad 05 if-else - Teórica.docx`  
**Basado en:** `Informes/Unidad_05/Informe_Unidad05_v1.md`

---

## Cambios propuestos

### CAMBIO #1 — Prioridad: ALTA

#### Introducir tipo Booleano y ampliar tabla de tipos

**Ubicación:** Antes o junto a la sección "Comandos nativos". Propuesta: nueva subsección.

**Texto propuesto:**

> Con las estructuras condicionales aparece un nuevo tipo de valor: el **Booleano**. Los valores booleanos son solo dos: **Verdadero** y **Falso**. Ampliemos nuestra tabla de tipos:
>
> | Tipo | Valores posibles | Ejemplo de uso |
> |------|-----------------|----------------|
> | Direcciones | Norte, Este, Sur, Oeste | `Mover(Norte)` |
> | Colores | Azul, Negro, Rojo, Verde | `Poner(Azul)` |
> | Números | 0, 1, 2, 3… | `repeat(5)` |
> | **Booleanos** | **Verdadero, Falso** | **`puedeMover(Norte)`** |
>
> Las condiciones del `if` siempre se evalúan a un valor booleano: Verdadero o Falso.

---

### CAMBIO #2 — Prioridad: ALTA

#### Renombrar "Comandos nativos" → "Consultas nativas"

**Ubicación:** Sección "Comandos nativos" — renombrar título y reformular párrafo introductorio.

**Problema:** `puedeMover`, `hayBolitas` y `nroBolitas` no son comandos (no producen efecto). La distinción formal comando/expresión se hará en Unidad 7. Por ahora, usar el término **"consultas nativas"** como nombre intermedio que no genera confusión.

**Texto propuesto (reemplazar título y párrafo introductorio):**

> **Consultas nativas de Gobstones**
>
> Hasta ahora conocíamos los **comandos** nativos (`Poner`, `Sacar`, `Mover`), que producen un efecto en el tablero. Ahora introducimos las **consultas** nativas, que no modifican el tablero sino que nos **devuelven información** sobre el estado del mismo.
>
> - `puedeMover(direccion)` — Devuelve **Verdadero** si hay una celda en la dirección indicada, **Falso** en caso contrario. Tipo: Booleano.
> - `hayBolitas(color)` — Devuelve **Verdadero** si hay al menos una bolita de ese color en la celda actual, **Falso** en caso contrario. Tipo: Booleano.
> - `nroBolitas(color)` — Devuelve la cantidad de bolitas de ese color en la celda actual. Tipo: **Número** (no Booleano). No se puede usar directamente como condición del `if`.

---

### CAMBIO #3 — Prioridad: MEDIA

#### Aclarar que `nroBolitas` devuelve Número, no Booleano

**Ubicación:** Dentro de la sección reformulada del Cambio #2.

**Nota:** Si se aplica el Cambio #2, este ya queda cubierto en la descripción de `nroBolitas`. Si no, agregar al menos una aclaración:

> `nroBolitas(color)` devuelve un Número, no un Booleano. Para usarlo como condición se necesitaría compararlo con otro valor (por ejemplo, `nroBolitas(Azul) > 0`), pero las comparaciones numéricas se verán más adelante.

---

### CAMBIO #4 — Prioridad: MEDIA

#### Formalizar qué es una "condición"

**Ubicación:** Sección "¿Qué es una estructura condicional?", después de "condición es una expresión que se evalúa como verdadera o falsa".

**Texto propuesto (agregar):**

> Una **condición** es una expresión que produce un valor booleano (Verdadero o Falso). En Gobstones, las condiciones más comunes son las expresiones nativas como `puedeMover(Norte)` o `hayBolitas(Azul)`.

---

### CAMBIO #5 — Prioridad: BAJA

#### Corregir "identación" → "indentación"

**Ubicación:** Sección "Buenas prácticas" de la teórica. También en "Requisitos de la práctica" de Práctica 05.

**Texto actual:** "identación"  
**Texto corregido:** "indentación"

---

### CAMBIO #6 — Prioridad: BAJA

#### Corregir ambigüedad en ejemplo básico

**Ubicación:** Propósito del ejemplo básico.

**Texto actual:** "Coloca una bolita Roja en la celda actual solo si hay ninguna bolita Azul en ella."  
**Texto corregido:** "Coloca una bolita Roja en la celda actual solo si hay al menos una bolita Azul en ella."

(Verificar contra el código del ejemplo para confirmar el sentido correcto.)

---

## Resumen de cambios v1

| # | Prioridad | Tipo | Ubicación | Descripción |
|---|-----------|------|-----------|-------------|
| 1 | Alta | Agregar | Nueva sección / junto a "Comandos nativos" | Introducir tipo Booleano + tabla de tipos ampliada |
| 2 | Alta | Modificar | Sección "Comandos nativos" | Renombrar a "Consultas nativas" (distinción formal comando/expresión en Unidad 7) |
| 3 | Media | Agregar | Dentro de Cambio #2 o por separado | Aclarar que nroBolitas devuelve Número |
| 4 | Media | Agregar | "¿Qué es una estructura condicional?" | Formalizar qué es una condición |
| 5 | Baja | Corregir | "Buenas prácticas" + Práctica 05 | "identación" → "indentación" |
| 6 | Baja | Corregir | Ejemplo básico | Ambigüedad "si hay ninguna" |

---

## Decisiones tomadas por el docente

- **Tipo Booleano:** ✅ Sí, introducir como nuevo tipo en la tabla (Cambio #1)
- **"Comandos nativos" → "Consultas nativas":** ✅ Usar este término intermedio (Cambio #2). La distinción formal comando/expresión se hará en Unidad 7.
- **Expresiones booleanas (&&, ||, not):** ❌ No en Unidad 5. Dejar para Unidad 6.

## Preguntas pendientes para el docente

1. **¿Ejercicio 10 de la práctica es intencional?** Pide "Deja 5 bolitas del color col" sin aparente necesidad de if/else. ¿Anticipa funciones?
2. **¿Corregir "identación" en teórica y práctica?** (Cambio #5)

---

**Fin del documento de cambios v1.**
