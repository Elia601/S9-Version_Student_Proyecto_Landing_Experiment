# S9-Version_Student_Proyecto_Landing_Experiment

Descripción del proyecto
La tienda online está probando dos versiones de su landing page (A y B) para aumentar la conversión. 

El objetivo es analizar el comportamiento de los usuarios, verificar la calidad de los datos y validar si la nueva versión (B) tiene una tasa de conversión significativamente mayor que la actual (A).Dataset

Archivo ab_project.csv con 40,000 registros:user_id - ID de usuariolanding - versión de landing (A / B)converted - si hubo conversión (0 / 1)dispositivo - tipo de dispositivotraffic_source - fuente de tráficouser_type - nuevo / recurrenteregion - Norte, Centro, Sur, Occidentefecha

Objetivos:
Realizar EDA y revisar balance de grupos A/BCalcular la tasa de conversión general y por segmentos
Plantear hipótesis estadísticasAplicar pruebas z-test y t-test para validar significancia
Dar una recomendación de negocio

Pasos:
1.- RealizadosCarga y limpieza de datos, 
2.-Verificación de duplicados y nulos.
3. Conteo de categorías:landing: A=19982, B=20018 (grupos balanceados)region, dispositivo, traffic_source, user_typeconverted: análisis de desbalance de conversión
4.- Cálculo de conversión por versión: groupby('landing')['converted'].mean()
Gráficos de conversión por dispositivo, fuente y región.
Pruebas de hipótesis:H0: No hay diferencia entre A y BH1: B tiene mayor conversión que A
Nivel de significancia alfa = 0.05Interpretación de p-value y toma de decisión.

Recomendaciones de negocio:

Recomendación 1: Implementar la página B al 100%. Genera 
68.75 vs $61.09) y 682 conversiones más que A. Es la que genera mayor valor económico, aunque la tasa de conversión sea similar.
Recomendación 2: Optimizar presupuesto de marketing. Mantener Organic por volumen (44% de las ventas) pero aumentar inversión en Email (14.99% conversión) y Ads (14.74%) que son los canales con mejor ROI. No crear estrategias diferenciadas por tipo de usuario porque no hay diferencia (14.35% vs 14.09%).
