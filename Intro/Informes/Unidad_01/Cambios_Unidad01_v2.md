# Cambios a Aplicar: Unidad 01 Teórica

**Versión:** 2 (post-corrección)  
**Fecha:** 2026-02-04  
**Archivo a modificar:** `Teórica/Unidad 01 Teórica.odt`  
**Basado en:** `Informes/Informe_Unidad01_v2.md`

---

## Estado de cambios de v1

Todos los cambios de `Cambios_Unidad01_v1.md` fueron aplicados correctamente:

| # | Cambio | Estado |
|---|--------|--------|
| 1 | Definición formal de "valor" y "tipo de valor" | ✅ Aplicado |
| 2 | Comando `Sacar` + operaciones totales/parciales + precondición | ✅ Aplicado |
| 3 | Aclarar que el argumento determina el resultado | ✅ Aplicado |
| 4 | Mención de `IrAlBorde`, `VaciarTablero` | ✅ Aplicado |
| 5 | Explicar qué es un "error de tipo" | ✅ Aplicado |

---

## Nuevos cambios detectados en v2

### CAMBIO #1 — Prioridad: BAJA

#### Corregir typo en tabla de comandos

**Ubicación:** Segunda tabla de comandos (la que lista valores posibles), fila de `Sacar`

**Texto actual (con error):**
```
Sacar(color(Colores
```

**Texto corregido:**
```
Sacar(color) | Colores | Azul, Negro, Rojo, Verde
```

---

### CAMBIO #2 — Prioridad: BAJA

#### Agregar referencia cruzada en sección de errores

**Ubicación:** Sección "Errores de tipeo y/o de tipos", después de mencionar `Mover(Azul)`.

**Texto a agregar:**

> Como vimos antes, esto es un **error de tipo**: el comando `Mover` espera una Dirección, no un Color.

---

## Resumen de cambios v2

| # | Prioridad | Tipo | Ubicación | Descripción |
|---|-----------|------|-----------|-------------|
| 1 | Baja | Corregir typo | Tabla de valores posibles | `Sacar(color(Colores` → formato correcto |
| 2 | Baja | Agregar | Sección "Errores de tipeo y/o de tipos" | Referencia cruzada a "error de tipo" |

---

## Verificación de coherencia con Práctica 01

- [x] Todos los contenidos de Práctica 01 están cubiertos en Teórica
- [x] No hay desajustes
- [x] No es necesario modificar la práctica

---

## Cambios NO aplicados

Ninguno.

---

**Fin del documento de cambios v2.**
