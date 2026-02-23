# Informe de Revisión: Unidad 02 Teórica — Procedimientos

**Versión:** 2 (post-corrección)  
**Fecha de revisión:** 2026-02-08  
**Archivo revisado:** `Teórica/Unidad 02 Procedimientos - Teórica.odt`  
**Práctica asociada:** `Práctica/Práctica 02 Procedimientos_.docx`  
**Informe anterior:** `Informe_Unidad02_v1.md`

---

## 1) Resumen ejecutivo

**Estado general de alineación:** Alta

**3 principales fortalezas:**
1. Define formalmente procedimiento como "acción definida por el programador" alineado con las bases conceptuales.
2. Introduce el concepto de "efecto" conectándolo con la documentación (propósito).
3. Conecta "precondición" con operaciones parciales de Unidad 1, dando continuidad conceptual.

**3 principales problemas (resueltos en v1):**
1. ~~Faltaba definición formal de procedimiento~~ → **RESUELTO**
2. ~~No mencionaba "efecto"~~ → **RESUELTO**
3. ~~Precondición desconectada de Unidad 1~~ → **RESUELTO**

**Riesgo pedagógico global:** Bajo — La guía está completa y bien alineada.

---

## 2) Identificación de unidad y alcance

| Campo | Valor |
|-------|-------|
| **Unidad** | 2 – Procedimientos |
| **Tema central** | Definición y uso de procedimientos para estructurar código |
| **Subtemas detectados** | Definición de procedimiento, sintaxis, efecto, llamada a procedimientos, documentación (propósito, precondición, indentación), errores comunes, preguntas de reflexión |
| **Prerrequisitos asumidos** | Unidad 1: comandos nativos, ejecución secuencial, operaciones parciales |
| **Documentos usados** | `programa 2024.docx`, `Planificación 2025.docx`, `BasesConceptualesProg.pdf`, `Unidad 02 Procedimientos - Teórica.odt`, `Práctica 02 Procedimientos_.docx` |

---

## 3) Alineación con Programa (programa 2024 + planificación 2025)

### 3.1 Mapa de objetivos ↔ cobertura

| Objetivo/resultado esperado (del programa) | Estado | Evidencia en Teórica | Observación |
|--------------------------------------------|--------|----------------------|-------------|
| Definir procedimientos simples | **Cubierto** | Sección "Definición de un procedimiento" con sintaxis | OK |
| Nombrar procedimientos descriptivamente | **Cubierto** | "Asigna un nombre descriptivo que comience con mayúscula" | OK |
| Documentar procedimientos (propósito, precondición) | **Cubierto** | Sección "Documentación y buenas prácticas" + conexión con Unidad 1 | OK (mejorado en v1) |
| Reutilización de código | **Cubierto** | Mencionado como beneficio + ejemplo comparativo | OK |
| Llamada a procedimientos | **Cubierto** | Sección "Llamada a procedimientos" | OK |

### 3.2 Secuenciación y tiempo

- **¿Respeta la secuencia sugerida por planificación?** Sí.
- **¿Hay temas adelantados o atrasados?** Las preguntas de reflexión adelantan parámetros (Unidad 4), lo cual es intencional y pedagógicamente válido.

---

## 4) Correspondencia con BasesConceptualesProg.pdf

### Verificación de cambios aplicados desde v1

| Hallazgo v1 | Estado | Evidencia |
|-------------|--------|-----------|
| Definición formal de procedimiento | **Resuelto** | "Un procedimiento es una acción definida por el programador" |
| Concepto de "efecto" | **Resuelto** | "A este cambio que produce el procedimiento en el tablero lo llamamos efecto" |
| Conexión precondición con Unidad 1 | **Resuelto** | "Recordá que en la Unidad 1 vimos que algunas operaciones son parciales..." |
| Procedimientos no retornan valores | **Ignorado** | Decisión del docente: no anticipar conceptos sin marco de referencia |
| Conexión pedagógica "crear nuestro propio comando" | **Resuelto** | "crear un procedimiento es como crear nuestro propio comando" |

### Hallazgos nuevos (v2)

No se detectaron nuevos hallazgos conceptuales.

---

## 5) Coherencia Teórica ↔ Práctica

| Contenido exigido por Práctica 02 | ¿Presente en Teórica? | Observación |
|-----------------------------------|----------------------|-------------|
| Definir procedimientos con `procedure` | Sí | OK |
| Nombrar procedimientos descriptivamente | Sí | OK |
| Documentar propósito y precondición | Sí | OK + conectado con Unidad 1 |
| Indentación correcta | Sí | OK |
| Reutilización de procedimientos | Sí | OK |

**Desajuste pendiente (de v1):**
- **Práctica 02, Ejercicio 11:** Dice "Poner_8_Azules que ponga **5** bolitas" — posible typo. Pendiente de decisión del docente.

---

## 6) Observaciones pedagógicas y de claridad

### Mejoras aplicadas
- La conexión "crear nuestro propio comando" en la introducción facilita la transición desde Unidad 1.
- El concepto de "efecto" conectado con "propósito" en la documentación es muy claro.
- La conexión de precondición con operaciones parciales refuerza la continuidad entre unidades.

### Observación menor
- La palabra "identación" aparece en el texto. La forma correcta en español es **"indentación"** (del inglés *indentation*). Es un detalle ortográfico menor.

---

## 7) Lista de cambios recomendados (backlog)

| Prioridad | Cambio propuesto | Ubicación sugerida | Justificación |
|-----------|------------------|--------------------|---------------|
| **Baja** | Corregir "identación" → "indentación" | Sección "Documentación y buenas prácticas" | Ortografía |

---

## 8) Preguntas abiertas (para el docente)

1. **Typo en Práctica 02 (pendiente de v1):** Ejercicio 11 dice "Poner_8_Azules que ponga **5** bolitas". ¿Corregir a 8 o a 5?

---

**Fin del informe v2.**
