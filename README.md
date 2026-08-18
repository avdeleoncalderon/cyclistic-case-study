# 🚲 Cyclistic Bike-Share Case Study

Análisis de datos de viajes de bike-share (Divvy/Cyclistic, Chicago) para identificar 
diferencias de comportamiento entre ciclistas con membresía anual y ciclistas ocasionales, 
como parte del Google Data Analytics Professional Certificate.

## Business TaskAnalizar los datos históricos de viajes de Cyclistic para identificar diferencias de comportamiento entre ciclistas con membresía anual (members) y ciclistas ocasionales (casual), con el fin de generar insights que sustenten una estrategia de marketing orientada a convertir ciclistas ocasionales en miembros anuales.

## Proceso (Ask → Prepare → Process → Analyze → Share → Act)
El análisis completo, con documentación paso a paso, está en 
[`notebook.ipynb`](./notebook.ipynb).

## Principales hallazgos
- Los members hacen ~10.6x más viajes, pero de menor duración (mediana 8.5 min vs 23.1 min).
- Los members muestran un patrón claro de "commute" (picos 7-9h y 16-18h entre semana).
- Los casual riders concentran su actividad en fines de semana y tardes, con uso más 
  recreativo.

## Herramientas
Python (Pandas, Matplotlib, Seaborn) en Jupyter Notebook.

## Datos
Divvy Trip Data (2019 Q1, 2020 Q1), datos públicos de Motivate International Inc. 
bajo [Divvy Data License Agreement](https://divvybikes.com/data-license-agreement).

## Recomendaciones

**Recomendación 1: Campaña de "conversión de fin de semana" con incentivo a la 
membresía anual.** Los casual riders concentran su actividad los fines de semana 
(sábado y domingo son sus días de mayor volumen y duración). Se recomienda una campaña 
dirigida específicamente a usuarios que rentan en fin de semana, ofreciendo una prueba 
gratuita o descuento en la primera membresía anual, presentada justo al finalizar un 
viaje de fin de semana (vía notificación push o correo).

**Recomendación 2: Membresía flexible o "fin de semana" como puente hacia la anual.** 
Dado que la duración de viaje de casual riders es consistentemente más alta (mediana 
23 min vs 8.5 min de members) y concentrada en tardes/fines de semana, un plan 
intermedio (ej. membresía de fin de semana o de bajo compromiso) podría capturar a 
usuarios que aún no están listos para el compromiso anual completo, sirviendo como 
puente de conversión.

**Recomendación 3: Comunicación dirigida a "casi members".** Identificar y dar 
seguimiento a casual riders con alta frecuencia de uso (aunque sea solo en fin de 
semana) mediante campañas de email/app basadas en su propio historial de ahorro 
potencial (ej. "Ya gastaste $X en pases individuales este mes — con la membresía 
anual habrías ahorrado $Y"), aprovechando que ya conocen y usan el servicio.

**Próximos pasos sugeridos:**
- Ampliar el análisis a los 12 meses completos (no solo Q1) para confirmar si el 
  patrón estacional afecta las conclusiones.
- Investigar estaciones específicas con mayor concentración de casual riders para 
  focalizar geográficamente las campañas.
- Diseñar un test A/B de las ofertas propuestas antes de un rollout completo.
