# Informe de Revisión: Unidad 05 Teórica — Condicional Simple (if-else)

**Versión:** 1 (revisión inicial)  
**Fecha de revisión:** 2026-02-15  
**Archivo revisado:** `Teórica/Unidad 05 if-else - Teórica.docx`  
**Práctica asociada:** `Práctica/Práctica 05 if - else_.docx`

---

## 1) Resumen ejecutivo

**Estado general de alineación:** Media

**3 principales fortalezas:**

1. Buena conexión con unidades anteriores: menciona que hasta ahora los programas eran secuenciales o repetitivos, y ahora toman decisiones.
2. Ejemplo motivador del buscaminas para explicar la necesidad del `else`.
3. Introduce `puedeMover`, `hayBolitas` y `nroBolitas` como herramientas para construir condiciones.

**3 principales problemas:**

1. **No introduce el tipo Booleano (Verdadero/Falso)** — Las funciones `puedeMover` y `hayBolitas` "devuelven verdadero o falso", pero no se formaliza como un nuevo tipo del sistema de tipos. Es una oportunidad de ampliar la tabla de tipos.
2. **No formaliza el concepto de "expresión booleana" o "condición"** — Dice que la condición "se evalúa como verdadera o falsa" pero no le da nombre al tipo de valor ni explica qué es una expresión.
3. **"identación" en vez de "indentación"** — Mismo error que ya se corrigió en Unidad 3.

**Riesgo pedagógico global:** Medio — Funcional pero falta formalizar conceptos clave del sistema de tipos.

---

## 2) Identificación de unidad y alcance

| Campo | Valor |
|-------|-------|
| **Unidad** | 5 – Condicional Simple (if-else) |
| **Tema central** | Estructura de control condicional para toma de decisiones |
| **Subtemas detectados** | Definición de condicional, sintaxis if, extensión else, uso en procedimientos, comandos nativos (puedeMover, hayBolitas, nroBolitas), buenas prácticas, errores comunes, preguntas de reflexión |
| **Prerrequisitos asumidos** | Unidad 1-2: comandos, procedimientos. Unidad 3: repeat, estructura de control. Unidad 4: parámetros |
| **Documentos usados** | `programa 2024.docx`, `Planificación 2025.docx`, `BasesConceptualesProg.pdf`, `Unidad 05 if-else - Teórica.docx`, `Práctica 05 if - else_.docx` |

---

## 3) Alineación con Programa (programa 2024 + planificación 2025)

### 3.1 Mapa de objetivos ↔ cobertura

| Objetivo/resultado esperado (del programa) | Estado | Evidencia en Teórica | Observación |
|--------------------------------------------|--------|----------------------|-------------|
| Comprender la estructura condicional if | **Cubierto** | Sección "¿Qué es una estructura condicional?" con sintaxis y ejemplo | OK |
| Comprender la extensión else | **Cubierto** | Sección "Extensión del condicional: if-else" con ejemplo motivador | OK |
| Usar condicionales en procedimientos | **Cubierto** | Sección "Uso de condiciones en procedimientos" | OK |
| Conocer funciones nativas para condiciones | **Cubierto** | Sección "Comandos nativos" con puedeMover, hayBolitas, nroBolitas | OK |
| Comprender el tipo Booleano | **No cubierto** | Dice "verdadero o falso" pero no formaliza el tipo | Faltante |
| Comprender qué es una expresión/condición | **Parcial** | Dice "expresión que se evalúa como verdadera o falsa" pero no profundiza | Oportunidad |

### 3.2 Secuenciación y tiempo

- **¿Respeta la secuencia sugerida por planificación?** Sí.
- **¿Hay temas adelantados o atrasados?** No. Las preguntas de reflexión anticipan combinación if+repeat, coherente con la progresión.

---

## 4) Correspondencia con BasesConceptualesProg.pdf

### 4.1 Hallazgos específicos

| Severidad | Tipo | Descripción | Ubicación |
|-----------|------|-------------|-----------|
| **Alta** | Faltante | No introduce el tipo Booleano como nuevo tipo del sistema de tipos. `puedeMover` y `hayBolitas` devuelven valores booleanos, pero no se nombra el tipo. La tabla de tipos debería ampliarse: Direcciones, Colores, Números, **Booleanos**. | Sección "Comandos nativos" / nueva sección |
| **Alta** | Terminología | Llama "comandos nativos" a `puedeMover`, `hayBolitas` y `nroBolitas`, pero estos no son comandos (no producen efecto). Son **expresiones** o **funciones** que devuelven un valor. Esto es una distinción importante: un comando produce un efecto, una expresión devuelve un valor. | Sección "Comandos nativos" |
| **Media** | Faltante | No explica qué es una "condición" formalmente. Dice "expresión que se evalúa como verdadera o falsa" pero no conecta con el tipo Booleano ni con el concepto de expresión. | Sección "¿Qué es una estructura condicional?" |
| **Media** | Inconsistencia | `nroBolitas(color)` devuelve un Número, no un Booleano. Está listado junto a `puedeMover` y `hayBolitas` que sí devuelven booleanos. Debería aclararse que `nroBolitas` no es directamente una condición sino que se puede usar en comparaciones. | Sección "Comandos nativos" |
| **Baja** | Ortografía | "identación" → "indentación" (mismo error corregido en Unidad 3) | Sección "Buenas prácticas" |
| **Baja** | Claridad | Dice "Coloca una bolita Roja en la celda actual solo si hay ninguna bolita Azul" — debería ser "solo si hay alguna bolita Azul" o "solo si no hay ninguna bolita Azul". Ambiguo. | Ejemplo básico (Propósito) |

---

## 5) Coherencia Teórica ↔ Práctica

| Contenido exigido por Práctica 05 | ¿Presente en Teórica? | Observación |
|-----------------------------------|----------------------|-------------|
| Uso de if simple | Sí | OK |
| Uso de if-else | Sí | OK |
| puedeMover(direccion) | Sí | OK |
| hayBolitas(color) | Sí | OK |
| nroBolitas(color) | Sí | Pero no aclara que devuelve Número, no Booleano |
| Condicionales en procedimientos | Sí | OK |
| Documentación | Sí | OK |

**Observaciones sobre la Práctica 05:**

- **"identación" en requisitos:** Mismo error que en la teórica.
- **Ejercicio 10:** Pide "Deja 5 bolitas del color col en la celda inicial" — no parece requerir if/else. Está en la sección "Reflexión para la próxima unidad", probablemente anticipa el uso de expresiones o funciones. ¿Es intencional?
- **Ejercicio 11:** Excelente ejercicio que combina dos condiciones (hay celda + hay bolita). Anticipa operadores lógicos.
- **Preguntas guía:** Mencionan "condiciones que evalúan valores externos a los datos del tablero" y "cumplir dos condiciones a la vez" — buena anticipación de operadores lógicos y funciones.

---

## 6) Observaciones pedagógicas y de claridad

### Fortalezas

- El ejemplo del buscaminas es excelente para motivar el `else`.
- La progresión if → if-else → uso en procedimientos es clara.
- Los errores comunes (olvidar llaves, condiciones inválidas) son muy pertinentes.

### Oportunidades de mejora

- **Formalizar tipo Booleano:** Es el momento natural para ampliar la tabla de tipos con Booleanos (Verdadero, Falso). Esto conecta con el sistema de tipos progresivo de las unidades anteriores.
- **Distinguir "comando" de "expresión/función":** `puedeMover` y `hayBolitas` no son comandos (no producen efecto). Son expresiones que devuelven un valor. Esta distinción es fundamental y debería formalizarse.
- **Aclarar `nroBolitas`:** Devuelve un Número, no un Booleano. No es directamente una condición.

---

## 7) Lista de cambios recomendados (backlog)

| Prioridad | Cambio propuesto | Ubicación sugerida | Justificación |
|-----------|------------------|--------------------|---------------|
| **Alta** | Introducir tipo Booleano y ampliar tabla de tipos | Nueva sección o junto a "Comandos nativos" | Formalizar el nuevo tipo que aparece con las condiciones |
| **Alta** | Distinguir "comando" (produce efecto) de "expresión/función" (devuelve valor). Renombrar sección "Comandos nativos" | Sección "Comandos nativos" | puedeMover y hayBolitas no son comandos |
| **Media** | Aclarar que `nroBolitas` devuelve un Número, no un Booleano | Sección "Comandos nativos" | Evitar confusión sobre qué se puede usar como condición |
| **Media** | Formalizar qué es una "condición" (expresión booleana) | Sección "¿Qué es una estructura condicional?" | Conectar con tipo Booleano |
| **Baja** | Corregir "identación" → "indentación" | Sección "Buenas prácticas" |  Ortografía (ya corregido en Unidad 3) |
| **Baja** | Corregir "solo si hay ninguna bolita Azul" → aclarar sentido | Ejemplo básico (Propósito) | Ambigüedad |

---

## 8) Preguntas abiertas (para el docente)

1. **¿Introducir el tipo Booleano formalmente?** Es el momento natural. Propuesta: ampliar la tabla de tipos con Booleanos (Verdadero, Falso) y explicar que `puedeMover` y `hayBolitas` devuelven valores de este tipo.

2. **¿Distinguir "comando" de "expresión/función"?** `puedeMover`, `hayBolitas` y `nroBolitas` no son comandos (no producen efecto). ¿Querés introducir el término "expresión" o "función" en esta unidad, o preferís dejarlo para más adelante?

3. **¿Ejercicio 10 de la práctica es intencional?** Pide "Deja 5 bolitas del color col" sin aparente necesidad de if/else. ¿Anticipa funciones/expresiones?

4. **¿Corregir "identación" → "indentación" en teórica y práctica?** (Mismo error que Unidad 3)

---

**Fin del informe v1.**
