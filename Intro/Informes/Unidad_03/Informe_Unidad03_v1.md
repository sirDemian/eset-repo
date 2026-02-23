# Informe de Revisión: Unidad 03 Teórica — Repetición Simple (repeat)

**Versión:** 1 (revisión inicial)  
**Fecha de revisión:** 2026-02-11  
**Archivo revisado:** `Teórica/Unidad 03 Repeat - Teórica.docx`  
**Práctica asociada:** `Práctica/Práctica 03 Repetición Simple_.docx`

---

## 1) Resumen ejecutivo

**Estado general de alineación:** Media

**3 principales fortalezas:**
1. Buen ejemplo comparativo (sin repeat vs con repeat) que muestra claramente la ventaja.
2. Combina repeat con procedimientos, reforzando Unidad 2.
3. Sección de errores comunes bien orientada con casos concretos (llaves, valores no válidos, estado inicial).

**3 principales problemas:**
1. **No define formalmente "estructura de control"** — usa el término con una nota al pie ("estructura de control 1") pero no lo explica.
2. **No introduce el tipo Número** — `repeat` requiere un valor entero pero no se conecta con el sistema de tipos visto en Unidad 1.
3. **Falta el concepto de "subtarea repetida"** — no explica que lo que se repite es una subtarea, conectando con la idea de procedimiento como subtarea de Unidad 2.

**Riesgo pedagógico global:** Medio — Funcional pero falta formalización de conceptos clave.

---

## 2) Identificación de unidad y alcance

| Campo | Valor |
|-------|-------|
| **Unidad** | 3 – Repetición Simple (repeat) |
| **Tema central** | Estructura de control `repeat` para repetición de bloques de código |
| **Subtemas detectados** | Definición de repeat, sintaxis, ventajas, combinación con procedimientos, buenas prácticas, errores comunes, preguntas de reflexión |
| **Prerrequisitos asumidos** | Unidad 1: comandos, valores, tipos. Unidad 2: procedimientos, efecto, documentación |
| **Documentos usados** | `programa 2024.docx`, `Planificación 2025.docx`, `BasesConceptualesProg.pdf`, `Unidad 03 Repeat - Teórica.docx`, `Práctica 03 Repetición Simple_.docx` |

---

## 3) Alineación con Programa (programa 2024 + planificación 2025)

### 3.1 Mapa de objetivos ↔ cobertura

| Objetivo/resultado esperado (del programa) | Estado | Evidencia en Teórica | Observación |
|--------------------------------------------|--------|----------------------|-------------|
| Comprender la estructura de repetición simple | **Cubierto** | Sección "¿Qué es la repetición simple?" + sintaxis | OK |
| Usar `repeat` con un número fijo de repeticiones | **Cubierto** | Ejemplo con repeat(5) | OK |
| Combinar repeat con procedimientos | **Cubierto** | Sección "Repetición dentro de procedimientos" | OK |
| Identificar ventajas de repeat vs secuencia manual | **Cubierto** | Sección "Ventajas del uso de repeat" | OK |
| Documentar programas con repeat | **Cubierto** | Sección "Buenas prácticas con repeat" | OK |

### 3.2 Secuenciación y tiempo

- **¿Respeta la secuencia sugerida por planificación?** Sí.
- **¿Hay temas adelantados o atrasados?** Las preguntas de reflexión adelantan la idea de generalización (parámetros, Unidad 4), lo cual es intencional.

---

## 4) Correspondencia con BasesConceptualesProg.pdf

### 4.1 Conceptos que deberían estar según las bases

| Concepto de las bases | ¿Presente? | Observación |
|-----------------------|------------|-------------|
| Estructura de control | **Parcial** | Menciona "estructura de control" con nota al pie pero no la define |
| repeat como repetición indexada | **Parcial** | Describe la mecánica pero no usa terminología formal |
| Tipo Número (entero positivo) | **No** | Dice "n es un valor entero positivo" pero no lo conecta con el sistema de tipos |
| Modificación del flujo de ejecución | **Cubierto** | "repetir un bloque de código rompe con la ejecución secuencial" |

### 4.2 Hallazgos específicos

| Severidad | Tipo | Descripción | Ubicación |
|-----------|------|-------------|-----------|
| **Alta** | Faltante | No define "estructura de control". Dice "estructura de control 1" con una nota al pie que no se resuelve en el texto extraído | Sección "¿Qué es la repetición simple?" |
| **Media** | Faltante | No introduce el tipo Número. El `repeat` usa un número entero pero no se conecta con el sistema de tipos (Colores, Direcciones → ahora también Números) | Sección "Definición y sintaxis de repeat" |
| **Media** | Inconsistencia | Usa "identación" en lugar de "indentación" (mismo error que Unidad 2) | Sección "Buenas prácticas con repeat" |
| **Baja** | Faltante | No menciona que `repeat(0)` es válido pero no ejecuta el bloque (lo menciona parcialmente: "n debe ser mayor que cero... no se producirá ningún cambio") | Sección "Errores comunes" |
| **Baja** | Oportunidad | Podría conectar "lo que se repite" con el concepto de subtarea/efecto de Unidad 2 | General |

---

## 5) Coherencia Teórica ↔ Práctica

| Contenido exigido por Práctica 03 | ¿Presente en Teórica? | Observación |
|-----------------------------------|----------------------|-------------|
| Uso de `repeat` con número fijo | Sí | OK |
| Combinación de repeat con procedimientos | Sí | OK |
| Documentación (propósito, precondición) | Sí | OK |
| Dibujar patrones (líneas, cuadrados, cruces) | Sí | Ejemplo de línea; los patrones complejos se dejan para la práctica |
| Reflexión sobre generalización | Sí | Preguntas guía al final |

**Desajustes detectados:**
- **Práctica 03, Ejercicio 5:** Dice "Define un procedimiento llamado DibujarLineaAzulDeTres()" pero el ejercicio pide "Dibujar un cuadrado 3x3". El nombre del procedimiento no coincide con la consigna — parece un copy-paste del Ejercicio 4.
- **Práctica 03, Ejercicio 9:** Pide "MoverHastaElBordeNorte" usando `repeat`, pero con `repeat` necesitás saber de antemano cuántas celdas hay. La pista dice "tablero de 5x3" pero esto es una limitación de `repeat` que podría confundir. Este ejercicio parece más adecuado para `while` (Unidad 8).

---

## 6) Observaciones pedagógicas y de claridad

### Fortalezas
- El ejemplo comparativo sin/con repeat es muy efectivo.
- La sección de errores comunes cubre casos reales que los alumnos van a encontrar.
- Las preguntas de reflexión preparan bien para parámetros (Unidad 4).

### Oportunidades de mejora
- **Definir "estructura de control":** Es la primera vez que aparece el concepto. Merece una definición clara: "una instrucción que modifica el flujo de ejecución del programa".
- **Introducir tipo Número:** El `repeat` es la primera vez que se usa un número explícitamente. Es una buena oportunidad para ampliar el sistema de tipos.
- **Conectar con Unidad 2:** Mencionar que lo que se repite dentro del `repeat` es una subtarea, reforzando el concepto de efecto.

---

## 7) Lista de cambios recomendados (backlog)

| Prioridad | Cambio propuesto | Ubicación sugerida | Justificación |
|-----------|------------------|--------------------|---------------|
| **Alta** | Definir "estructura de control": instrucción que modifica el flujo de ejecución | Sección "¿Qué es la repetición simple?", reemplazando la nota al pie | Primera aparición del concepto |
| **Media** | Introducir el tipo Número como nuevo tipo de valor | Sección "Definición y sintaxis de repeat", al explicar `n` | Ampliación del sistema de tipos |
| **Media** | Corregir "identación" → "indentación" | Sección "Buenas prácticas con repeat" | Ortografía (mismo error que Unidad 2) |
| **Baja** | Conectar la subtarea repetida con el concepto de efecto de Unidad 2 | Sección "Repetición dentro de procedimientos" | Coherencia conceptual |

---

## 8) Preguntas abiertas (para el docente)

1. **¿Introducir el tipo Número formalmente?** El `repeat` usa un entero. ¿Querés que se agregue como nuevo tipo de valor (sumándose a Colores y Direcciones)?

2. **Ejercicio 5 de Práctica 03:** Parece un copy-paste del Ejercicio 4 (dice "DibujarLineaAzulDeTres" pero pide un cuadrado 3x3). ¿Corregir?

3. **Ejercicio 9 de Práctica 03:** Pide "MoverHastaElBordeNorte" con `repeat`, pero esto requiere conocer el tamaño del tablero de antemano. ¿Es intencional para mostrar la limitación de `repeat`, o debería moverse a la unidad de `while`?

---

**Fin del informe v1.**
