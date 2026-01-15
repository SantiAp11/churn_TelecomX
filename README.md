# Análisis de Churn - TelecomX

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-green.svg)
![Status](https://img.shields.io/badge/Status-Completado-success.svg)

## Descripción del Proyecto

Proyecto de análisis de churn (abandono de clientes) para TelecomX, desarrollado como parte del Challenge de Ciencia de Datos del programa ONE (Oracle Next Education).

El objetivo es identificar los factores que influyen en la deserción de clientes y generar insights accionables para desarrollar estrategias de retención efectivas.

---

## Objetivos

- Analizar el comportamiento de abandono de clientes
- Identificar factores críticos asociados al churn
- Generar insights y recomendaciones estratégicas
- Desarrollar capacidades de análisis de datos profesional

---

## Estructura del Proyecto
```
churn_TelecomX/
│
├── data/
│   ├── raw/                    # Datos originales
│   │   └── TelecomX_raw.csv
│   └── processed/              # Datos procesados
│       └── TelecomX_clean.csv
│
├── notebooks/
│   ├── 00_setup.ipynb                  # Configuración del proyecto
│   ├── 01_extraccion_datos.ipynb       # Extracción desde API
│   ├── 02_limpieza_datos.ipynb         # Limpieza y transformación
│   └── 03_analisis_exploratorio.ipynb  # EDA e informe final
│
└── README.md
```

---

## Proceso de Análisis

### 1. Extracción de Datos
- Descarga desde API de GitHub
- 7,267 registros iniciales
- 21 variables extraídas

### 2. Limpieza y Transformación
- Conversión de tipos de datos
- Eliminación de valores nulos (235 registros)
- Estandarización de variables categóricas
- Creación de variable derivada: cargo diario
- Dataset final: 7,032 registros

### 3. Análisis Exploratorio (EDA)
- Análisis descriptivo completo
- Análisis de churn por variables categóricas
- Análisis de churn por variables numéricas
- Matriz de correlaciones
- Identificación de patrones

---

## Hallazgos Principales

### Tasa de Churn General
- 26.58% de los clientes abandonan el servicio
- 1,869 clientes abandonaron
- 5,163 clientes permanecen activos

### Factores Críticos Identificados

#### 1. Tipo de Contrato (Factor más crítico)
- Contratos mensuales: 42.71% de churn
- Contratos de 1 año: 11.28% de churn
- Contratos de 2 años: 2.85% de churn

#### 2. Método de Pago
- Electronic check: 45.29% de churn
- Pagos automáticos: 15-16% de churn

#### 3. Tipo de Servicio de Internet
- Fiber optic: 41.89% de churn
- DSL: 19.00% de churn

#### 4. Antigüedad del Cliente
- Clientes que abandonan: promedio de 18 meses
- Clientes que permanecen: promedio de 37.7 meses

---

## Insights Clave

1. Período crítico: Los primeros 18 meses son decisivos para la retención
2. Contratos largos reducen el churn hasta en un 93%
3. Problema con Fiber optic: Tasa de churn 2.2x mayor que DSL
4. Pagos automáticos reducen el churn en un 66%
5. Clientes premium abandonan más: Mayor cargo mensual correlaciona con mayor churn

---

## Recomendaciones Estratégicas

### Prioridad Alta
1. Programa de retención para nuevos clientes (primeros 18 meses)
2. Incentivos para contratos largos (15-25% de descuento)
3. Promoción de pagos automáticos (descuentos adicionales)
4. Auditoría técnica de Fiber optic (resolver problemas de calidad)

### Impacto Proyectado
- Reducción esperada del churn: 15-40%
- Nueva tasa objetivo: 16-22%
- Ahorro anual estimado: $1.5-4M

---

## Tecnologías Utilizadas

- Python 3.8+
- Pandas: Manipulación y análisis de datos
- NumPy: Operaciones numéricas
- Matplotlib: Visualizaciones
- Seaborn: Gráficos estadísticos
- Jupyter Notebook: Desarrollo interactivo
- Google Colab: Entorno de ejecución
- Git/GitHub: Control de versiones

---

## Resultados del Proyecto

### Métricas del Dataset
- 7,032 clientes analizados
- 22 variables estudiadas
- 0 valores nulos en dataset final
- 100% de datos procesados correctamente

### Análisis Realizados
- Estadísticas descriptivas completas
- 6 variables categóricas analizadas
- 5 variables numéricas comparadas
- Matriz de correlaciones generada

---

## Cómo Usar Este Proyecto

### Requisitos
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Ejecución
1. Clonar el repositorio:
```bash
git clone https://github.com/SantiAp11/churn_TelecomX.git
cd churn_TelecomX
```

2. Abrir los notebooks en orden:
   - 00_setup.ipynb
   - 01_extraccion_datos.ipynb
   - 02_limpieza_datos.ipynb
   - 03_analisis_exploratorio.ipynb

3. Ejecutar las celdas secuencialmente

---

## Estructura de Notebooks

### Notebook 00: Setup
Configuración inicial del proyecto y estructura de carpetas

### Notebook 01: Extracción
- Conexión con API de GitHub
- Descarga de datos
- Aplanamiento de estructura JSON
- Guardado en data/raw/

### Notebook 02: Limpieza
- Detección de valores nulos
- Conversión de tipos de datos
- Estandarización de variables
- Transformación a formato binario
- Guardado en data/processed/

### Notebook 03: Análisis Exploratorio
- Estadísticas descriptivas
- Análisis de churn por categorías
- Análisis de variables numéricas
- Correlaciones
- Informe ejecutivo completo

---

## Autor

Santiago Aparicio Pérez
- Proyecto: Challenge ONE - Ciencia de Datos
- Programa: Oracle Next Education (ONE)
- Fecha: Diciembre 2024 - Enero 2025

---

## Licencia

Este proyecto fue desarrollado con fines educativos como parte del programa ONE.

---

## Agradecimientos

- Oracle Next Education (ONE) por el programa de formación
- Alura Latam por el contenido educativo
- TelecomX (empresa ficticia) por los datos del challenge

---

## Contacto

Preguntas o sugerencias sobre el proyecto:
- GitHub: [@SantiAp11](https://github.com/SantiAp11)
- Email: santiagoaparicioperez674@gmail.com
