# Deconvolución de imágenes
La deconvolución de imágenes es también _simplemente_ una forma especial de filtrado de imágenes. Dedicamos un capítulo entero a esto porque las deconvoluciones juegan un papel importante en la microscopía de fluorescencia.

Demostraremos los principios en imágenes bidimensionales. Sin embargo, cabe destacar que la deconvolución debería realizarse en tres dimensiones si es posible, ya que los principios físicos subyacentes no son los mismos en todas las direcciones; la función de dispersión puntual típicamente no es simétrica en la microscopía de fluorescencia.

## Instalación de requisitos

Usaremos [RedLionFish](https://github.com/rosalindfranklininstitute/RedLionfish) y [SimpleITK](https://simpleitk.readthedocs.io/) para deconvolucionar imágenes. Para facilitar su uso, trabajaremos con este último a través de una capa de conveniencia, [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing). Ingresa estos comandos en la terminal para instalar todo:

```
mamba install reikna pyopencl -c conda-forge
pip install redlionfish
pip install napari-simpleitk-image-processing
```

<!--
## Instalación de dependencias opcionales

En un cuaderno también usaremos NVidia CUDA para deconvolución. Si tu unidad de procesamiento gráfico soporta cuda, siéntete libre de instalar [pycudadecon](https://github.com/tlambert03/pycudadecon).

```
mamba install -c conda-forge pycudadecon
```
-->

## Ver también
* [BioDIP Dresden, Cómo deconvolucionar imágenes usando Huygens](https://www.biodip.de/wiki/How_to_deconvolve_images_using_Huygens)