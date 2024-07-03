# Agrupamiento
En este capítulo agruparemos puntos de datos según sus propiedades. No proporcionaremos anotaciones de las que la computadora pueda aprender y, por lo tanto, los métodos que usamos aquí pertenecen a la categoría de [_aprendizaje automático no supervisado_](https://en.wikipedia.org/wiki/Unsupervised_learning).

## Ciencia de datos exploratoria de imágenes y generación de hipótesis
En este capítulo, utilizamos métodos de exploración de datos de imágenes. Ninguno de ellos permite sacar conclusiones directamente. Por ejemplo, puede concluir de uno de los siguientes cuadernos que una combinación de intensidad media, la varianza de intensidad y descriptores de forma de núcleos segmentados permite agrupar los núcleos en grupos como _mitóticos_ y _no mitóticos_. El propósito del cuaderno era permitirle generar esta hipótesis. Sin embargo, esta hipótesis necesita ser confirmada en un conjunto de datos representativo.
Los métodos presentados, como la reducción de dimensionalidad, el escalado y el agrupamiento, le permiten obtener información sobre las relaciones entre los parámetros medidos en las imágenes. Con fines académicos, hacemos esto en imágenes individuales. Tenga en cuenta que ninguno de los procedimientos mostrados es generalizable. Es posible que aplicar los mismos cuadernos a diferentes imágenes de ejemplo conduzca a resultados diferentes. Siempre que planee aplicar estas técnicas a datos de imágenes, se recomienda:
* Usar mediciones de múltiples imágenes
* Asegurarse de haber seleccionado un conjunto representativo de muestras de la población de datos que desea comprender mejor.
* Utilizar los conocimientos obtenidos de las técnicas de análisis de datos exploratorios presentes para configurar experimentos de seguimiento que prueben las relaciones presumidas.

## Instalación
Utilizaremos las bibliotecas [scikit-learn](https://scikit-learn.org/), [umap_learn](https://umap-learn.readthedocs.io/) y [hdbscan](https://hdbscan.readthedocs.io/). Para la visualización de datos utilizaremos [seaborn](https://seaborn.pydata.org/).
Todos se pueden instalar usando mamba/conda.

```
mamba install scikit-learn umap-learn hdbscan seaborn
```