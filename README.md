📘 Análisis de Clientes y Patrones de Uso — ConnectaTel

🎯 Objetivo del Proyecto

Este proyecto tiene como objetivo analizar el comportamiento de los usuarios de ConnectaTel para identificar segmentos de clientes, patrones de uso, outliers relevantes y oportunidades comerciales basadas en datos. El análisis se centra en variables como edad, mensajes, llamadas, minutos de llamadas, y en la creación de segmentos de uso y segmentos por edad.

---

📂 Datasets Utilizados

El proyecto utiliza tres archivos principales:

• users_latam.csv - Contiene información demográfica y de registro de los usuarios.

• usage.csv - Incluye datos de uso del servicio: cantidad de mensajes, llamadas y minutos de llamadas.

• plans.csv - Catálogo de planes disponibles (Básico y Premium).

---
🔍 Etapas del Análisis
1. Carga y exploración inicial
• Lectura de los datasets con pandas.
• Revisión de estructura, tipos de datos y valores faltantes.
• Identificación de registros inválidos (ej. fechas futuras).
2. Limpieza de datos
• Eliminación de 40 registros con fechas imposibles (año 2026).
• Validación de rangos de edad.
• Revisión de duplicados y consistencia general.
3. Análisis descriptivo
• Cálculo de estadísticas básicas (describe()).
• Histogramas para visualizar distribuciones.
• Boxplots para detectar valores extremos.
4. Detección de outliers
• Aplicación del método IQR para:
	◦ cant_mensajes
	◦ cant_llamadas
	◦ cant_minutos_llamada
• Decisión sobre mantener o revisar outliers según su naturaleza.
5. Segmentación
• Segmentos por uso: Bajo uso, Uso medio, Alto uso.
• Segmentos por edad: Joven, Adulto, Adulto Mayor.
• Clasificación mediante condiciones lógicas en Pandas.
6. Visualización
• Gráficos de barras para distribución de segmentos.
• Análisis cruzado entre grupos de uso y edad.
7. Conclusiones accionables
• Identificación de segmentos valiosos.
• Recomendaciones comerciales basadas en patrones detectados.
