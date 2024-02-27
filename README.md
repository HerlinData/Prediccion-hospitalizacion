# Prediccion-hospitalizacion
## **Planteamiento de la problemática**

Hemos sido contratados en el equipo de ciencia de datos en una consultora de renombre. Nos han asignado a un proyecto de estudio de atención en salud para un importante hospital. **Nuestro cliente desea saber las características más importantes que tienen los pacientes de cierto tipo de enfermedad que terminan en hospitalización.** Fue definido como caso aquel paciente que fue sometido a biopsia prostática y que en un periodo máximo de 30 días posteriores al procedimiento presentó fiebre, infección urinaria o sepsis; requiriendo manejo médico ambulatorio u hospitalizado para la resolución de la complicación y como control al paciente que fue sometido a biopsia prostática y que no presentó complicaciones infecciosas en el período de 30 días posteriores al procedimiento. Dado que tienen en su base de datos algunos datos referentes a los pacientes y resultados de exámenes diagnósticos, de pacientes hospitalizados y no hospitalizados, nos han entregado esta información.  

El departamente de datos advierte que hay algunos problemas de calidad de datos en la información suministrada por lo que el primer reto del equipo es realizar un análisis exploratorio de los datos con el fin de transformar y preparar las datos adecuadamente. 

### Archivos:

- BBDD_Hospitalización.xlxs: Estos datos provienen del dataset original.
- BBDD_Hospitalización2encod.csv: Estos datos luedo del ETL y EDA.: Desarrollo de la limpieza de los datos y exploración.
- ETL_EDA_2.ipynb: Desarrollo del proceso ETL y EDA.
- Modelamiento.ipynb: Desarrollo de los modelos de Machine Learning.

## Conclusiones

*Se realizaron entrenamientos de tres modelos (Árbol de Decisión, K-Vecinos Cercanos y Máquina de Soporte de Vectores) mediante dos enfoques de análisis. Uno consideró todas las variables del conjunto de datos, mientras que el otro exploró cuatro escenarios de reducción de dimensionalidad.*

*En ambos enfoques, se concluyó que el Árbol de Decisión fue el algoritmo más efectivo para clasificar a los pacientes, ya sea hospitalizados o no. No obstante, en el primer enfoque, que utilizó todas las variables del conjunto de datos, el modelo solo alcanzó un F1 Score de 0.77, considerado relativamente bajo. En contraste, en el enfoque de reducción de dimensionalidad, el modelo más destacado fue un Árbol de Decisión con una profundidad máxima de 30, empleando el criterio Gini y con 10 componentes de reducción. En este último escenario, se logró un F1 Score de 0.91, representando un rendimiento aceptable, especialmente dado el considerable desbalance en la clase objetivo.*