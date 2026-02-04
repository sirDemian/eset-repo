# Informe de Revisión: Unidad 01 Teórica

**Fecha de revisión:** 2026-02-03  
**Archivo revisado:** `Teórica/Unidad 01 Teórica.docx`  
**Práctica asociada:** `Práctica/Práctica 01 Introducción a Gobstones_.docx`

---

## 1) Resumen ejecutivo

**Estado general de alineación:** Media

**3 principales fortalezas:**
1. Cubre correctamente los conceptos de programa, comandos nativos (`Mover`, `Poner`), valores y tipos de valores (Colores, Direcciones).
2. Introduce el entorno Gobstones con descripción visual del tablero, celdas, cabezal y bolitas.
3. Incluye sección pedagógica sobre errores ("Equivocarse es aprender") alineada con la filosofía del programa.

**3 principales problemas:**
1. **No define formalmente "valor" ni "tipo de valor"** como conceptos abstractos; solo los enumera. El programa y las bases conceptuales esperan una introducción conceptual más explícita.
2. **Omite el comando `Sacar`** y la distinción entre operaciones totales y parciales (presente en BasesConceptualesProg y mencionada implícitamente en el programa).
3. **No menciona `IrAlBorde` ni `VaciarTablero`**, comandos nativos que aparecen en las bases conceptuales como parte del repertorio inicial.

**Riesgo pedagógico global:** Medio — La guía es funcional para arrancar, pero deja huecos conceptuales que pueden generar confusión en unidades posteriores (ej. precondiciones, operaciones parciales).

---

## 2) Identificación de unidad y alcance

| Campo | Valor |
|-------|-------|
| **Unidad** | 1 – Gobstones / Introducción |
| **Tema central** | Qué es un programa, entorno Gobstones, comandos nativos, valores y tipos |
| **Subtemas detectados** | Definición de programa, tablero/celdas/cabezal/bolitas, comandos `Mover` y `Poner`, tipos Colores y Direcciones, flujo secuencial, manejo de errores |
| **Prerrequisitos asumidos** | Ninguno explícito (es la primera unidad) |
| **Documentos usados** | `programa 2024.docx`, `Planificación 2025.docx`, `BasesConceptualesProg.pdf`, `Unidad 01 Teórica.docx`, `Práctica 01 Introducción a Gobstones_.docx` |

---

## 3) Alineación con Programa (programa 2024 + planificación 2025)

### 3.1 Mapa de objetivos ↔ cobertura

| Objetivo/resultado esperado (del programa) | Estado | Evidencia en Teórica | Observación |
|--------------------------------------------|--------|----------------------|-------------|
| Conocer el entorno de desarrollo Gobstones | **Cubierto** | Sección "¿Qué es Gobstones?" y "Conociendo Gobstones" con descripción visual | OK |
| Entender el concepto de valores | **Parcial** | Menciona valores (colores, direcciones) pero no define formalmente qué es un "valor" | Falta definición conceptual |
| ¿Qué es un programa? / ¿Qué es programar? | **Cubierto** | Sección "Introducción" con definición de programa | OK |
| Introducción a Valores y Tipos de valores | **Parcial** | Lista Colores y Direcciones, pero no explica qué es un "tipo" como abstracción | Falta concepto de "tipo" |
| Acciones y Comandos, diferencias | **Parcial** | Menciona "comandos son descripciones de acciones" pero no profundiza la distinción | Podría ser más explícito |
| Comandos nativos: Mover, Poner | **Cubierto** | Tabla con comandos, tipos de valor y ejemplos | OK |
| Ejecución secuencial de un programa | **Cubierto** | Sección "Flujo de un programa" | OK |

### 3.2 Secuenciación y tiempo

- **¿Respeta la secuencia sugerida por planificación?** Sí. La planificación indica período 5/3–12/3 para Unidad 1 con contenidos de entorno, valores, tipos, comandos nativos.
- **¿Hay temas adelantados o atrasados?** No se detectan temas fuera de secuencia. Sin embargo, la guía menciona "argumentos" y "parámetros" de forma informal; el concepto formal de parámetros corresponde a Unidad 4.

---

## 4) Correspondencia con BasesConceptualesProg.pdf

### Hallazgo 1: Definición de "valor" ausente

| Campo | Detalle |
|-------|---------|
| **Severidad** | Medio |
| **Tipo** | Definición |
| **Evidencia en Teórica** | "Estos Valores pueden ser agrupados en diferentes grupos llamados Tipos de Valores" |
| **Evidencia en BasesConceptualesProg** | Definición 2.2.6: "Un valor es un elemento abstracto que representa información..." |
| **Diagnóstico** | La guía usa "valor" sin definirlo; asume que el estudiante entiende el concepto |
| **Recomendación** | Agregar una definición breve de "valor" antes de enumerar Colores y Direcciones |

### Hallazgo 2: Comando `Sacar` omitido

| Campo | Detalle |
|-------|---------|
| **Severidad** | Bajo |
| **Tipo** | Alcance |
| **Evidencia en Teórica** | Solo menciona `Mover` y `Poner` |
| **Evidencia en BasesConceptualesProg** | Tabla T.2.1 incluye `Sacar(< color >)` como comando básico con precondición |
| **Diagnóstico** | `Sacar` no es estrictamente necesario en Unidad 1, pero su omisión impide introducir el concepto de precondición y operación parcial |
| **Recomendación** | Evaluar si conviene mencionar `Sacar` brevemente para anticipar precondiciones, o dejarlo para unidad posterior (pregunta para el docente) |

### Hallazgo 3: Operaciones totales vs. parciales no explicadas

| Campo | Detalle |
|-------|---------|
| **Severidad** | Medio |
| **Tipo** | Definición / prerequisito |
| **Evidencia en Teórica** | Menciona que `Mover` fuera del tablero genera error, pero no usa terminología "operación parcial" ni "precondición" |
| **Evidencia en BasesConceptualesProg** | Definiciones 2.2.13–2.2.15: operación total, operación parcial, precondición |
| **Diagnóstico** | El estudiante ve el error pero no adquiere el vocabulario técnico que usará en unidades posteriores |
| **Recomendación** | Introducir brevemente los términos "operación total" (Poner) y "operación parcial" (Mover) con sus precondiciones |

### Hallazgo 4: Comandos `IrAlBorde` y `VaciarTablero` no mencionados

| Campo | Detalle |
|-------|---------|
| **Severidad** | Bajo |
| **Tipo** | Alcance |
| **Evidencia en Teórica** | No aparecen |
| **Evidencia en BasesConceptualesProg** | Tabla T.2.1 los lista como comandos básicos |
| **Diagnóstico** | No son críticos para Unidad 1; pueden introducirse más adelante |
| **Recomendación** | Dejar para unidad posterior o mencionar como "otros comandos nativos que veremos" |

---

## 5) Coherencia Teórica ↔ Práctica

| Contenido exigido por Práctica 01 | ¿Presente en Teórica? | Observación |
|-----------------------------------|----------------------|-------------|
| Comando `Mover` | Sí | OK |
| Comando `Poner` | Sí | OK |
| Tipos Colores y Direcciones | Sí | OK |
| Ejecución secuencial | Sí | OK |
| Manejo de errores (cabezal fuera de tablero) | Sí | Sección "Equivocarse es aprender" |
| Concepto de "tablero inicial" y "tablero final" | Sí | Mencionado en flujo de programa |

**Desajustes detectados:** Ninguno crítico. La práctica no exige contenidos que la teoría no introduzca.

**Observación menor:** La práctica pregunta "¿Cómo decide Gobstones el tipo de bolita que coloca cuando usas el comando Poner?" — la teoría no explica que el tipo lo determina el argumento (valor) pasado; podría ser más explícita.

---

## 6) Observaciones pedagógicas y de claridad

- **Punto confuso:** "A los valores que van dentro de los paréntesis los llamamos argumentos" — luego dice "los comandos pueden recibir argumentos". La distinción argumento/parámetro no se aclara (parámetros se ven en Unidad 4). Podría generar confusión terminológica.
- **Falta motivación:** No se explica *por qué* existen tipos de valores ni qué problema resuelven. Solo se listan.
- **Falta ejemplo de error de tipo:** La sección de errores muestra `Mover(Azul)` pero no explica formalmente que es un error de tipo (valor incorrecto para el tipo esperado).
- **Progresión de ejemplos:** Adecuada (básico → error → interpretación de mensajes).

---

## 7) Lista de cambios recomendados (backlog)

| Prioridad | Cambio propuesto | Ubicación sugerida | Justificación |
|-----------|------------------|--------------------|---------------|
| **Alto** | Agregar definición formal de "valor" y "tipo de valor" | Después de "Conociendo Gobstones", antes de la tabla de comandos | Programa y bases conceptuales lo requieren |
| **Medio** | Introducir términos "operación total" y "operación parcial" con ejemplos (`Poner` vs `Mover`) | Sección "Flujo de un programa" o nueva subsección | Alinear vocabulario con bases conceptuales |
| **Medio** | Aclarar que el argumento determina el tipo de bolita/dirección (responde pregunta de práctica) | Después de la tabla de comandos | Coherencia teoría-práctica |
| **Bajo** | Mencionar existencia de `Sacar`, `IrAlBorde`, `VaciarTablero` como "otros comandos que veremos" | Final de la guía o nota al pie | Anticipar contenido sin profundizar |
| **Bajo** | Explicar brevemente qué es un "error de tipo" en la sección de errores | Sección "Errores de tipeo y/o de tipos" | Ya muestra el ejemplo pero no lo nombra formalmente |

---

## 8) Preguntas abiertas (para el docente)

1. **¿Se espera introducir `Sacar` en Unidad 1 o se deja para más adelante?** — Las bases conceptuales lo listan como comando básico, pero el programa no lo menciona explícitamente en Unidad 1.
2. **¿Se quiere usar la terminología "operación total/parcial" y "precondición" desde Unidad 1, o se introduce gradualmente?** — Afecta cuánto vocabulario técnico agregar ahora.
3. **¿El término "argumento" se usa intencionalmente para distinguirlo de "parámetro" (Unidad 4), o es intercambiable en este contexto?** — Conviene definir convención para evitar confusión.

---

**Fin del informe.**
