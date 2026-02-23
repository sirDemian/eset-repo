# Informe de Revisión: Unidad 02 Teórica — Procedimientos

**Versión:** 1 (revisión inicial)  
**Fecha de revisión:** 2026-02-04  
**Archivo revisado:** `Teórica/Unidad 02 Procedimientos - Teórica.docx`  
**Práctica asociada:** `Práctica/Práctica 02 Procedimientos_.docx`

---

## 1) Resumen ejecutivo

**Estado general de alineación:** Media-Alta

**3 principales fortalezas:**
1. Introduce correctamente el concepto de procedimiento con sus tres beneficios (organizar, reutilizar, mantener).
2. Incluye documentación y buenas prácticas (propósito, precondición, indentación) desde el inicio.
3. Sección de errores comunes y preguntas de reflexión bien orientadas pedagógicamente.

**3 principales problemas:**
1. **Falta definición formal de "procedimiento"** según BasesConceptualesProg.pdf — no menciona que es una "acción definida por el programador".
2. **Terminología inconsistente:** Usa "precondición" en documentación pero no la conecta con el concepto de operación parcial de Unidad 1.
3. **Omite el concepto de "efecto"** — qué cambios produce el procedimiento en el tablero (terminología de las bases conceptuales).

**Riesgo pedagógico global:** Medio — Conceptos bien presentados pero falta conexión con terminología formal.

---

## 2) Identificación de unidad y alcance

| Campo | Valor |
|-------|-------|
| **Unidad** | 2 – Procedimientos |
| **Tema central** | Definición y uso de procedimientos para estructurar código |
| **Subtemas detectados** | Definición de procedimiento, sintaxis (procedure, nombre, llaves), llamada a procedimientos, documentación (propósito, precondición, indentación), errores comunes |
| **Prerrequisitos asumidos** | Unidad 1: comandos nativos, ejecución secuencial, concepto de programa |
| **Documentos usados** | `programa 2024.docx`, `Planificación 2025.docx`, `BasesConceptualesProg.pdf`, `Unidad 02 Procedimientos - Teórica.docx`, `Práctica 02 Procedimientos_.docx` |

---

## 3) Alineación con Programa (programa 2024 + planificación 2025)

### 3.1 Mapa de objetivos ↔ cobertura

| Objetivo/resultado esperado (del programa) | Estado | Evidencia en Teórica | Observación |
|--------------------------------------------|--------|----------------------|-------------|
| Definir procedimientos simples | **Cubierto** | Sección "Definición de un procedimiento" con sintaxis | OK |
| Nombrar procedimientos descriptivamente | **Cubierto** | "Asigna un nombre descriptivo que comience con mayúscula" | OK |
| Documentar procedimientos (propósito, precondición) | **Cubierto** | Sección "Documentación y buenas prácticas" | OK |
| Reutilización de código | **Cubierto** | Mencionado como uno de los tres beneficios | OK |
| Llamada a procedimientos | **Cubierto** | Sección "Llamada a procedimientos" | OK |

### 3.2 Secuenciación y tiempo

- **¿Respeta la secuencia sugerida por planificación?** Sí.
- **¿Hay temas adelantados o atrasados?** Las preguntas de reflexión al final adelantan el concepto de parámetros (Unidad 4), lo cual es intencional y pedagógicamente válido.

---

## 4) Correspondencia con BasesConceptualesProg.pdf

### 4.1 Conceptos que deberían estar según las bases

| Concepto de las bases | ¿Presente? | Observación |
|-----------------------|------------|-------------|
| Procedimiento como "acción definida por el programador" | **Parcial** | Dice que "encapsula código" pero no usa la terminología formal |
| Efecto de un procedimiento | **No** | No menciona "efecto" como el cambio que produce en el tablero |
| Procedimiento vs comando nativo | **Parcial** | Implícito en la introducción pero no explícito |
| Subtarea / división del problema | **Parcial** | Menciona "resolver un problema específico" pero no usa "subtarea" |

### 4.2 Hallazgos específicos

| Severidad | Tipo | Descripción | Ubicación |
|-----------|------|-------------|-----------|
| **Media** | Faltante | No define formalmente qué es un procedimiento según las bases: "acción definida por el programador" | Sección "¿Qué es un procedimiento?" |
| **Media** | Faltante | No menciona el concepto de "efecto" (cambio en el tablero) | Sección de definición |
| **Baja** | Inconsistencia | Usa "precondición" en documentación pero no la conecta con Unidad 1 | Sección "Documentación y buenas prácticas" |
| **Baja** | Faltante | No menciona que los procedimientos NO retornan valores (a diferencia de funciones, Unidad 7) | General |

---

## 5) Coherencia Teórica ↔ Práctica

| Contenido exigido por Práctica 02 | ¿Presente en Teórica? | Observación |
|-----------------------------------|----------------------|-------------|
| Definir procedimientos con `procedure` | Sí | OK |
| Nombrar procedimientos descriptivamente | Sí | OK |
| Documentar propósito y precondición | Sí | OK |
| Indentación correcta | Sí | OK |
| Reutilización de procedimientos | Sí | OK |
| Ejercicios de transición (líneas de longitud variable) | Sí | Preguntas de reflexión preparan para parámetros |

**Desajustes detectados:**
- La práctica pide "Poner_8_Azules que ponga **5** bolitas" — posible typo en la práctica (dice 8 en el nombre pero 5 en la descripción).

---

## 6) Observaciones pedagógicas y de claridad

### Fortalezas
- Buen ejemplo comparativo (sin procedimientos vs con procedimientos).
- Las preguntas de reflexión al final son excelentes para motivar la siguiente unidad.
- Sección de errores comunes muy útil para principiantes.

### Oportunidades de mejora
- **Conexión con Unidad 1:** Podría mencionar explícitamente que los procedimientos son como "crear nuestros propios comandos".
- **Terminología formal:** Agregar que un procedimiento es una "acción definida por el programador" y que produce un "efecto" en el tablero.
- **Precondición:** Conectar con el concepto de operación parcial de Unidad 1.

---

## 7) Lista de cambios recomendados (backlog)

| Prioridad | Cambio propuesto | Ubicación sugerida | Justificación |
|-----------|------------------|--------------------|---------------|
| **Alta** | Agregar definición formal: "Un procedimiento es una acción definida por el programador" | Sección "¿Qué es un procedimiento?" | Alineación con BasesConceptualesProg.pdf |
| **Alta** | Introducir el concepto de "efecto": el cambio que produce el procedimiento en el tablero | Después de "siempre modifican el tablero" | Terminología formal de las bases |
| **Media** | Conectar "precondición" con operaciones parciales de Unidad 1 | Sección "Documentación y buenas prácticas" | Coherencia conceptual entre unidades |
| **Media** | Agregar que los procedimientos NO retornan valores (anticipando funciones) | Al final de la definición | Preparación para Unidad 7 |
| **Baja** | Mencionar explícitamente que crear procedimientos es como "crear nuestros propios comandos" | Introducción | Conexión pedagógica con Unidad 1 |

---

## 8) Preguntas abiertas (para el docente)

1. **¿Querés introducir el término "efecto" formalmente?** Las bases conceptuales lo usan para describir qué hace un procedimiento. Podría agregarse junto a "propósito".

2. **¿Conectar precondición con Unidad 1?** En Unidad 1 se introdujo "precondición" para operaciones parciales. ¿Querés hacer referencia explícita a eso en la documentación de procedimientos?

3. **Typo en Práctica 02:** El ejercicio 11 dice "Poner_8_Azules que ponga **5** bolitas". ¿Es intencional o debería ser 8?

---

**Fin del informe v1.**
