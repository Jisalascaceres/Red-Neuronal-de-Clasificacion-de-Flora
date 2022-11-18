## Proyecto clasificación Plantas.
#### Hecho por: José Ignacio Salas Cáceres


Temas: Red neuronal, Python, Clasificador, Transfer learning, Plantas, otánica

### Introducción.

En este programa se ha elaborado una red neuronal que pueda clasificar entre 10 plantas de la flora española.  
El dataset usado cuenta con 10 clases de 200 imágenes aprox. cada uno.  
Las imágenes de todo el grupo excepto el girasol proceden del Banco taxonómico Digital de la Flora Ibérica de la web Biodiversidadvirtual.org  (https://www.biodiversidadvirtual.org/herbarium/)    
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
   
 #### Contenido:
 
  El contenido del repositorio estará organizado de la siguiente manera:
  + Las versiones anteriores a la final, con los modelos probados estan en la carpeta: __Versiones__.
  + La versión final, junto con un informe más detallado del proyecto, se encuentra en la carpeta: __Resultado__
