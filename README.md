# Análisis de Retención de Clientes en el Sector de Telecomunicaciones

## Descripción del Proyecto
Este proyecto desarrolla un análisis exploratorio y descriptivo sobre el comportamiento de abandono (churn) de clientes en una compañía de telecomunicaciones. El objetivo principal es identificar los factores demográficos, financieros y de servicio que correlacionan con la pérdida de usuarios para proporcionar recomendaciones basadas en datos que mitiguen este impacto económico.

## Estructura de los Datos
El conjunto de datos original se obtuvo en formato JSON con estructuras anidadas, representando la información de los clientes, los servicios contratados y los cargos financieros.

Las variables principales analizadas incluyen:
- **Datos de Cliente:** Antigüedad, género y perfil demográfico.
- **Servicios:** Tipo de conexión a internet, seguridad en línea y soporte técnico.
- **Información Financiera:** Contratos, métodos de pago, cargos mensuales y cargos totales.

## Metodología y Procesamiento
El flujo de trabajo se dividió en cuatro fases técnicas:

1. **Normalización y Limpieza:**
   - Desanidación de estructuras JSON a formato tabular (Pandas DataFrame).
   - Conversión de tipos de datos (coerción de variables de texto a numéricas en cargos totales).
   - Tratamiento de registros incompletos y eliminación de valores nulos.

2. **Ingeniería de Características:**
   - Creación de la métrica `Cuentas_Diarias` para evaluar la presión financiera por jornada.
   - Codificación binaria de la variable objetivo (Churn) para análisis estadístico.
   - Estandarización de la nomenclatura de columnas para mejorar la legibilidad del código.

3. **Análisis Descriptivo:**
   - Cálculo de medidas de tendencia central y dispersión.
   - Segmentación de métricas financieras comparando clientes activos frente a los que han abandonado el servicio.

4. **Visualización Exploratoria:**
   - Análisis de frecuencia de variables categóricas.
   - Estudio de la distribución de densidad en variables numéricas (antigüedad y facturación).

## Hallazgos Principales
- **Impacto del Contrato:** Los clientes bajo contratos mensuales presentan una tasa de abandono significativamente mayor en comparación con los contratos a largo plazo.
- **Factor de Antigüedad:** Existe una concentración crítica de abandono en los primeros seis meses de
