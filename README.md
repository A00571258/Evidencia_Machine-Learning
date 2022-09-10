# Evidencia_Machine-Learning

En esta entrega se realiza la implementación de una máquina de aprendizaje: Regresión Lineal con gradiente descendiente. Es importante recalcar que no se utlizó alguna librería al ejecutarlo. 
El data frame se encuentra en: (https://www.kaggle.com/datasets/rsadiq/salary). Utilizando la relación entre el variable independiente, años de experiencia y Y, nuestra variable dependiente como el salario con un tamaño de muestra de 35 accionistas.

Para analizar los datos aseguramos que no hubiera valores repetidos. Posterior a esto visualizamos los datos utilizando un scatterplot con la librería de Seaborn con los X y Y previamente establecidas. Con esto pudimos confirmar que nuestro dataframe efectivamente presentaba un comportamiento lineal sin considerable dispersión. 
<img width="418" alt="Screenshot 2022-09-10 at 2 22 55" src="https://user-images.githubusercontent.com/83677775/189473678-08a0b492-ee9e-436e-b259-84a448acb6a2.png">

Para realizar el análisis de nuestros datos fue necesario dividirlos en entrenamiento (75%) y prueba (25%). De igual manera, visualizamos los subsets de cada relación para asegurarnos que se asimilaba a un comportamiento lineal.
Los parámetros para gradiente descendiente fueron lo siguiente:
- alpha = 0.01
- theta = [1.5,0.5]

Nuestro modelo de regresión lineal se comporta de la siguiente manera: 
<img width="478" alt="Screenshot 2022-09-10 at 2 23 20" src="https://user-images.githubusercontent.com/83677775/189473690-39117337-006e-4195-9ce7-2ad4f999d437.png">

Al emplear nuestro modelo observamos que presenta los siguientes valores:
- Coeficiente determinación: 0.9875928586744418
- Error cuadrático medio: 58779957.00593381
Tenemos un muy buen coeficiente de determinación, es decir, nuestro modelo de regresión lineal. 

# Análisis del Dataframe: Salary
En está sección presentaremos el análisis para sesgo, varianza y ajuste de modelo. 

## Sesgo
Para el sesgo comparamos la distribución de datos de entrenamiento del salario con la distribución de datos del modelo. 
<img width="999" alt="Screenshot 2022-09-10 at 2 23 31" src="https://user-images.githubusercontent.com/83677775/189473694-5dbaaebd-741e-41b8-a07b-5ff26828c5fd.png">
Observamos un comportamiento similar en las dos gráficas. Ambas presentan dos picos donde el de la izquierda es más pronunciada. Sin embargo, los picos de la predicción de ventas están desplazados hacia la derecha. Es decir, presenta un sesgo negativa. 

## Varianza
Calculamos la varianza para nuestro variable dependiente del subset de prueba y los valores de nuestro modelo. 
- La varianza de y prueba es 751550960.4137931
- La varianza de y modelo es 1188704860.3995128

Como podemos observar, nuestro modelo presenta una mayor variación que los datos de Y de prueba. 

## Nivel de ajuste del modelo (underfitting, fit, overfitting)
Para observar el nivel de ajuste de nuestro modelo consideramos el error cuadrático medio y coeficiente de determinación con los datos de entrenamiento. Si el modelo presenta overfitting estos valores deben dar valores cerca de 0. A nosotros nos dió lo siguiente: 
- El error cuadratico medio es: 173156661.95266923
- El coeficiente de determinación es: 0.9551567153288066

Son valores considerablemente altos por lo que declaramos que el nivel de ajust del modelo es: underfitting. 
