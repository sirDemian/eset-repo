# Informe de Revisión: Unidad 05 Teórica — Condicional Simple (if-else)

**Versión:** 2 (post-corrección)  
**Fecha de revisión:** 2026-02-20  
**Archivo revisado:** `Teórica/Unidad 05 if-else - Teórica.odt`  
**Práctica asociada:** `Práctica/Práctica 05 if - else_.docx`  
**Informe anterior:** `Informe_Unidad05_v1.md`

---

## 1) Resumen ejecutivo

**Estado general de alineación:** Alta

**3 principales fortalezas:**

1. **Tipo Booleano introducido formalmente:** Tabla de tipos ampliada con Booleano (True/Verdadero, False/Falso), manteniendo la progresión del sistema de tipos.
2. **"Consultas nativas" bien diferenciadas de "comandos":** Sección renombrada y reformulada, distinguiendo que las consultas devuelven información sin modificar el tablero.
3. **Condición formalizada:** Se define como expresión que produce un valor booleano, conectada con las consultas nativas.

**Cambios aplicados desde v1:**

1. ~~No introducía tipo Booleano~~ → **RESUELTO** (tabla de tipos ampliada)
2. ~~Llamaba "comandos nativos" a puedeMover/hayBolitas/nroBolitas~~ → **RESUELTO** (renombrado a "Consultas Nativas")
3. ~~nroBolitas no aclaraba que devuelve Número~~ → **RESUELTO** (aclara "Tipo: Número. No booleano")
4. ~~No formalizaba qué es una "condición"~~ → **RESUELTO** (definición agregada)
5. ~~"identación"~~ → **RESUELTO** en teórica ("indentación")
6. ~~"solo si hay ninguna bolita Azul"~~ → **RESUELTO** ("solo si hay al menos una bolita Azul")

**Riesgo pedagógico global:** Bajo — La guía está completa y bien alineada.

---

## 2) Identificación de unidad y alcance

| Campo | Valor |
|-------|-------|
| **Unidad** | 5 – Condicional Simple (if-else) |
| **Tema central** | Estructura de control condicional para toma de decisiones |
| **Subtemas detectados** | Definición de condicional, sintaxis if, extensión else, condición como expresión booleana, uso en procedimientos, consultas nativas (puedeMover, hayBolitas, nroBolitas), tipo Booleano, tabla de tipos ampliada, buenas prácticas, errores comunes, preguntas de reflexión |
| **Prerrequisitos asumidos** | Unidad 1-2: comandos, procedimientos. Unidad 3: repeat, estructura de control. Unidad 4: parámetros |
| **Documentos usados** | `programa 2024.docx`, `Planificación 2025.docx`, `BasesConceptualesProg.pdf`, `Unidad 05 if-else - Teórica.odt`, `Práctica 05 if - else_.docx` |

---

## 3) Alineación con Programa (programa 2024 + planificación 2025)

### 3.1 Mapa de objetivos ↔ cobertura

| Objetivo/resultado esperado (del programa) | Estado | Evidencia en Teórica | Observación |
|--------------------------------------------|--------|----------------------|-------------|
| Comprender la estructura condicional if | **Cubierto** | Sección "¿Qué es una estructura condicional?" con sintaxis y ejemplo | OK |
| Comprender la extensión else | **Cubierto** | Sección "Extensión del condicional: if-else" con ejemplo motivador | OK |
| Usar condicionales en procedimientos | **Cubierto** | Sección "Uso de condiciones en procedimientos" | OK |
| Conocer consultas nativas para condiciones | **Cubierto** | Sección "Consultas Nativas (expresiones)" | OK (mejorado en v1) |
| Comprender el tipo Booleano | **Cubierto** | Tabla de tipos ampliada con Booleano | OK (mejorado en v1) |
| Comprender qué es una condición | **Cubierto** | Definición formal como expresión booleana | OK (mejorado en v1) |

---

## 4) Correspondencia con BasesConceptualesProg.pdf

### Verificación de cambios aplicados desde v1

| Hallazgo v1 | Estado | Evidencia |
|-------------|--------|-----------|
| Introducir tipo Booleano | **Resuelto** | Tabla de tipos con Booleano: "True (Verdadero) / False (Falso)" |
| Renombrar "Comandos nativos" → "Consultas nativas" | **Resuelto** | Sección "Consultas Nativas (expresiones)" con distinción clara |
| Aclarar nroBolitas devuelve Número | **Resuelto** | "Tipo: Número. No booleano, no se puede pasar directo como condición del if" |
| Formalizar qué es una condición | **Resuelto** | "Es una expresión que produce un valor booleano (Verdadero o Falso)" |
| Corregir "identación" | **Resuelto** | Ahora dice "indentación" en teórica |
| Corregir ambigüedad ejemplo | **Resuelto** | "solo si hay al menos una bolita Azul" |

### Hallazgos nuevos (v2)

| Severidad | Tipo | Descripción | Ubicación |
|-----------|------|-------------|-----------|
| **Baja** | Typo | "Algunos consultas nativas" → "Algunas consultas nativas" | Sección "Consultas Nativas" |
| **Baja** | Typo | Tabla de tipos: "Valores Posibler" → "Valores Posibles" | Tabla de tipos |
| **Baja** | Claridad | Título "Consultas Nativas (expresiones)" — el "(expresiones)" podría anticipar terminología de Unidad 7. Considerar si dejarlo o quitarlo. | Título de sección |

---

## 5) Coherencia Teórica ↔ Práctica

| Contenido exigido por Práctica 05 | ¿Presente en Teórica? | Observación |
|-----------------------------------|----------------------|-------------|
| Uso de if simple | Sí | OK |
| Uso de if-else | Sí | OK |
| puedeMover(direccion) | Sí | OK |
| hayBolitas(color) | Sí | OK |
| nroBolitas(color) | Sí | OK, con aclaración de tipo |
| Condicionales en procedimientos | Sí | OK |
| Documentación | Sí | OK |

**Observaciones sobre la Práctica 05:**

- **"identación" en requisitos de la práctica:** Sigue sin corregir (la teórica ya fue corregida).
- **Ejercicio 10:** Sigue pidiendo "Deja 5 bolitas del color col" sin aparente necesidad de if/else. Pendiente de respuesta del docente.

---

## 6) Observaciones pedagógicas y de claridad

### Mejoras aplicadas

- La tabla de tipos ampliada con Booleano mantiene la excelente progresión del sistema de tipos a lo largo de las unidades.
- La distinción consultas vs comandos es clara y no anticipa terminología formal innecesaria.
- La definición de condición como expresión booleana conecta bien con el nuevo tipo.
- La aclaración de `nroBolitas` como Número (no Booleano) previene confusiones.

### Observaciones menores

- Hay 2 typos menores (concordancia de género y "Posibler").
- El "(expresiones)" en el título de la sección es menor pero podría quitarse para no anticipar Unidad 7.

---

## 7) Lista de cambios recomendados (backlog)

| Prioridad | Cambio propuesto | Ubicación sugerida | Justificación |
|-----------|------------------|--------------------|---------------|
| **Baja** | Corregir "Algunos consultas" → "Algunas consultas" | Sección "Consultas Nativas" | Concordancia de género |
| **Baja** | Corregir "Valores Posibler" → "Valores Posibles" | Tabla de tipos | Typo |
| **Baja** | Considerar quitar "(expresiones)" del título | Título de sección | Evitar anticipar Unidad 7 |
| **Baja** | Corregir "identación" → "indentación" en Práctica 05 | Requisitos de la práctica | Ortografía (pendiente) |

---

## 8) Preguntas abiertas (para el docente)

1. **¿Ejercicio 10 de la práctica es intencional?** Pide "Deja 5 bolitas del color col" sin aparente necesidad de if/else. ¿Anticipa funciones?

---

**Fin del informe v2.**
