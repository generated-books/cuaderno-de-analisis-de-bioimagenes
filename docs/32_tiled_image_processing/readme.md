# Procesamiento de imágenes en mosaico

Si los datos de la imagen son demasiado grandes para caber en la memoria, se hace necesario dividir la imagen en múltiples _mosaicos_ y procesarlos individualmente. Aunque este paso es sencillo, puede resultar muy desafiante unir los mosaicos de imagen resultantes y devolver una gran imagen de resultado. En esta sección elaboraremos múltiples estrategias para lidiar con el procesamiento de imágenes en mosaico. La [biblioteca dask](https://docs.dask.org/en/stable/) facilita el procesamiento de imágenes en mosaico. Este capítulo comienza con un flujo de trabajo completo que muestra dask en acción y luego explica los pasos individuales para configurar un flujo de trabajo adecuado para procesar tus datos posteriormente.

Ver también
* Charla de Genevieve Buckley sobre ["dask-image: procesamiento de imágenes distribuido para grandes datos"](https://www.youtube.com/watch?v=MpjgzNeISeI&t=1359s) (PyConline AU 2020) [Diapositivas](https://genevievebuckley.github.io/dask-image-talk-2020/)
* Charla de John Kirkham sobre ["dask image: Una biblioteca para el procesamiento distribuido de imágenes"](https://www.youtube.com/watch?v=XGUS174vvLs) (SciPy 2019)
* [Documentación de Dask](https://docs.dask.org/en/stable/)
* [Documentación de Dask image](http://image.dask.org/en/latest/)
* [Ejemplos de Dask: procesamiento de imágenes](https://examples.dask.org/applications/image-processing.html)
* https://github.com/VolkerH/DaskFusion