# Informe de Revisión: Unidad 01 Teórica

**Versión:** 2 (post-corrección)  
**Fecha de revisión:** 2026-02-04  
**Archivo revisado:** `Teórica/Unidad 01 Teórica.odt`  
**Práctica asociada:** `Práctica/Práctica 01 Introducción a Gobstones_.docx`  
**Informe anterior:** `Informe_Unidad01_v1.md`

---

## 1) Resumen ejecutivo

**Estado general de alineación:** Alta

**3 principales fortalezas:**
1. Cubre todos los objetivos del programa: definición de programa, entorno Gobstones, comandos nativos, valores y tipos.
2. Incluye conceptos avanzados: operaciones totales/parciales, precondiciones, comando `Sacar`.
3. Sección pedagógica sobre errores bien desarrollada, alineada con filosofía del programa.

**3 principales problemas (resueltos en v1, pendientes menores):**
1. ~~No definía formalmente "valor" ni "tipo de valor"~~ → **RESUELTO**
2. ~~Omitía comando `Sacar` y operaciones totales/parciales~~ → **RESUELTO**
3. **Typo menor** en tabla de comandos: `Sacar(color(Colores` debería ser `Sacar(color) | Colores`

**Riesgo pedagógico global:** Bajo — La guía está completa y alineada con programa y bases conceptuales.

---

## 2) Identificación de unidad y alcance

| Campo | Valor |
|-------|-------|
| **Unidad** | 1 – Gobstones / Introducción |
| **Tema central** | Qué es un programa, entorno Gobstones, comandos nativos, valores y tipos |
| **Subtemas detectados** | Definición de programa, tablero/celdas/cabezal/bolitas, comandos `Mover`, `Poner` y `Sacar`, tipos Colores y Direcciones, operaciones totales/parciales, precondiciones, flujo secuencial, manejo de errores |
| **Prerrequisitos asumidos** | Ninguno explícito (es la primera unidad) |
| **Documentos usados** | `programa 2024.docx`, `Planificación 2025.docx`, `BasesConceptualesProg.pdf`, `Unidad 01 Teórica.odt`, `Práctica 01 Introducción a Gobstones_.docx` |

---

## 3) Alineación con Programa (programa 2024 + planificación 2025)

### 3.1 Mapa de objetivos ↔ cobertura

| Objetivo/resultado esperado (del programa) | Estado | Evidencia en Teórica | Observación |
|--------------------------------------------|--------|----------------------|-------------|
| Conocer el entorno de desarrollo Gobstones | **Cubierto** | Sección "¿Qué es Gobstones?" y "Conociendo Gobstones" | OK |
| Entender el concepto de valores | **Cubierto** | "Un valor es un dato concreto que usamos en nuestros programas..." | OK (agregado en v1) |
| ¿Qué es un programa? / ¿Qué es programar? | **Cubierto** | Sección "Introducción" con definición de programa | OK |
| Introducción a Valores y Tipos de valores | **Cubierto** | "Los valores se agrupan en Tipos de Valores. Un tipo de valor es una categoría..." | OK (agregado en v1) |
| Acciones y Comandos, diferencias | **Cubierto** | "Los comandos son descripciones de las acciones..." + operaciones totales/parciales | OK (mejorado en v1) |
| Comandos nativos: Mover, Poner | **Cubierto** | Tabla con comandos, tipos de valor y ejemplos | OK |
| Ejecución secuencial de un programa | **Cubierto** | Sección "Flujo de un programa" | OK |

### 3.2 Secuenciación y tiempo

- **¿Respeta la secuencia sugerida por planificación?** Sí.
- **¿Hay temas adelantados o atrasados?** No. Los conceptos de operación total/parcial y precondición se introducen de forma básica, preparando para unidades posteriores.

---

## 4) Correspondencia con BasesConceptualesProg.pdf

### Verificación de cambios aplicados desde v1

| Hallazgo v1 | Estado | Evidencia |
|-------------|--------|-----------|
| Definición de "valor" ausente | **Resuelto** | "Un valor es un dato concreto que usamos en nuestros programas" |
| Comando `Sacar` omitido | **Resuelto** | Sección "El comando Sacar" + tabla actualizada |
| Operaciones totales/parciales no explicadas | **Resuelto** | Sección "Operaciones totales y parciales" con tabla de precondiciones |
| Comandos `IrAlBorde` y `VaciarTablero` no mencionados | **Resuelto** | Nota al final mencionándolos |

### Hallazgos nuevos (v2)

| Severidad | Tipo | Descripción | Ubicación |
|-----------|------|-------------|-----------|
| Bajo | Typo | Tabla de comandos tiene `Sacar(color(Colores` en lugar de `Sacar(color) \| Colores` | Tabla de valores posibles |

---

## 5) Coherencia Teórica ↔ Práctica

| Contenido exigido por Práctica 01 | ¿Presente en Teórica? | Observación |
|-----------------------------------|----------------------|-------------|
| Comando `Mover` | Sí | OK |
| Comando `Poner` | Sí | OK |
| Tipos Colores y Direcciones | Sí | OK |
| Ejecución secuencial | Sí | OK |
| Manejo de errores | Sí | OK + ahora explica precondición |
| Concepto de "tablero inicial" y "tablero final" | Sí | OK |

**Desajustes detectados:** Ninguno.

---

## 6) Observaciones pedagógicas y de claridad

- **Mejora notable:** La explicación de que el argumento determina el resultado específico del comando responde directamente a la pregunta de la práctica.
- **Mejora notable:** La introducción de operaciones totales/parciales prepara al estudiante para entender errores de ejecución.
- **Pendiente menor:** En la sección "Errores de tipeo y/o de tipos" se podría agregar una referencia cruzada al concepto de "error de tipo" ya definido antes.

---

## 7) Lista de cambios recomendados (backlog)

| Prioridad | Cambio propuesto | Ubicación sugerida | Justificación |
|-----------|------------------|--------------------|---------------|
| **Bajo** | Corregir typo en tabla: `Sacar(color(Colores` → `Sacar(color) \| Colores` | Tabla de valores posibles (segunda tabla) | Error de formato |
| **Bajo** | Agregar referencia cruzada en sección de errores: "Como vimos antes, esto es un error de tipo" | Sección "Errores de tipeo y/o de tipos" | Refuerzo conceptual |

---

## 8) Preguntas abiertas (para el docente)

Ninguna. Todas las preguntas de v1 fueron respondidas y los cambios aplicados.

---

**Fin del informe v2.**
