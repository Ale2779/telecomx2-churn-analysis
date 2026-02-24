# telecomx2-churn-analysis
📊 Informe Final – Análisis Predictivo de Cancelación (Churn)

El objetivo de este proyecto fue analizar los factores que influyen en la cancelación de clientes (Churn) en Telecom X2 y desarrollar modelos predictivos capaces de identificar clientes con alta probabilidad de evasión.

La cancelación de clientes impacta directamente en los ingresos de la empresa, por lo que anticiparla permite diseñar estrategias de retención efectivas.

🧹 Preparación y Tratamiento de Datos

Se realizaron los siguientes pasos:

Eliminación de identificadores irrelevantes.

Eliminación de registros con valores nulos en la variable objetivo.

Transformación de variables categóricas mediante One-Hot Encoding.

Análisis de desbalance de clases (~73% clientes activos vs ~27% cancelaciones).

División del dataset en 70% entrenamiento y 30% prueba.

Normalización con StandardScaler para modelos sensibles a la escala.

🤖 Modelos Utilizados

Se implementaron dos modelos predictivos:

1️⃣ Regresión Logística

Requiere normalización.

Permite interpretar el impacto de cada variable.

Ofrece buena capacidad de generalización.

2️⃣ Random Forest

No requiere normalización.

Modelo más robusto.

Permite analizar la importancia de variables.

📈 Evaluación de Modelos

Se evaluaron con:

Exactitud (Accuracy)

Precisión

Recall

F1-score

Matriz de Confusión

🔎 Variables Más Relevantes

📌 Según Regresión Logística

Las variables que aumentan la probabilidad de cancelación incluyen:

Contrato mensual

Pago mediante Electronic Check

Servicio de fibra óptica

Mayor cargo mensual

Las variables que reducen la cancelación incluyen:

Mayor antigüedad

Contrato de 1 o 2 años

Mayor gasto total acumulado

📌 Según Random Forest

Las variables más importantes fueron:

Antigüedad del cliente

Cargo total

Cargo mensual

Tipo de contrato

Servicio de internet

Esto confirma que el tiempo de permanencia y el tipo de contrato son determinantes clave.

🧠 Principales Factores que Influyen en la Cancelación

Clientes nuevos tienen mayor probabilidad de cancelar.

Contratos mensuales presentan mayor riesgo.

Métodos de pago manuales muestran mayor evasión.

Cargos mensuales elevados aumentan la probabilidad de churn.

💡 Estrategias de Retención Propuestas

1️⃣ Implementar campañas de fidelización en los primeros meses del cliente.

2️⃣ Incentivar contratos de largo plazo con descuentos.

3️⃣ Ofrecer beneficios a clientes con contrato mensual para migrarlos a planes anuales.

4️⃣ Revisar estructura de precios en clientes con alta factura mensual.

5️⃣ Diseñar alertas predictivas usando el modelo entrenado.

🏆 Conclusión

El análisis permitió identificar patrones claros asociados a la cancelación de clientes.
Los modelos predictivos desarrollados pueden utilizarse como herramienta estratégica para reducir la evasión y mejorar la retención en Telecom X2.

![Matriz de Correlación](images/correlacion.png)
