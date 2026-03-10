# Análisis Alura Store

## Descripción

Análisis de datos de ventas para identificar cuál de las 4 tiendas de Alura Store debería ser vendida. Se evaluó ingresos, satisfacción de clientes, productos vendidos y costos de envío.

## Objetivo

Ayudar al Sr. Juan a decidir qué tienda vender para iniciar un nuevo emprendimiento, basándose en análisis de datos concretos.

## Datos Analizados

- **4 Tiendas**: tienda_1 a tienda_4
- **Total de transacciones**: 9,435 registros
- **Columnas principales**: Producto, Categoría, Precio, Costo de envío, Calificación, Ubicación

## Análisis Realizado

### Paso 1: Exploración de Datos
- Carga de archivos CSV con Pandas
- Análisis de estructura y valores faltantes
- Estadísticas básicas por tienda

### Paso 2: Análisis de Ingresos
- Ingresos totales por tienda
- Precio promedio y rango de precios

### Paso 3: Análisis de Categorías
- Productos vendidos por categoría
- Distribución de categorías en cada tienda

### Paso 4: Productos Más y Menos Vendidos
- Top 10 productos por tienda
- Productos con menor demanda

### Paso 5: Análisis Logístico
- Costo de envío promedio por tienda
- Eficiencia operacional

### Extra: Análisis Geográfico
- Distribución de ventas por ubicación
- Ingresos por región
- Patrones geográficos en cada tienda

## Hallazgos Clave

| Métrica | Store 1 | Store 2 | Store 3 | Store 4 |
|---------|---------|---------|---------|---------|
| Ingresos | $1,150.88B | $1,116.34B | $1,098.02B | $1,038.38B |
| Transacciones | 2,359 | 2,359 | 2,359 | 2,358 |
| Precio Promedio | $487,867 | $473,227 | $465,459 | $440,362 |
| Rating Promedio | 2.77/5 | 2.75/5 | 2.76/5 | 2.72/5 |

## Recomendación

**Vender: Store 4**

### Justificación:
1. **Ingresos más bajos**: $1,038.38B (11% menos que Store 1)
2. **Rating más bajo**: 2.72/5 (satisfacción reducida)
3. **Precio promedio menor**: $440,362 (menos competitividad)
4. **Costo de envío alto**: Sin compensar en volumen de ventas
5. **Margen reducido**: Combinación de bajos ingresos y altos costos

## Visualizaciones

Se generaron 6 gráficos principales:

1. **Ingresos Totales** - Gráfico de barras comparativo
2. **Distribución de Categorías** - Gráficos de pastel por tienda
3. **Top 10 Productos** - Barras horizontales (Store 1)
4. **Costo de Envío Promedio** - Gráfico de barras comparativo
5. **Distribución Geográfica** - Scatter plot con coordenadas
6. **Ingresos por Ubicación** - Análisis regional

## Estructura del Proyecto

```
ALURA-Alura-Store/
├── datos/
│   ├── tienda_1.csv
│   ├── tienda_2.csv
│   ├── tienda_3.csv
│   └── tienda_4.csv
├── notebooks/
│   └── alura_store.ipynb
├── resultados/
│   ├── grafico_ingresos.png
│   ├── grafico_categorias.png
│   ├── grafico_productos_top.png
│   ├── grafico_envios.png
│   ├── grafico_distribucion_geografica.png
│   └── grafico_ingresos_por_ubicacion.png
└── README.md
```

## Cómo Usar

1. Abre `notebooks/alura_store.ipynb` en Jupyter o Google Colab
2. Ejecuta todas las celdas de código
3. Los gráficos se guardarán automáticamente en `resultados/`

## Tecnologías Utilizadas

- **Pandas**: Manipulación y análisis de datos
- **Matplotlib**: Visualización de datos
- **NumPy**: Cálculos numéricos

## Conclusión

Basándose en el análisis exhaustivo de datos de ventas, operacionales y geográficos, **Store 4 es la recomendación más sólida para vender**. Su desempeño inferior en todas las métricas clave la convierte en la candidata menos eficiente del grupo.
