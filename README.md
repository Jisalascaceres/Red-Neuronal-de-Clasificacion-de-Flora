## Red Neuronal de Clasificación de Flora.
#### Hecho por: José Ignacio Salas Cáceres


### Introducción.

En este programa se ha elaborado una red neuronal que pueda clasificar entre 10 plantas de la flora española.  
El dataset usado cuenta con 10 clases de 200 imágenes aprox. , cada uno.  
Las imágenes de todo el grupo excepto el girasol proceden del Banco taxonómico Digital de la Flora Ibérica de la web Biodiversidadvirtual.org.  (https://www.biodiversidadvirtual.org/herbarium/)    
Las imágenes del girasol proceden del dataset "Flower Recognition" de kaggle. (https://www.kaggle.com/datasets/alxmamaev/flowers-recognition)

El listado de plantas usado, con nombre científico y común, es el siguiente:  

 + n1 = Papaver rhoeas, Amapola
 + n2 = Aphyllanthes monspeliensis, chunqueta
 + n3 = Helianthus annuus, Girasol
 + n4 = Astragalus incanus, Piorno
 + n5 = Campanula rapunculus, Campanilla
 + n6 = Gynandriris sisyrinchium, lirio
 + n7 = Lonicera etrusca, madreselva
 + n8 = Oxalis pes crapae, Trebolina
 + n9 = Paronychia capitata, Hierba plateada
 + n10 = Vincetoxicum hirundinaria, Matatósico
 
 
 Para realizar esta clasificación se ha comenzado con una red convolutiva estándar al que se le han ido cambiando los hiperparámetros para aumentar el rendimiento.
 También, se ha aplicado Transfer Learning, en concreto importando el modelo VGG16 y cambiando algunas capas, añadiendo otras o haciendolas entrenables.  
 Este último modelo, con 2 capas entrenables, es el que ha dado mayor precision a la hora de clasificar el conjunto de validación, llegando a más del __90%__ .
   
 #### Contenido:
 
 En el repositorio nos encontramos con varias versiones de este mismo proyecto, y es que para obtener un modelo con buenos resultados se han probado otros tantos. A modo de resumen, se han subido 4 versiones del trabajo:  
 
 + Una versión con una serie de hiperparametros usando solamente redes convolutivas.
 + Una versión parecida a la anterior con otros hiperparametros.
 + Una versión aplicando Transfer Learning con el modelo VGG16, sin entrenar ninguna de las capas de este.
 + Una versión aplicando Transfer Learning con el modelo VGG16, aplicando también Fine Tunning, es decir, entrenando del modelo VGG16 algunas capas.
   
 Aunque estos son los entregados, se han probado por el camino varios modelos más, diferentes iteraciones de estos 4. Estas versiones se encuentran en la carpeta __Versiones__, excepto la final y que obtuvo mejores resultados que se encuentra junto con el Readme.
 
 #### Recursos utilizados:
 
 Para la realización de este trabajo se han utilizado los siguientes recursos:  
 + Librería Keras para la construcción de los modelos de redes neuronales y el Transfer Learning.
 + Librería Matplotlib y Seaborn para la representación gráfica de resultados.
 + Google Colab como IDE.
 
