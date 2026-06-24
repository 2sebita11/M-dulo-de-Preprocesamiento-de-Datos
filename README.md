prompt-engineering-data-science.
Repositorio colaborativo de prompts técnicos para la Tecnicatura Superior en Ciencia de Datos e IA.
# 📂 Repositorio Técnico: Módulo de Preprocesamiento de Datos

**Descripción:** Plantilla técnica optimizada para la automatización de la limpieza de valores faltantes (`NaN`) en DataFrames de Pandas, discriminando estrategias por tipo de variable (numérica/categorica) sin alterar la fuente original.

---

## ⚙️ Parámetros de Configuración (Placeholders)
Al reutilizar este prompt, el Científico de Datos debe reemplazar los siguientes campos según las necesidades del proyecto:

| Variable / Placeholder | Descripción | Valores Soportados | Valor por Defecto |
| :--- | :--- | :--- | :--- |
| `{{DATASET_VARIABLE}}` | Nombre de la variable del DataFrame en Python. | Variable de tipo `pd.DataFrame` | *Obligatorio* |
| `{{ESTRATEGIA_NUMERICA}}`| Método de imputación para variables cuantitativas. | `'mean'`, `'median'`, `'mode'` | `'mean'` |
| `{{ESTRATEGIA_CATEGORICA}}`| Método de imputación para variables cualitativas. | `'mode'`, `'constant'` (ej. 'Desconocido')| `'mode'` |
| `{{UMBRAL_ELIMINACION}}` | Criterio para borrar filas completamente vacías. | `'all'` (toda la fila), `'any'` (al menos un nulo)| `'all'` |

---

## 📋 Instrucciones de Uso para el Equipo
1. Copiar el prompt del repositorio técnico.
2. Reemplazar las variables entre llaves `{{ }}` con los requerimientos específicos de su pipeline de datos.
3. Ejecutar en el entorno de IA generativa para obtener el código productivo.
4. Validar el reporte por consola emitido por la función `clean_missing_values`.
