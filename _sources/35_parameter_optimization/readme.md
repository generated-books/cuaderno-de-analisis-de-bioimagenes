# Optimización de parámetros

En este capítulo aplicaremos algunas estrategias para optimizar los parámetros de los flujos de trabajo de procesamiento de imágenes.
En general, es importante contar con datos de referencia de alta calidad, como imágenes segmentadas manualmente.
Además, es necesaria una función de aptitud (también llamada a veces función de pérdida) bien diseñada.
Para la optimización de parámetros utilizaremos el [paquete optimize de scipy](https://docs.scipy.org/doc/scipy/reference/optimize.html) y el plugin de Napari [napari-workflow-optimizer](https://github.com/haesleinhuepf/napari-workflow-optimizer).