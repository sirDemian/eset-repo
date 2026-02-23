# Informe de Revisión: Unidad 03 Teórica — Repetición Simple (repeat)

**Versión:** 2 (post-corrección)  
**Fecha de revisión:** 2026-02-11  
**Archivo revisado:** `Teórica/Unidad 03 Repeat - Teórica.odt`  
**Práctica asociada:** `Práctica/Práctica 03 Repetición Simple_.docx`  
**Informe anterior:** `Informe_Unidad03_v1.md`

---

## 1) Resumen ejecutivo

**Estado general de alineación:** Alta

**3 principales fortalezas:**
1. Define "estructura de control" formalmente como instrucción que modifica el flujo de ejecución.
2. Introduce el tipo Número con tabla que amplía el sistema de tipos (Direcciones, Colores, Números).
3. Conecta subtarea repetida con el concepto de efecto de Unidad 2.

**Cambios aplicados desde v1:**
1. ~~No definía "estructura de control"~~ → **RESUELTO**
2. ~~No introducía tipo Número~~ → **RESUELTO**
3. ~~"identación" en lugar de "indentación"~~ → **RESUELTO**
4. ~~Faltaba conexión subtarea/efecto~~ → **RESUELTO**

**Riesgo pedagógico global:** Bajo — La guía está completa y bien alineada.

---

## 2) Identificación de unidad y alcance

| Campo | Valor |
|-------|-------|
| **Unidad** | 3 – Repetición Simple (repeat) |
| **Tema central** | Estructura de control `repeat` para repetición de bloques de código |
| **Subtemas detectados** | Definición de estructura de control, sintaxis de repeat, tipo Número, ventajas, combinación con procedimientos, subtarea/efecto, buenas prácticas, errores comunes, preguntas de reflexión |
| **Prerrequisitos asumidos** | Unidad 1: comandos, valores, tipos. Unidad 2: procedimientos, efecto, documentación |
| **Documentos usados** | `programa 2024.docx`, `Planificación 2025.docx`, `BasesConceptualesProg.pdf`, `Unidad 03 Repeat - Teórica.odt`, `Práctica 03 Repetición Simple_.docx` |

---

## 3) Alineación con Programa (programa 2024 + planificación 2025)

### 3.1 Mapa de objetivos ↔ cobertura

| Objetivo/resultado esperado (del programa) | Estado | Evidencia en Teórica | Observación |
|--------------------------------------------|--------|----------------------|-------------|
| Comprender la estructura de repetición simple | **Cubierto** | Definición formal de estructura de control + sintaxis | OK (mejorado en v1) |
| Usar `repeat` con un número fijo de repeticiones | **Cubierto** | Ejemplo con repeat(5) | OK |
| Combinar repeat con procedimientos | **Cubierto** | Sección "Repetición dentro de procedimientos" + conexión subtarea/efecto | OK (mejorado en v1) |
| Identificar ventajas de repeat vs secuencia manual | **Cubierto** | Sección "Ventajas del uso de repeat" | OK |
| Documentar programas con repeat | **Cubierto** | Sección "Buenas prácticas con repeat" | OK |
| Ampliar sistema de tipos con Números | **Cubierto** | Tabla de tipos: Direcciones, Colores, Números | OK (nuevo en v1) |

### 3.2 Secuenciación y tiempo

- **¿Respeta la secuencia sugerida por planificación?** Sí.
- **¿Hay temas adelantados o atrasados?** Las preguntas de reflexión adelantan generalización (parámetros, Unidad 4), lo cual es intencional.

---

## 4) Correspondencia con BasesConceptualesProg.pdf

### Verificación de cambios aplicados desde v1

| Hallazgo v1 | Estado | Evidencia |
|-------------|--------|-----------|
| Definir "estructura de control" | **Resuelto** | "Una estructura de control es una instrucción especial que modifica el flujo de ejecución del programa" |
| Introducir tipo Número | **Resuelto** | Tabla con Direcciones, Colores, Números + "Ahora aparece un nuevo tipo: los Números" |
| Corregir "identación" → "indentación" | **Resuelto** | "Observen la indentación" / "Indentación:" |
| Conectar subtarea con efecto | **Resuelto** | "lo que se repite dentro del repeat es una subtarea..." |

### Hallazgos nuevos (v2)

| Severidad | Tipo | Descripción | Ubicación |
|-----------|------|-------------|-----------|
| **Media** | Imprecisión | La tabla de tipos muestra Números como `...-3, -2, -1, 0, 1, 2, 3, ...` (incluye negativos). Sin embargo, `repeat` requiere un entero **positivo** (el propio texto lo dice). Incluir negativos puede confundir al alumno. Según las bases conceptuales, el tipo Número incluye todos los enteros, pero convendría aclarar que `repeat` solo acepta positivos. | Tabla de tipos en "Definición y sintaxis de repeat" |

---

## 5) Coherencia Teórica ↔ Práctica

| Contenido exigido por Práctica 03 | ¿Presente en Teórica? | Observación |
|-----------------------------------|----------------------|-------------|
| Uso de `repeat` con número fijo | Sí | OK |
| Combinación de repeat con procedimientos | Sí | OK |
| Documentación (propósito, precondición) | Sí | OK |
| Dibujar patrones (líneas, cuadrados, cruces) | Sí | Ejemplo de línea; patrones complejos en práctica |
| Reflexión sobre generalización | Sí | Preguntas guía al final |

**Desajustes corregidos por el docente:**

- **Ejercicio 5:** ✅ Corregido → Ahora dice "DibujarCuadradoAzulDeLadoTres() que dibuje un cuadrado azul de 3x3"
- **Ejercicio 9:** ✅ Eliminado por el docente (MoverHastaElBordeNorte no era adecuado para `repeat`)

---

## 6) Observaciones pedagógicas y de claridad

### Mejoras aplicadas
- La definición de "estructura de control" es clara y conecta bien con el flujo secuencial previo.
- La tabla de tipos es un excelente recurso visual que muestra la progresión del sistema de tipos.
- La conexión subtarea/efecto refuerza la continuidad con Unidad 2.

### Observación nueva
- La tabla de tipos incluye números negativos (`...-3, -2, -1, 0, 1, 2, 3, ...`). Si bien el tipo Número en Gobstones incluye todos los enteros, en el contexto de `repeat` esto puede confundir. Se podría agregar una aclaración: "Si bien el tipo Número incluye todos los enteros, `repeat` solo acepta números positivos."

---

## 7) Lista de cambios recomendados (backlog)

| Prioridad | Cambio propuesto | Ubicación sugerida | Justificación |
|-----------|------------------|--------------------|---------------|
| **Media** | Aclarar que `repeat` solo acepta números positivos, aunque el tipo Número incluya todos los enteros | Después de la tabla de tipos | Evitar confusión con negativos |

---

## 8) Preguntas abiertas (para el docente)

1. **¿Aclarar la restricción de `repeat` sobre números positivos?** La tabla muestra negativos pero `repeat` no los acepta.
2. **Ejercicio 5 de Práctica 03 (pendiente de v1):** Sigue siendo copy-paste del Ejercicio 4. ¿Corregir?
3. **Ejercicio 9 de Práctica 03 (pendiente de v1):** ¿Es intencional para mostrar la limitación de `repeat`?

---

**Fin del informe v2.**
