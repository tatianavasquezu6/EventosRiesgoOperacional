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

# Conclusión: PONER CONCLUSIÓN

# 5 Dashboard

