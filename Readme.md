# ETL End-to-End
### Prueba Corta 4 — TI6900 Inteligencia de Negocios

---

## Descripción del proyecto

Este proyecto trabaja sobre el dataset de Kaggle **`btcusd_1-min_data.csv`** (1,048,576 filas · 6 columnas). El objetivo principal fue aplicar conceptos de análisis de datos para comunicar la información recabada a partir de datos históricos del precio del Bitcoin.

---

## Stack técnico

| Herramienta | Uso |
|---|---|
| **Tableau Prep Builder** | Preparación, limpieza y transformación del dataset |
| **Tableau Desktop** | Comunicación de *data insights* mediante dashboards comprensibles |

---

## Conceptos clave

**Vela** — Representación de lo que ocurrió con el precio de un activo durante un periodo determinado.

**Cerro** — Venta realizada.

**Alta** — El activo fue vendido a un precio mayor al que fue comprado originalmente.

**Baja** — El activo fue vendido a un precio menor al que fue comprado originalmente.

---

## Lo que se hizo

### 1. Perfilamiento inicial

Se analizó el dataset identificando **5 preguntas de negocio** y aplicando un proceso de limpieza para trabajar con el dataset sin inconsistencias.

### 2. Reglas de transformación y limpieza

Se aplicaron las siguientes transformaciones:

- **Eliminación de nulls** en la columna `Timestamp`.
- **Columna `Actividad`** — Determina si hubo actividad en ese minuto (campo compuesto por cadenas).
- **Columna `Rango de vela`** — Indica si la vela cerró al alza o a la baja.
- **Columna `Fecha`** — Convierte los valores no nulos de `Timestamp` de formato UNIX/ASCII a formato `Date`.

---

## Estructura del proyecto

```
📦 proyecto/
├── 📂 datos_originales/
│   └── 📄 dataset
│
├── 📂 datos_preparados/
│   ├── 📄 archivo de Tableau Prep Builder
│   └── 📄 archivo de Tableau con visualizaciones
│
└── 📂 documentacion/
    └── 📄 TI6900_PC4.pdf
```
