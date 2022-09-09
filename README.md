# Evidencia_Machine-Learning

Reto: Uso de framework o biblioteca de aprendizaje máquina para la implementación de una solución.

*Instrucciones:*
1. Crea un repositorio de GitHub para este proyecto.
2. Programa uno de los algoritmos vistos en el módulo (o que tu profesor de módulo autorice) haciendo uso de una biblioteca o framework de aprendizaje máquina. Lo que se busca es que demuestres tu conocimiento sobre el framework y como configurar el algoritmo. 
3. Prueba tu implementación con un set de datos y realiza algunas predicciones. Las predicciones las puedes correr en consola o las puedes implementar con una interfaz gráfica apoyándote en los visto en otros módulos.
4. Tu implementación debe de poder correr por separado solamente con un compilador, no debe de depender de un IDE o de un “notebook”. Por ejemplo, si programas en Python, tu implementación final se espera que esté en un archivo .py no en un Jupyter Notebook.
5. Después de la entrega intermedia se te darán correcciones que puedes incluir en tu entrega final.

El dataset contiene variables relevantes a los valores de vivienda en los suburbios de Boston. El archivo .csv fue obtenido de Kaggle: https://www.kaggle.com/datasets/arslanali4343/real-estate-dataset

Para el análisis de nuestros datos utilizamos la librería de skikit-learn train-test-split, 75% de los datos se utilizan para entrenar y 25% para probar el modelo. 

Para la solución de este reto se utilizó la librería de skikit-learn. un software para aprendizaje máquina (ML). Específicamente utilizaremos el modelo de machine learning de .... 

Primero filtramos los datos el cual involucró quitar los datos NaN. Las demás columnas eran valores numéricos así que no hubo necesidad de agregar, cambiar o quitar columnas de datos. 
Posterior a esto, empleamos en una matriz de correlación del método pearson a todas las variables. Con esto podemos ver qué tan fuerte es la correlación entre variables y agregar otra capa de filtro al implementar nuestro modelo de regresión lineal múltiple. Todos los variables que presentaban un |r|>0.45 no se consideran como un variable independiente para nuestro modelo. 

# Desempeño utilizado

