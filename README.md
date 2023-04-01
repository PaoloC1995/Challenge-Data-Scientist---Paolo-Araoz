1. How is the data distributed? Did you find any noteworthy insight to share? What can you conclude about this?

      La base de datos presentada en el informe esta distribuida de una forma ordenada en la cual podemos sacar informacion necesaria para           poder realizar las siguientes afirmaciones:
      - De los 68206 vuelos realizado desde el aeropuerto de Santiago de Chile en el año 2021 tuvieron 62 destinos programados
      - De los 68206 vuelos realizado desde el aeropuerto de Santiago de Chile en el año 2021 fueron atendidos por 23 aerolineas
      - De los 68206 vuelos realizado desde el aeropuerto de Santiago de Chile a grandes rasgos podemos notar que entre la Fecha y hora             prevista del vuelo y la Fecha y hora de operacion del vuelo hay cierto margen de diferencia en algunos vuelos programados, el cual nos         permitirá calcular la tasa de delay en los vuelos

2. Generate the following additional columns. Please export them to a CSV file named synthetic_features.csv:

Revisar el repositorio

3. What is the behavior of the delay rate across destination, airline, month of the year, day of the week, season, type of flight?What
variables would you expect to have the most influence in predicting delays?
      En base a los datos proporcionados podemos indicar que de los 68206 vuelos realizado desde el aeropuerto de Santiago de Chile en el año 2021, el 18.49% tuvieron delay en la operacion de sus vuelos (12614). De los 12614 vuelos con delay podemos concluir detalles importantes para las variables indicadas:
      - Segun el destino tenemos que Buenos Aires y Lima son los que encabezan el numero de destinos de vuelos con delay (12.84% y 9.62% respectivamente)
      - Segun la aerolinea tenemos que el grupo Latam y Sky Airline son los que encabezan la lista con un 57.92% y 20,14% respectivamente
      - Segun el mes del año tenemos que en el mes de Julio y Diciembre son los periodos que tienen mayor cantidad de vuelos con delay con un 13.94% y 12.80% respectivamente
      - Segun el dia de la semana tenemos que viernes, lunes y jueves son los que encabezan la lista y tienen un porcentaje similar con un 18.11%, 16.24% y 16.21% 
      - Segun la temporada tenemos que en la temporada normal hay mayor cantidad de vuelos con delay con un 63.98% mientras que la alta con un 36.02%
      - Segun el tipo de vuelo tenemos que los vuelos internaciones tienen mayor cantidad de vuelos con delay con un 55.87%
       Con esto podemos concluir que las variables que tienen mayor influencia a mi parecer las 6 variables son adecuadas para poder utilizarlas para identificar la probabilidad de delay en los vuelos
      
4. Train one or several models (using the algorithm(s) of your choice) to estimate the likelihood of a flight delay.
Feel free to generate additional variables and/or supplement with external variables.

Revisar el repositorio

5. Evaluate model performance in the predictive task across each model that you trained. Define and justify what metrics you used
to assess model performance. Pick the best trained model and evaluate the following: What variables were the most influential in
the prediction task? How could you improve the
Performance?

Utilice 4 modelos de los cuales todas tienen un porcentaje de error similar bajo que pueden ser utilizadas para las predicciones de si en vuelos futuros puede tener delay o no. Indicar que para mi, el modelo de regresion multiple permite manejar las variables con mayor comodidas si queremos agregar o quitar variables. Las variables que mas influyen son las del destino y la aerolinea, teniendo mas cantidad de segmentacion de datos podemos tener un mejor pronostico
