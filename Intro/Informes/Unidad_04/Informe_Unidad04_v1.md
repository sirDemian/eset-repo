# Informe de Revisión: Unidad 04 Teórica — Parámetros

**Versión:** 1 (revisión inicial)  
**Fecha de revisión:** 2026-02-15  
**Archivo revisado:** `Teórica/Unidad 04 Parámetros -Teórica.docx`  
**Práctica asociada:** `Práctica/Práctica 04 Parámetros_.docx`

---

## 1) Resumen ejecutivo

**Estado general de alineación:** Media-Alta

**3 principales fortalezas:**
1. Excelente progresión pedagógica: parte de comandos nativos que ya usan parámetros (`Poner(Azul)`, `Mover(Norte)`) para mostrar que ya los conocían.
2. Introduce alcance local de parámetros con ejemplo concreto — concepto avanzado bien dosificado.
3. Buenas prácticas bien detalladas: nombres descriptivos, documentación, cantidad máxima de parámetros como señal de alerta.

**3 principales problemas:**
1. **No hace la distinción formal entre "parámetro" y "argumento"** — decisión predefinida indica que en Unidad 4 debe hacerse esta distinción explícita.
2. **No conecta parámetros con el sistema de tipos** ampliado en Unidad 3 (Números, Colores, Direcciones). Menciona los tipos pero no referencia la tabla de Unidad 3.
3. **Falta mencionar que `repeat` también recibe un parámetro** — oportunidad de conectar con Unidad 3.

**Riesgo pedagógico global:** Medio — Funcional pero falta una distinción terminológica clave.

---

## 2) Identificación de unidad y alcance

| Campo | Valor |
|-------|-------|
| **Unidad** | 4 – Parámetros |
| **Tema central** | Parametrización de procedimientos para generalización |
| **Subtemas detectados** | Definición de parámetros, sintaxis, uso en comandos nativos, uso en procedimientos, múltiples parámetros, alcance local, tipos de parámetros, buenas prácticas, errores comunes, preguntas de reflexión |
| **Prerrequisitos asumidos** | Unidad 1: comandos, tipos. Unidad 2: procedimientos, efecto. Unidad 3: repeat, tipo Número |
| **Documentos usados** | `programa 2024.docx`, `Planificación 2025.docx`, `BasesConceptualesProg.pdf`, `Unidad 04 Parámetros -Teórica.docx`, `Práctica 04 Parámetros_.docx` |

---

## 3) Alineación con Programa (programa 2024 + planificación 2025)

### 3.1 Mapa de objetivos ↔ cobertura

| Objetivo/resultado esperado (del programa) | Estado | Evidencia en Teórica | Observación |
|--------------------------------------------|--------|----------------------|-------------|
| Comprender qué son los parámetros | **Cubierto** | Sección "¿Qué son los parámetros?" con definición y analogía de "caja" | OK |
| Definir procedimientos con parámetros | **Cubierto** | Sección "Definición y sintaxis" con ejemplo de PonerN | OK |
| Usar múltiples parámetros | **Cubierto** | Ejemplo con MoverYPoner(dirección, cantidad, color) | OK |
| Comprender alcance local | **Cubierto** | Sección "Alcance de los parámetros" con ejemplo | OK |
| Distinguir parámetro de argumento | **No cubierto** | Usa "argumento" como sinónimo informal pero no hace la distinción | Decisión predefinida requiere distinción en Unidad 4 |
| Documentar procedimientos con parámetros | **Cubierto** | Sección "Buenas prácticas" | OK |

### 3.2 Secuenciación y tiempo

- **¿Respeta la secuencia sugerida por planificación?** Sí.
- **¿Hay temas adelantados o atrasados?** Las preguntas de reflexión adelantan la idea de verificación (condicionales), coherente con la práctica (Ejercicio 11).

---

## 4) Correspondencia con BasesConceptualesProg.pdf

### 4.1 Conceptos que deberían estar según las bases

| Concepto de las bases | ¿Presente? | Observación |
|-----------------------|------------|-------------|
| Parámetro como variable local | **Cubierto** | Sección "Alcance de los parámetros" |
| Parámetro vs argumento | **No** | Dice "Son como 'argumentos'" pero no distingue formalmente |
| Tipos de parámetros (Números, Colores, Direcciones) | **Cubierto** | Sección "Tipos de parámetros" |
| Generalización mediante parámetros | **Cubierto** | Introducción + ejemplos |

### 4.2 Hallazgos específicos

| Severidad | Tipo | Descripción | Ubicación |
|-----------|------|-------------|-----------|
| **Alta** | Faltante | No distingue "parámetro" (en la definición) de "argumento" (en la llamada). Decisión predefinida: "En Unidad 4 hacer la distinción explícita". Actualmente dice "Son como 'argumentos'" lo cual los iguala en vez de distinguirlos. | Sección "¿Qué son los parámetros?" |
| **Media** | Oportunidad | No conecta con el sistema de tipos ampliado en Unidad 3. La sección "Tipos de parámetros" lista Números, Colores, Direcciones pero no referencia la tabla de tipos de Unidad 3. | Sección "Tipos de parámetros" |
| **Media** | Oportunidad | No menciona que `repeat(n)` también recibe un valor (un número). Sería una buena conexión: "ya usábamos parámetros sin saberlo, no solo en Poner y Mover sino también en repeat". | Sección "Definición y sintaxis" |
| **Baja** | Claridad | La analogía de la "caja" es útil pero podría confundirse con el concepto de variable (que viene después). Considerar si vale la pena ajustarla. | Sección "¿Qué son los parámetros?" |
| **Baja** | Ortografía | "direccion" sin tilde en la sección de buenas prácticas (nombres descriptivos). | Sección "Buenas prácticas" |

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

- **Ejercicio 3:** El propósito dice "Mover al Este" pero el procedimiento se llama `MoverEnDireccionEste(cantidad)`. Esto es correcto pero podría ser una oportunidad perdida: ¿por qué no parametrizar también la dirección? El Ejercicio 4 lo hace (`MoverN(cantidad, direccion)`), así que la progresión es intencional.
- **Ejercicio 11:** Excelente ejercicio de reflexión que anticipa condicionales. Bien alineado con las preguntas guía de la teórica.
- **Buena progresión:** 1 parámetro (Ej. 1-3) → 2 parámetros (Ej. 4-6) → problemas complejos (Ej. 7-10) → reflexión (Ej. 11).

---

## 6) Observaciones pedagógicas y de claridad

### Fortalezas
- La estrategia de mostrar que ya usaban parámetros en comandos nativos es excelente pedagógicamente.
- El concepto de alcance local está bien introducido con un ejemplo concreto.
- La regla de "más de 3 parámetros = señal de alerta" es una buena práctica profesional.
- La viñeta de Mafalda es un buen recurso para distender antes de un tema nuevo.

### Oportunidades de mejora
- **Distinción parámetro/argumento:** Es el momento indicado según la decisión predefinida. Propuesta: "El **parámetro** es el nombre que aparece en la definición del procedimiento (es la 'caja vacía'). El **argumento** es el valor concreto que le pasamos al llamarlo (es lo que ponemos dentro de la caja)."
- **Conexión con Unidad 3:** Mencionar que `repeat(5)` también recibe un argumento, reforzando que ya usaban este mecanismo.

---

## 7) Lista de cambios recomendados (backlog)

| Prioridad | Cambio propuesto | Ubicación sugerida | Justificación |
|-----------|------------------|--------------------|---------------|
| **Alta** | Agregar distinción formal parámetro vs argumento | Sección "¿Qué son los parámetros?", después de la definición actual | Decisión predefinida: hacer distinción explícita en Unidad 4 |
| **Media** | Conectar tipos de parámetros con tabla de tipos de Unidad 3 | Sección "Tipos de parámetros" | Coherencia con sistema de tipos progresivo |
| **Media** | Mencionar que `repeat(n)` también recibe un argumento | Sección "Definición y sintaxis", junto al ejemplo de Poner/Mover | Refuerza que ya usaban parámetros |
| **Baja** | Corregir "direccion" → "dirección" (tilde) | Sección "Buenas prácticas" | Ortografía |

---

## 8) Preguntas abiertas (para el docente)

1. **¿Cómo formular la distinción parámetro/argumento?** Propuesta: "El parámetro es el nombre en la definición (la caja vacía). El argumento es el valor concreto en la llamada (lo que ponemos en la caja)." ¿Te parece bien o preferís otra formulación?

2. **¿La analogía de la "caja" puede confundir con variables?** En unidades futuras se introducen variables. ¿Querés mantener la analogía o ajustarla?

---

**Fin del informe v1.**
