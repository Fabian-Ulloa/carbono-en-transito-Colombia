# 🌍 Carbono en tránsito: ¿Colombia importa o exporta CO₂?

Proyecto de análisis de datos con Python y Jupyter Notebook — Universitaria Agraria de Colombia (Grupo S).

## Integrantes y reparto del trabajo

| Integrante | ID | Parte | Archivo |
|---|---|---|---|
| Luis Fabián Ulloa Rodríguez | 45210 | **Parte 1:** carga, exploración y limpieza | `01 Luis Fabian.ipynb` |
| Luis Andrés Santos Cortés | 45297 | **Parte 2:** visualización (3 gráficos) | `02 Luis Andres.ipynb` |
| Michelle Andrea Murillo Gonzalez | 37858 | **Parte 3:** modelo de regresión lineal, interpretación y conclusiones | `03 Michelle.ipynb` |

El archivo `Comercio CO2 Colombia.ipynb` reúne las tres partes en un solo cuaderno, de principio a fin.

## Descripción
Casi siempre se habla de las emisiones que un país *produce*. Pero los países también compran y venden productos cuya fabricación emitió CO₂. Este proyecto usa el dato **"Share of CO₂ emissions embedded in trade"** de Our World in Data para responder:

> ¿Colombia es importador o exportador neto de CO₂ por el comercio, y cómo ha cambiado desde 1990 hasta el último año disponible?

- **Valor positivo:** el país importa más CO₂ del que exporta (importador neto).
- **Valor negativo:** el país exporta más CO₂ del que importa (exportador neto).
- El valor se expresa como **% de las emisiones que el país produce**.

## Fuente de los datos
- Artículo: [CO₂ and Greenhouse Gas Emissions — Our World in Data](https://ourworldindata.org/co2-emissions)
- Gráfico usado del artículo: *Share of CO₂ emissions embedded in trade* — https://ourworldindata.org/grapher/share-co2-embedded-in-trade
- Datos originales: Global Carbon Budget (2026), con procesamiento de Our World in Data. Desde 1990 hasta el último año disponible.

## Qué hace cada parte
1. **Parte 1 (Luis Fabián):** descarga los datos, explora la tabla, quita repetidos y vacíos, y separa a Colombia.
2. **Parte 2 (Luis Andrés):** gráfico de Colombia por año, comparación con otros países de América y los 10 mayores importadores y exportadores netos.
3. **Parte 3 (Michelle):** regresión lineal (entrena con el 80 % de los años y prueba con el 20 % final), error promedio, predicción, interpretación y conclusiones.

## Sobre el código
El código es sencillo y está pensado para aprender: cada bloque tiene una explicación en español antes del código, comentarios en cada paso y un mini glosario al final de cada cuaderno.

## Cómo ejecutarlo
```bash
pip install -r requirements.txt
jupyter notebook
```
Abrir cualquier cuaderno y ejecutar las celdas en orden con **Shift + Enter**. Se necesita internet para descargar los datos. Cada parte funciona por sí sola.

## Qué aprendió cada integrante
- **Luis Fabián:** Aprendí a descargar datos de internet con Python y a limpiarlos: quitar datos repetidos y vacíos y quedarme solo con los de Colombia.
- **Luis Andrés:** (escribir aquí una o dos frases)
- **Michelle:** Aprendí a hacer una regresión lineal para ver la tendencia de los datos y a interpretar sus resultados, entendiendo que el modelo no predice con exactitud.
## Limitaciones
- No todos los países tienen datos de comercio de buena calidad.
- Solo incluye CO₂ de combustibles fósiles e industria (no uso de la tierra ni deforestación).
- El modelo usa solo el año como variable, por lo que muestra una tendencia general y no predice con exactitud.
