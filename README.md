# Retos 2 y 3 - Programación SIG (UNAL)

Entrega del taller ArcPy de la asignatura *Programacion en SIG*,
Maestria en Geomatica, Universidad Nacional de Colombia, 2026-1.

## 🔗 Ver entrega online

**[Abrir el HTML interactivo →](https://linaq11.github.io/Retos-2-y-3-clase/retos_arcpy_2_3.html)**

(También disponible como `retos_arcpy_2_3.pdf` para descarga offline.)

## Contenido

- `retos_arcpy_2_3.qmd` - fuente Quarto con tablas, resultados y PNGs en base64.
- `retos_arcpy_2_3.html` - render autocontenido para abrir en cualquier navegador.
- `retos_arcpy_2_3.pdf` - versión PDF para revisión offline.
- `figures_pig/` - PNGs originales (25 archivos = 5 escenarios x 5 tipos).

## Cobertura

| Reto | Tema | Función central |
|---|---|---|
| 2 | Propiedades del Feature Class | `arcpy.Describe()` |
| 3 | Validar y crear Feature Dataset | `arcpy.Exists()`, `CreateFeatureDataset()` |
| 6-8 | Filtrar y exportar | `MakeFeatureLayer`, `SelectLayerByAttribute`, `CopyFeatures` |
| 13-14 | Puente ArcPy <-> NumPy | `FeatureClassToNumPyArray`, `NumPyArrayToTable` |
| 15 | Edición en sitio | `UpdateCursor` |

## Resultados sobre Test.gdb (escenario spring)

- 7 363 puntos de telemetría sobre las 7 aves rastreadas.
- 1 039 registros de Folkert exportados (~14 % del total).
- 202 puntos con filtro ambiental (viento + vuelo activo).
- Velocidad promedio 0,4256 m/s sobre 7 356 registros válidos.
- Correlación maxima del modelo: rho(va_mtss, vw_mtss) = 0,945.

## Como regenerar

`quarto render retos_arcpy_2_3.qmd --to html`

## Autora

Lina Maria Quintero Fonseca - 2026-05-26
