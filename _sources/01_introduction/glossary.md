# Glosario

Este glosario contiene términos utilizados en todo el libro de Jupyter. Las descripciones deben interpretarse en el contexto del análisis de imágenes biológicas.

## Array

Un término común para estructuras de datos que contienen múltiples valores. En Python, dos tipos comunes de arrays son [listas](#list) y [tuplas](#tuple).
Los arrays multidimensionales también se denominan [matrices](#matrix) e [hiperapilamientos](#hyperstack).

## Binarización

La binarización es el acto de segmentar una imagen en dos clases: Verdadero y Falso. Verdadero típicamente se refiere a una región en la imagen donde hay objetos, también llamada el primer plano.
Falso se refiere a la región de fondo donde no hay objetos presentes.

## Imagen binaria

Una imagen binaria es una imagen que contiene solo dos intensidades diferentes. Dependiendo del software utilizado, pueden ser los valores [booleanos](#boolean) Verdadero y Falso, números como 0 y 1, o como en ImageJ 0 y 255.
Una definición común es asociar 0 con Falso y todos los demás valores posibles con Verdadero.

## Booleano

Una variable de tipo booleano solo puede contener dos valores: Verdadero o Falso.

## Clasificación

La clasificación es la tarea de categorizar cosas como células o píxeles en diferentes categorías ("clases").
La clasificación se puede lograr utilizando métodos clásicos simples como la declaración `if` de Python, y utilizando técnicas más complejas de [aprendizaje automático](#machine-learning).

## Agrupamiento

Los algoritmos que agrupan objetos o píxeles según sus propiedades son algoritmos de agrupamiento. Estos algoritmos pueden usarse para [segmentación semántica](#semantic-segmentation) y [clasificación](#classification) de células.

## Etiquetado de componentes conectados

El análisis de componentes conectados o _etiquetado_ es una categoría de algoritmos que típicamente toman imágenes binarias como entrada y producen [imágenes de etiquetas](#label-image).
Estos algoritmos etiquetan por igual los píxeles vecinos que están marcados como objetos. Los píxeles donde no hay conexión se etiquetan de manera diferente.
Ver también [wikipedia](https://en.wikipedia.org/wiki/Connected-component_labeling).

## Convolución

La convolución es el procedimiento que combina una imagen y un [kernel](#kernel) de filtro para producir una nueva imagen. Para cada píxel, su intensidad y las intensidades de sus píxeles vecinos se combinan según lo definido por el kernel del filtro para calcular la intensidad del píxel correspondiente en la imagen de salida.

## Redes neuronales convolucionales

Las redes neuronales convolucionales son una categoría de algoritmos de aprendizaje automático que se utilizan comúnmente en la eliminación de ruido, restauración y segmentación de imágenes.
Estos algoritmos utilizan arquitecturas que simulan la funcionalidad del cerebro para aprender cómo realizar tareas de [regresión](#regression) o [clasificación](#classification).

## DataFrame

Un DataFrame de [pandas](https://pandas.pydata.org/) es una estructura de datos que imita una tabla.
Los DataFrames son comúnmente utilizados por científicos de datos para almacenar datos tabulares como mediciones cuantitativas para realizar análisis estadísticos.

## Aprendizaje profundo

El aprendizaje profundo, a menudo asociado con [redes neuronales convolucionales](#convolutional-neural-networks) profundas, es una categoría de algoritmos de aprendizaje automático con alta complejidad y grandes arquitecturas.
Estos algoritmos se utilizan cada vez más en campos científicos y demuestran superar a los algoritmos clásicos.
Por otro lado, a menudo se necesitan grandes cantidades de datos de entrenamiento y grandes recursos computacionales para entrenar estos modelos.

## Imagen de características

Las imágenes de características se utilizan para algoritmos de [clasificación de píxeles](#classification) como los [clasificadores de bosques aleatorios](#random-forest-classifier).
Esas imágenes se producen aplicando [filtros](#filter) a los datos de la imagen.

## Filtro

En el procesamiento de imágenes, un filtro es una operación que toma una imagen de entrada para producir una imagen de salida. Las imágenes de entrada y salida pueden tener diferente dimensionalidad y tamaño.
Los filtros de procesamiento de imágenes lineales se producen aplicando [convolución](#convolution) a las imágenes.
Los filtros de procesamiento de imágenes no lineales combinan las intensidades de los píxeles en un vecindario local definido de cada píxel de una manera no lineal, por ejemplo, determinando el valor mínimo, máximo o mediano en esta región.

## GPU

Unidad de procesamiento gráfico. Se utiliza para procesar datos de imagen y para entrenar algoritmos de aprendizaje automático, en particular algoritmos de [aprendizaje profundo](#deep-learning).

## Hiperapilamiento

El término hiperapilamiento se usa comúnmente en el procesamiento de imágenes para describir un conjunto de datos de imágenes que tiene más de 3 dimensiones. Las dimensiones adicionales, típicamente no espaciales, pueden ser tiempo, longitud de onda u otra información como la almacenada en [imágenes paramétricas](#parametric-image).

## Segmentación de instancias

Los algoritmos de segmentación que identifican imágenes individuales, por ejemplo, en forma de [imágenes de etiquetas](#label-image) segmentan instancias.

## Imagen de intensidad

Las imágenes de intensidad son típicamente producidas por microscopios, cámaras y dispositivos de tomografía médica. La intensidad en los píxeles de la imagen describe una medición física, por ejemplo, del número de fotones que golpearon el detector durante la adquisición.

## Kernel

Un kernel de filtro describe cómo las intensidades de píxeles locales alrededor de un píxel dado deben combinarse usando una suma ponderada para [convolucionar](#convolution) una imagen de entrada.

## Imagen de etiquetas

Una imagen de etiquetas es una imagen donde la intensidad del píxel expresa a qué objeto pertenece el píxel.
Por ejemplo, si un píxel tiene intensidad 1, pertenece al objeto 1. Si un píxel tiene intensidad 3, pertenece al objeto 3.
La intensidad máxima en una imagen [etiquetada secuencialmente](#sequential-labeling) corresponde al número de objetos en la imagen.

## Etiquetado

Los algoritmos de etiquetado típicamente toman imágenes como entrada y producen [imágenes de etiquetas](#label-image). De esa manera, los píxeles se asocian con identidades de objetos.

## Lista

Las listas son estructuras de datos, por ejemplo en programación Python, que pueden ser cambiadas. Es posible agregar, eliminar y cambiar elementos en la lista.

## Aprendizaje automático

El aprendizaje automático es una categoría de algoritmos que se basan en métodos estadísticos para derivar modelos a partir de datos.
Por ejemplo, un algoritmo que toma anotaciones de imágenes generadas manualmente por humanos y logra _aprender_ de las anotaciones cómo anotar otras imágenes es una máquina de aprendizaje.

## Matriz

Array multidimensional de valores. Las matrices bidimensionales pueden interpretarse como imágenes. Las matrices tridimensionales se llaman comúnmente pilas de imágenes. Las matrices de dimensionalidad superior también se denominan hiperapilamientos.

## Imagen paramétrica

Las imágenes paramétricas, o mapas paramétricos, son imágenes donde una intensidad de píxel dada expresa una medición de un objeto dado.
Por ejemplo, un píxel con valor 2 en una `imagen-de-relación-de-aspecto` pertenece a un objeto que es dos veces más largo que ancho. Ver también [mapas paramétricos](data_visualization.parametric_maps).

## Clasificación de píxeles

La clasificación de píxeles es el proceso de categorizar píxeles en múltiples clases. Típicamente, la clasificación de píxeles conduce a una imagen que expresa una [segmentación semántica](#semantic-segmentation) o a [mapas de probabilidad](#probability-maps).

## Mapas de probabilidad

Un mapa de probabilidad es una imagen donde la intensidad del píxel expresa la probabilidad de que el píxel pertenezca a una clase o categoría específica. Estas imágenes son resultados intermedios comunes de los algoritmos de [clasificación de píxeles](#pixel-classification).

## Clasificador de bosque aleatorio

Algoritmo de aprendizaje automático supervisado, comúnmente utilizado para [clasificación de píxeles](pixel_classification.apoc) y [clasificación de objetos](pixel_classification.apoc) en datos de imágenes de microscopía.

## Regionalización

Subdividir una imagen en múltiples regiones. Ver también [Etiquetado](#labeling).

## Regresión

La regresión en el contexto del aprendizaje automático es una categoría de algoritmos que intentan reducir un sistema observado, por ejemplo, un video de células en movimiento, a valores numéricos, por ejemplo, la velocidad promedio de las células en movimiento.
Ver también [análisis de regresión (Wikipedia)](https://en.wikipedia.org/wiki/Regression_analysis).

## Segmentación semántica

Asociar píxeles con una categoría como "citoplasma" o "núcleo" pero sin especificar qué célula o núcleo.

## Etiquetado secuencial

El etiquetado secuencial es un paso de procesamiento que toma cualquier [imagen de etiquetas](#label-image) y produce otra imagen de etiquetas que cumple una condición: Existe cada intensidad de píxel entero entre 0 y la intensidad máxima.
Por lo tanto, si la imagen contiene el valor 4, se garantiza que también existen los valores de píxel 1, 2 y 3.
Hay algoritmos que solo funcionan con imágenes de entrada etiquetadas secuencialmente.

## Cadena

Las variables de cadena en lenguajes de programación comunes son variables que contienen texto. Técnicamente, la variable es un [array](#array) de caracteres.

## Tupla

Estructura de datos en Python que contiene múltiples valores que no pueden ser cambiados (inmutable).