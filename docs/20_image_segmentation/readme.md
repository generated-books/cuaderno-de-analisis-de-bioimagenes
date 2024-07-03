# Segmentación de imágenes

Los analistas de imágenes se refieren a la segmentación de imágenes cuando subdividen una imagen en múltiples grupos de píxeles con diferentes características. En este capítulo aprenderemos algoritmos básicos para binarizar imágenes y para etiquetar objetos en imágenes.

## Instalación de requisitos

Como en los capítulos anteriores, utilizaremos [scikit-image](https://scikit-image.org/), [pyclesperanto-prototype](https://github.com/clEsperanto/pyclesperanto_prototype) y [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing) para segmentar las imágenes. Algunas visualizaciones se realizarán nuevamente utilizando [matplotlib](https://matplotlib.org/).

## Instalación de dependencias opcionales

Para algunos atajos a algoritmos de segmentación de imágenes basados en watershed, se recomienda la instalación del plugin scriptable de napari [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes). Puedes instalarlo usando pip:

```
pip install napari-segment-blobs-and-things-with-membranes
```

Ver también
* [Cuadernos de SimpleITK](https://github.com/InsightSoftwareConsortium/SimpleITK-Notebooks)