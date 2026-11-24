# Eventos de Riesgo Operacional
Evidencias de trabajo relacionado con los eventos de riesgo operacional, transformaciones de la data y visualizaciones asociadas.

# 1. Caso de negocio
En la Cooperativa se registran eventos de riesgo operacional asociados con fallas de procesos, errores humanos, incidentes tecnológicos, deficiencias de control, proveedores y otras causas. La Superintendencia Financiera de Colombia exige que en las entidades financieras se lleve un histórico con la información histórica de los eventos de riesgo operacional, sin embargo, esta información es susceptible de ser analizada para identificar tendencias, eventos con causas recurrentes que requieran planes de tratamientos de riesgo y estimaciones de exposición económica o pérdidas potenciales. 

<img width="794" height="470" alt="image" src="https://github.com/user-attachments/assets/0bb48ee4-9390-4bf4-8de1-7747854116df" />

# 2. Beneficios
El presente proyecto busca convertir registros históricos en información útil para identificar tendencias, tomar acciones preventivas y correctivas y medir exposición económica. Se esperan los siguientes beneficios: Reducir el tiempo para consolidar, depurar y analizar eventos; visibilizar procesos, causas y categorías que concentran frecuencia y pérdidas; incorporar estimaciones cuantitativas de pérdida esperada y del VaR; apoyar la priorización de procesos, controles y acciones de mitigación; facilitar el seguimiento de cambios en frecuencia, severidad y distribución de pérdidas.

# 3. Arquitectura

<img width="865" height="437" alt="image" src="https://github.com/user-attachments/assets/f18128da-afdb-4e11-8a54-412698231652" />

# 4. Pipeline

Se realiza ingesta de datos en Databricks con estructura medallion (bronze, silver y gold), y para ello se ejecuta el proceso en 6 diferentes etapas secuenciales:

# 4.1 Inspección de datos

<img width="1120" height="342" alt="image" src="https://github.com/user-attachments/assets/06d2f0fe-0b3d-4f7f-87a2-1503a653be76" />

<img width="964" height="378" alt="image" src="https://github.com/user-attachments/assets/72bce5cc-07e0-4986-97d7-aecf1f4d1a9d" />

# 4.2 Etapa Bronze

<img width="1149" height="420" alt="image" src="https://github.com/user-attachments/assets/b2c8474c-1381-4eaa-bb85-7dbf9438a388" />

<img width="932" height="245" alt="image" src="https://github.com/user-attachments/assets/cbfc60a4-dc13-490c-9f11-0e1f0a542d0d" />

# 4.3 Etapa Silver

<img width="1137" height="515" alt="image" src="https://github.com/user-attachments/assets/04f326a4-4858-4cd4-8448-57f1f832add7" />

<img width="979" height="462" alt="image" src="https://github.com/user-attachments/assets/421cb6b3-822e-45a7-af32-54734815237c" />

<img width="975" height="390" alt="image" src="https://github.com/user-attachments/assets/520924c6-2ccb-45ac-b3b5-947ebf44bbf1" />

<img width="959" height="374" alt="image" src="https://github.com/user-attachments/assets/935f292b-9687-4ebf-80df-df5a8bbf3843" />

<img width="973" height="331" alt="image" src="https://github.com/user-attachments/assets/e0533969-c995-43d1-9a73-74ea481013c0" />

# 4.4 Etapa Gold

<img width="1181" height="533" alt="image" src="https://github.com/user-attachments/assets/52aca7f1-2234-48cd-931b-40b2ee776aad" />

<img width="964" height="362" alt="image" src="https://github.com/user-attachments/assets/30f4190d-75a4-4187-9d19-e848fa1e2825" />

<img width="855" height="481" alt="image" src="https://github.com/user-attachments/assets/5d5c986b-be1b-4d55-bc36-71eb756f77a7" />

# 4.5 Etapa Controles de Calidad

<img width="1134" height="550" alt="image" src="https://github.com/user-attachments/assets/cdd8da76-8a72-4207-a5b4-f272246ff140" />

<img width="1004" height="314" alt="image" src="https://github.com/user-attachments/assets/b91f72b6-ba29-4b86-9e83-2363e34fe099" />

<img width="977" height="474" alt="image" src="https://github.com/user-attachments/assets/b22e688a-09c9-4712-9ef3-4b3823785532" />

# 4.6 Cálculo del VaR

m<img width="1143" height="333" alt="image" src="https://github.com/user-attachments/assets/951a656b-4696-4a5c-a099-4f06c0037e3a" />

<img width="979" height="420" alt="image" src="https://github.com/user-attachments/assets/ce9ebc1c-e182-434b-a5ab-071795bb408b" />

# Conclusión: Los resultados obtenidos durante el desarrollo del proyecto fueron satisfactorios y permitieron evidenciar el valor de la analítica de datos como herramienta de apoyo para la gestión del riesgo operacional. El análisis exploratorio de datos (EDA) facilitó la identificación de patrones, tendencias, concentraciones y comportamientos relevantes en los eventos y las pérdidas históricas, proporcionando una visión más amplia de la exposición de la entidad al riesgo operacional.

De igual manera, los análisis estadísticos y los procedimientos implementados para el cálculo del VaR, así como sus resultados, son coherentes y reflejan comportamientos razonables y consistentes con la realidad de la entidad, así como con las estimaciones y referencias de exposición a pérdidas disponibles a la fecha.

# Modelos de ciencia de datos

El proyecto utiliza técnicas de análisis y modelamiento de datos para comprender el comportamiento de los eventos de riesgo operacional y estimar las posibles pérdidas asociadas.

El desarrollo contempla dos componentes principales:

Análisis exploratorio de datos (EDA): permite examinar la información histórica, identificar tendencias, patrones, concentraciones de eventos y comportamientos de las pérdidas, facilitando la comprensión de la exposición al riesgo operacional de la entidad.

Simulación de Monte Carlo: permite realizar múltiples simulaciones de posibles escenarios de pérdidas, tomando como referencia el comportamiento histórico de los eventos. A partir de estas simulaciones se estiman indicadores tales como el VaR. 

Estos componentes permiten complementar el análisis histórico con estimaciones de pérdidas potenciales y generar información que contribuya al seguimiento y la gestión del riesgo operacional.

# 5 Dashboard

Se diseñó un tablero de control que consolida indicadores clave para la gestión del riesgo operacional, proporcionando información de valor para el seguimiento y la toma de decisiones. El análisis se centra principalmente en los eventos tipo A, que generan pérdidas económicas, y los eventos tipo B, que no producen impacto económico, así como en su distribución a través de los diferentes procesos y categorías. Adicionalmente, el tablero incorpora el cálculo del Valor en Riesgo (VaR) con niveles de confianza del 95% y 99%, permitiendo estimar la exposición potencial a pérdidas bajo distintos escenarios: un escenario moderado con un nivel de confianza del 95% y un escenario extremo o de mayor severidad con un nivel de confianza del 99%.

<img width="1512" height="653" alt="Tablero 1" src="https://github.com/user-attachments/assets/5c5fb881-fa11-4d12-abb0-9f1925454878" />

<img width="1508" height="363" alt="Tablero 2" src="https://github.com/user-attachments/assets/e0e37959-7730-49a3-b648-f2aca8cb605c" />

<img width="1506" height="543" alt="Tablero 3" src="https://github.com/user-attachments/assets/64ea476a-e612-4ae4-aca1-86ac2319a75a" />

<img width="1505" height="424" alt="Tablero 4" src="https://github.com/user-attachments/assets/0fc96eca-aa02-4b28-821d-303ee140e8d2" />

<img width="1501" height="262" alt="Tablero 5" src="https://github.com/user-attachments/assets/f1a21958-0ad1-47c9-a8ac-d32762050efa" />

