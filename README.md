# telecom-analysis
agregar version final: Análisis ConnectaTel
🔍 Etapas del Análisis Realizadas
1. Carga y exploración inicial de datos
• Lectura de los datasets.
• Revisión de estructura, tipos de datos y valores faltantes.
• Detección de registros inválidos (ej. fechas futuras en reg_date).
2. Limpieza de datos
• Eliminación de 40 registros con fechas imposibles (año 2026).
• Validación de rangos de edad.
• Revisión de valores extremos en variables de uso.
3. Análisis descriptivo
• Cálculo de estadísticas básicas (media, mediana, percentiles).
• Visualización con histogramas y boxplots para detectar outliers.
4. Detección de outliers
• Uso del método IQR para identificar valores extremos en:
	◦ cant_mensajes
	◦ cant_llamadas
	◦ cant_minutos_llamada
• Decisión sobre mantener o revisar outliers según su naturaleza.
5. Creación de segmentos
• Segmentos por uso: Bajo uso, Uso medio, Alto uso.
• Segmentos por edad: Joven, Adulto, Adulto Mayor.
• Clasificación mediante funciones lógicas en Pandas.
6. Visualización de segmentos
• Gráficos de barras para distribución de grupos de uso y edad.
• Análisis cruzado para identificar patrones relevantes.
7. Conclusiones accionables
• Identificación de segmentos valiosos.
• Recomendaciones comerciales basadas en patrones de uso.
• Propuestas de nuevos planes y estrategias de retención.
