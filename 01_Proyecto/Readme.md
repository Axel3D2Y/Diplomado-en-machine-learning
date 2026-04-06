
# Ejercicio número 1 del diplomado

Se dispone de un conjunto de datos que contiene información demográ ca y de salud de pacientes asegurados (insurance.csv). El
objetivo es contruir un modelo de regresión para predecir el gasto médico anual (charges) utilizando las siguientes covariables:
    * age: edad del asegurado
    * sex: sexo
    * bmi: índice de masa corporal
    * children: número de hijos
    * smoker: si fuma o no
    * region: región de residencia
## 1. Calcule estadísticas descriptivas de las variables numéricas:
    a) Grafique la distribución de charges.

    b) Analice la relación entre charges y las variables: age, bmi, smoker,
    
    Análisis esperado: identi car qué variables parecen tener mayor relación con los gastos médicos, detectar posibles valores
    atípicos y observar si la distribución de charges es asimétrica
## 2. Antes de aplicar el algoritmo KNN es necesario preparar los datos.

    a) Explique por qué es necesario codi car las variables categóricas (sex, smoker, region).

    b) Aplique una técnica One-Hot Encoding a las variables categóricas.

    c) Estandarice las variables predictoras.

    d) Divida el conjunto de datos en entrenamiento (80%) y prueba (20%).

    e) por qué el escalamiento es especialmente importante en KNN.
## 3. Entrene el algoritmo KNN(k) con distintos valores del número de vecinos: k = 1,3,5,7,9,11,15.
    a) Utilice validación cruzada de 10 folds para evaluar el desempeño del modelo.
    
    b) Calcule las siguientes métricas:
        1) MAE (Mean Absolute Error)
        2) RMSE (Root Mean Squared Error)
    
    c) Gra que el error en función de k.
    
    d) ¾cómo cambia el error al aumentar el número de vecinos? qué valor de k parece óptimo?
## 4. Explique el comportamiento observado en la grá ca anterior en términos del trade-o sesgo-varianza.
    a) qué ocurre cuando k = 1

    b) qué ocurre cuando k es muy grande

    c) cómo inuye esto en la capacidad predictiva del modelo.
## 5. Seleccione el valor óptimo de k y entrene el modelo nal utilizando el conjunto de entrenamiento. Evalúe el modelo en el onjunto de prueba calculando:
    a) MAE

    b) RMSE

    c) R2

    d) Interprete los resultados: ¾qué tan grande es el error promedio de predicción?. ¾el modelo parece adecuado para
    predecir gastos médicos? ¾qué variables podrían explicar los errores más grandes?
## 6. Implemente validación cruzada anidada para seleccionar el valor óptimo de k. Compare:
    a) el error estimado con validación cruzada simple

    b) el error estimado con validación cruzada anidada
    
    c) por qué la validación anidada proporciona una estimación más con able del error de generalización.