# Informe de Revisión: Unidad 04 Teórica — Parámetros

**Versión:** 2 (post-corrección)  
**Fecha de revisión:** 2026-02-15  
**Archivo revisado:** `Teórica/Unidad 04 Parámetros -Teórica.odt`  
**Práctica asociada:** `Práctica/Práctica 04 Parámetros_.docx`  
**Informe anterior:** `Informe_Unidad04_v1.md`

---

## 1) Resumen ejecutivo

**Estado general de alineación:** Alta

**3 principales fortalezas:**
1. **Distinción parámetro/argumento:** Ahora incluye una sección clara que distingue formalmente ambos términos (cumpliendo la decisión predefinida).
2. **Conexión con Unidad 3:** Menciona que `repeat(5)` también recibe argumentos y agrega `repeat(cantidad)` a la tabla de tipos.
3. **Excelente progresión pedagógica:** Parte de comandos nativos que ya usan parámetros, muestra que ya los conocían.

**Cambios aplicados desde v1:**
1. ~~No distinguía parámetro/argumento~~ → **RESUELTO**
2. ~~No conectaba con repeat~~ → **RESUELTO**
3. ~~No conectaba con tabla de tipos de Unidad 3~~ → **RESUELTO**
4. ~~"direccion" sin tilde~~ → **INTENCIONAL** (Gobstones no acepta acentos en nombres de parámetros)

**Riesgo pedagógico global:** Bajo — La guía está completa y bien alineada.

---

## 2) Identificación de unidad y alcance

| Campo | Valor |
|-------|-------|
| **Unidad** | 4 – Parámetros |
| **Tema central** | Parametrización de procedimientos para generalización |
| **Subtemas detectados** | Definición de parámetros, distinción parámetro/argumento, sintaxis, uso en comandos nativos, uso en procedimientos, múltiples parámetros, alcance local, tipos de parámetros, conexión con repeat, buenas prácticas, errores comunes, preguntas de reflexión |
| **Prerrequisitos asumidos** | Unidad 1: comandos, tipos. Unidad 2: procedimientos, efecto. Unidad 3: repeat, tipo Número |
| **Documentos usados** | `programa 2024.docx`, `Planificación 2025.docx`, `BasesConceptualesProg.pdf`, `Unidad 04 Parámetros -Teórica.odt`, `Práctica 04 Parámetros_.docx` |

---

## 3) Alineación con Programa (programa 2024 + planificación 2025)

### 3.1 Mapa de objetivos ↔ cobertura

| Objetivo/resultado esperado (del programa) | Estado | Evidencia en Teórica | Observación |
|--------------------------------------------|--------|----------------------|-------------|
| Comprender qué son los parámetros | **Cubierto** | Sección "¿Qué son los parámetros?" con definición y distinción | OK (mejorado en v1) |
| Definir procedimientos con parámetros | **Cubierto** | Sección "Definición y sintaxis" con ejemplo de PonerN | OK |
| Usar múltiples parámetros | **Cubierto** | Ejemplo con MoverYPoner(dirección, cantidad, color) | OK |
| Comprender alcance local | **Cubierto** | Sección "Alcance de los parámetros" con ejemplo | OK |
| Distinguir parámetro de argumento | **Cubierto** | Sección específica con distinción formal | OK (mejorado en v1) |
| Documentar procedimientos con parámetros | **Cubierto** | Sección "Buenas prácticas" | OK |

### 3.2 Secuenciación y tiempo

- **¿Respeta la secuencia sugerida por planificación?** Sí.
- **¿Hay temas adelantados o atrasados?** Las preguntas de reflexión adelantan la idea de verificación (condicionales), coherente con la práctica (Ejercicio 11).

---

## 4) Correspondencia con BasesConceptualesProg.pdf

### Verificación de cambios aplicados desde v1

| Hallazgo v1 | Estado | Evidencia |
|-------------|--------|-----------|
| Distinguir parámetro vs argumento | **Resuelto** | Sección con definición formal: "Parámetro: Es el nombre que aparece en la definición... Argumento: Es el valor concreto que le pasamos al llamar..." |
| Conectar tipos de parámetros con tabla de Unidad 3 | **Resuelto** | Tabla ampliada incluye `repeat(cantidad)` y menciona "Recordemos la tabla de la unidad 1" |
| Mencionar que repeat recibe argumentos | **Resuelto** | "De hecho, no solo los comandos nativos reciben argumentos. En la Unidad 3 ya usábamos repeat(5) pasándole un número como argumento." |

### Hallazgos nuevos (v2)

| Severidad | Tipo | Descripción | Ubicación |
|-----------|------|-------------|-----------|
| **Baja** | Typo | "Reflexión en retrospectivca" → "Reflexión en retrospectiva" | Sección "Reflexión en retrospectivca" |
| **Baja** | Typo | "argunmentos" → "argumentos" | Sección "Uso de parámetros en procedimientos" |
| **Baja** | Typo | "colore" → "color" | "En este caso los parámetros fueron del tipo colore" |

---

## 5) Coherencia Teórica ↔ Práctica

| Contenido exigido por Práctica 04 | ¿Presente en Teórica? | Observación |
|-----------------------------------|----------------------|-------------|
| Procedimientos con 1 parámetro | Sí | OK |
| Procedimientos con 2+ parámetros | Sí | OK |
| Parámetros de tipo Número | Sí | OK |
| Parámetros de tipo Color | Sí | OK |
| Parámetros de tipo Dirección | Sí | OK |
| Documentación con parámetros | Sí | OK |
| Alcance local | Sí | OK |
| Reflexión sobre condicionales (Ej. 11) | Parcial | Las preguntas guía lo insinúan pero no lo desarrollan (correcto, es anticipación) |

**Observaciones sobre la Práctica 04:**
- Sin cambios desde v1, lo cual está bien.
- Buena progresión: 1 parámetro → 2 parámetros → problemas complejos → reflexión.

---

## 6) Observaciones pedagógicas y de claridad

### Mejoras aplicadas
- La distinción parámetro/argumento es clara y cumple con la decisión predefinida.
- La conexión con `repeat` refuerza que ya usaban este mecanismo.
- La tabla de tipos ampliada con `repeat(cantidad)` es un excelente recurso visual.

### Observaciones menores
- "direccion" sin tilde es intencional (Gobstones no acepta acentos en nombres de parámetros).
- Hay algunos typos menores que podrían corregirse para mayor pulido.

---

## 7) Lista de cambios recomendados (backlog)

| Prioridad | Cambio propuesto | Ubicación sugerida | Justificación |
|-----------|------------------|--------------------|---------------|
| **Baja** | Corregir "Reflexión en retrospectivca" → "Reflexión en retrospectiva" | Título de sección | Ortografía |
| **Baja** | Corregir "argunmentos" → "argumentos" | Sección "Uso de parámetros en procedimientos" | Ortografía |
| **Baja** | Corregir "colore" → "color" | Mención de tipos de parámetros | Ortografía |

---

## 8) Preguntas abiertas (para el docente)

1. **¿Corregir los typos menores?** (retrospectivca, argunmentos, colore) Son detalles de pulido.

---

**Fin del informe v2.**
