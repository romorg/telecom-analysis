---📘 Análisis de Clientes y Patrones de Uso — ConnectaTel---
---

🎯 Objetivo del Proyecto
---
Este proyecto tiene como objetivo analizar el comportamiento de los usuarios de ConnectaTel para identificar segmentos de clientes, patrones de uso, outliers relevantes y oportunidades comerciales basadas en datos. El análisis se centra en variables como edad, mensajes, llamadas, minutos de llamadas, y en la creación de segmentos de uso y segmentos por edad.


📂 Datasets Utilizados
---
El proyecto utiliza tres archivos principales:

• users_latam.csv - Contiene información demográfica y de registro de los usuarios.

• usage.csv - Incluye datos de uso del servicio: cantidad de mensajes, llamadas y minutos de llamadas.

• plans.csv - Catálogo de planes disponibles (Básico y Premium).


🔍 Etapas del Análisis
---
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


▶️ Cómo ejecutar el notebook
---
Para ejecutar el notebook incluido en este repositorio:
Navega al archivo .ipynb dentro del repositorio.
Haz clic en “Open in GitHub” para visualizarlo directamente, o selecciona “Download raw file” para descargarlo.
Abre el archivo en tu entorno local usando Jupyter Notebook o Jupyter Lab.
Asegúrate de tener instaladas las dependencias necesarias:
pip install pandas seaborn matplotlib

Ejecuta las celdas en orden para reproducir el análisis completo.
---
🔁 Guía breve de reproducción
Descarga o clona el repositorio:
git clone <URL-del-repositorio>

Ubica los datasets en la carpeta data/:
users_latam.csv
usage.csv
plans.csv

Abre el notebook en tu entorno local:
jupyter notebook

Ejecuta las secciones en orden:
Carga de datos
Limpieza de registros inválidos
Exploración descriptiva
Histogramas y boxplots
Detección de outliers con IQR
Creación de segmentos (grupo_uso, grupo_edad)
Visualizaciones
Conclusiones finales
Verifica las rutas de los archivos dentro del notebook para asegurar que coincidan con tu estructura local.
Revisa los gráficos y tablas generadas para validar los resultados y conclusiones.

---
