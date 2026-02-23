# Cambios a Aplicar: Unidad 04 Teórica — Parámetros

**Versión:** 1 (inicial)  
**Fecha:** 2026-02-15  
**Archivo a modificar:** `Teórica/Unidad 04 Parámetros -Teórica.docx`  
**Basado en:** `Informes/Unidad_04/Informe_Unidad04_v1.md`

---

## Cambios propuestos

### CAMBIO #1 — Prioridad: ALTA

#### Agregar distinción formal parámetro vs argumento

**Ubicación:** Sección "¿Qué son los parámetros?", después de:
> "Son como 'argumentos' que le indican al procedimiento cómo debe actuar."

**Texto propuesto (agregar a continuación):**

> Ahora que introducimos formalmente los parámetros, es un buen momento para distinguir dos términos que hasta ahora usamos como sinónimos:
>
> - **Parámetro:** Es el nombre que aparece en la **definición** del procedimiento. Es la "caja vacía" que espera recibir un valor. Ejemplo: en `procedure PonerN(cantidad, color)`, `cantidad` y `color` son parámetros.
> - **Argumento:** Es el valor concreto que le pasamos al **llamar** al procedimiento. Es lo que ponemos dentro de la caja. Ejemplo: en `PonerN(5, Azul)`, `5` y `Azul` son argumentos.
>
> En resumen: el parámetro es el nombre, el argumento es el valor.

---

### CAMBIO #2 — Prioridad: MEDIA

#### Conectar tipos de parámetros con tabla de tipos de Unidad 3

**Ubicación:** Sección "Tipos de parámetros", reemplazar la lista actual por una versión que referencie la tabla de Unidad 3.

**Texto actual:**
> En Gobstones, los parámetros pueden ser de distintos tipos de valores, como:
> Números: Para controlar la cantidad de repeticiones.
> Colores: Para decidir qué color de bolita colocar.
> Direcciones: Para mover el cabezal en una dirección específica.

**Texto propuesto:**

> En Gobstones, los parámetros pueden recibir valores de cualquiera de los tipos que ya conocemos (recordá la tabla de tipos de la Unidad 3):
>
> | Tipo | Ejemplo de uso como argumento | ¿Para qué? |
> |------|------------------------------|-------------|
> | Números | `PonerN(5, Azul)` | Controlar cantidades o repeticiones |
> | Colores | `PonerN(3, Rojo)` | Decidir qué color de bolita colocar |
> | Direcciones | `MoverN(4, Norte)` | Mover el cabezal en una dirección específica |

---

### CAMBIO #3 — Prioridad: MEDIA

#### Mencionar que `repeat` y comandos nativos también reciben argumentos

**Ubicación:** Sección "Definición y sintaxis", en la parte donde muestra el ejemplo de `Poner(Azul)` y `Mover(Norte)`.

**Texto a agregar (después de la tabla de Poner):**

> De hecho, no solo los comandos nativos reciben argumentos. En la Unidad 3 ya usábamos `repeat(5)` pasándole un número como argumento. Ahora aprenderemos a hacer lo mismo con nuestros propios procedimientos.

---

### CAMBIO #4 — Prioridad: BAJA

#### Corregir "direccion" → "dirección" (tilde)

**Ubicación:** Sección "Buenas prácticas al usar parámetros", en la lista de nombres descriptivos.

**Texto actual:** `direccion`  
**Texto corregido:** `dirección`

---

## Resumen de cambios v1

| # | Prioridad | Tipo | Ubicación | Descripción |
|---|-----------|------|-----------|-------------|
| 1 | Alta | Agregar | "¿Qué son los parámetros?" | Distinción formal parámetro vs argumento |
| 2 | Media | Modificar | "Tipos de parámetros" | Conectar con tabla de tipos de Unidad 3 |
| 3 | Media | Agregar | "Definición y sintaxis" | Mencionar que repeat también recibe argumentos |
| 4 | Baja | Corregir | "Buenas prácticas" | "direccion" → "dirección" |

---

## Preguntas pendientes para el docente

1. **¿Te parece bien la formulación de la distinción parámetro/argumento?** "El parámetro es el nombre en la definición. El argumento es el valor en la llamada."

2. **¿La analogía de la "caja" puede confundir con variables?** En unidades futuras se introducen variables. ¿Mantener la analogía o ajustarla?

---

**Fin del documento de cambios v1.**
