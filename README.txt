Business Analytics for an E-commerce Startup
1. Project Description
This project provides a comprehensive analysis of business metrics for an e-commerce startup. The primary objective is to analyze data from marketing, user behavior, and sales to identify unprofitable marketing channels and optimize the advertising budget.

The analysis is based on three datasets: user visit logs, order logs, and marketing cost logs, covering the period from June 2017 to May 2018.

2. Key Business Questions Addressed
The analysis is structured to answer the following critical business questions:

Product: How do people use the product? (DAU, WAU, MAU, session length, user retention).

Sales: When do users start buying? What is the average purchase size? How much money do they generate (LTV)?

Marketing: How much was spent on marketing? What is the cost of acquiring a customer (CAC)? How profitable are the marketing investments (ROMI)?

3. Analysis Methodology
The project was carried out in a Jupyter Notebook (Analisis de negocio.ipynb) and followed these key steps:

a. Data Preprocessing
Loaded three separate CSV files (visits, orders, costs) into Pandas DataFrames.

Cleaned and prepared the data by standardizing column names and converting data types, especially dates to datetime format.

Enriched the data by creating new columns for time-based analysis, such as session_date, session_month, and cohort_month.

b. Product Analytics
Calculated key user engagement metrics:

DAU (Daily Active Users), WAU (Weekly Active Users), and MAU (Monthly Active Users).

Average Session Length (ASL).

Sticky Factor (DAU/MAU) to measure user retention and engagement.

c. Sales Analytics
Performed funnel analysis to determine the conversion time from a user's first visit to their first purchase.

Calculated the Average Order Value (AOV) to understand the typical purchase size.

Conducted a Cohort Analysis to calculate the Lifetime Value (LTV) of customers over time. The results were visualized using a heatmap to show cumulative LTV.

d. Marketing Analytics
Calculated total marketing expenditure and broke it down by acquisition source.

Determined the Customer Acquisition Cost (CAC) for each marketing channel by linking costs to the number of new customers acquired.

Calculated the Return on Marketing Investment (ROMI) for each source using the 6-month LTV as a benchmark to evaluate channel profitability.

4. Key Findings & Recommendations
Findings: The business shows healthy fundamentals with strong user conversion (most users buy on their first day) and good retention, with customer value more than doubling in the first year. However, the analysis revealed a significant inefficiency in marketing spend: the largest portion of the budget is allocated to Source 3, which has the highest CAC and the lowest ROMI. In contrast, Source 1 is the most profitable channel.

Recommendation: It is recommended to reallocate the marketing budget by reducing spending on the underperforming Source 3 and increasing investment in the most profitable channels: Source 1, followed by Sources 2 and 5. This strategic shift will optimize costs and maximize the return on investment.

5. Technologies and Libraries Used
Python 3

Pandas: For data manipulation and analysis.

Seaborn & Matplotlib: For generating graphs and visualizations.

Análisis de Negocio para una Startup de E-commerce
1. Descripción del Proyecto
Este proyecto presenta un análisis completo de las métricas de negocio para una startup de comercio electrónico. El objetivo principal es analizar los datos de marketing, comportamiento de usuarios y ventas para identificar los canales de marketing no rentables y optimizar el presupuesto publicitario.

El análisis se basa en tres conjuntos de datos: registros de visitas de usuarios, registros de pedidos y registros de costos de marketing, cubriendo el período de junio de 2017 a mayo de 2018.

2. Preguntas Clave del Negocio Abordadas
El análisis está estructurado para responder a las siguientes preguntas críticas de negocio:

Producto: ¿Cómo usan las personas el producto? (DAU, WAU, MAU, duración de la sesión, retención de usuarios).

Ventas: ¿Cuándo comienzan a comprar los usuarios? ¿Cuál es el tamaño promedio de compra? ¿Cuánto dinero generan (LTV)?

Marketing: ¿Cuánto se gastó en marketing? ¿Cuál es el costo de adquisición de un cliente (CAC)? ¿Qué tan rentables fueron las inversiones (ROMI)?

3. Metodología del Análisis
El proyecto se llevó a cabo en un Jupyter Notebook (Analisis de negocio.ipynb) y siguió los siguientes pasos clave:

a. Preprocesamiento de Datos
Se cargaron tres archivos CSV distintos (visits, orders, costs) en DataFrames de Pandas.

Se limpiaron y prepararon los datos estandarizando los nombres de las columnas y convirtiendo los tipos de datos, especialmente las fechas a formato datetime.

Se enriquecieron los datos creando nuevas columnas para el análisis basado en el tiempo, como session_date, session_month y cohort_month.

b. Analítica de Producto
Se calcularon métricas clave de engagement del usuario:

DAU (Usuarios Activos Diarios), WAU (Usuarios Activos Semanales) y MAU (Usuarios Activos Mensuales).

Duración Promedio de la Sesión (ASL).

Sticky Factor (DAU/MAU) para medir la retención y el compromiso del usuario.

c. Analítica de Ventas
Se realizó un análisis de embudo para determinar el tiempo de conversión desde la primera visita de un usuario hasta su primera compra.

Se calculó el Valor Promedio de Pedido (AOV) para entender el tamaño de compra típico.

Se llevó a cabo un Análisis de Cohortes para calcular el Valor de Vida del Cliente (LTV) a lo largo del tiempo. Los resultados se visualizaron usando un mapa de calor para mostrar el LTV acumulado.

d. Analítica de Marketing
Se calculó el gasto total en marketing y se desglosó por fuente de adquisición.

Se determinó el Costo de Adquisición de Cliente (CAC) para cada canal de marketing, vinculando los costos con el número de nuevos clientes adquiridos.

Se calculó el Retorno de la Inversión en Marketing (ROMI) para cada fuente, utilizando el LTV a 6 meses como punto de referencia para evaluar la rentabilidad de los canales.

4. Conclusiones y Recomendaciones Clave
Conclusiones: El negocio muestra fundamentos sólidos con una fuerte conversión de usuarios (la mayoría compra en su primer día) y una buena retención, con un valor del cliente que se duplica en el primer año. Sin embargo, el análisis reveló una ineficiencia significativa en el gasto de marketing: la mayor parte del presupuesto se asigna a la Fuente 3, que tiene el CAC más alto y el ROMI más bajo. En contraste, la Fuente 1 es el canal más rentable.

Recomendación: Se recomienda reasignar el presupuesto de marketing, reduciendo el gasto en la Fuente 3 de bajo rendimiento y aumentando la inversión en los canales más rentables: Fuente 1, seguida por las Fuentes 2 y 5. Este cambio estratégico optimizará los costos y maximizará el retorno de la inversión.

5. Tecnologías y Librerías Utilizadas
Python 3

Pandas: Para la manipulación y el análisis de datos.

Seaborn & Matplotlib: Para la generación de gráficos y visualizaciones.