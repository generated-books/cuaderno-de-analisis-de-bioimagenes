# Procesamiento de imágenes acelerado por GPU

Como trabajamos a menudo con datos de imágenes tridimensionales, potencialmente a lo largo del tiempo, el procesamiento de imágenes clásico lleva bastante tiempo.

Por lo tanto, también nos sumergiremos en el procesamiento de imágenes en unidades de procesamiento gráfico (GPU) utilizando [OpenCL](https://www.khronos.org/opencl/), [pyopencl](https://documen.tician.de/pyopencl/) y [pyclesperanto](https://github.com/clesperanto/pyclesperanto_prototype). Esta tecnología nos permite procesar imágenes más rápido, acelerado por GPU. Los algoritmos clásicos y el procesamiento de imágenes acelerado por GPU pueden diferir en los detalles muy específicos, pero nosotros como usuarios no deberíamos notarlo. Una operación específica de procesamiento de imágenes debería entregar resultados similares independientemente de cómo se calcule.

## Instalación de requisitos
Los usuarios de Windows y Mac no deberían necesitar instalar OpenCL. Todo lo que necesitas debería estar preinstalado. Los usuarios de Linux necesitan instalar un OpenCL-ICD-Loader.

Por lo tanto, los usuarios de Linux pueden tener que ejecutar comandos como este, dependiendo de la distribución de Linux:

```
sudo apt update
sudo apt install ocl-icd-opencl-dev
```

Después, la instalación puede proceder usando conda _y_ pip:
```
mamba install -c conda-forge l pyclesperanto-prototype
```

Posteriormente, puedes probarlo, por ejemplo, ejecutando estos comandos en un script de Python o un notebook de Jupyter:
```
import pyclesperanto_prototype as cle

print("Used GPU:", cle.get_device())
```

También siéntete libre de instalar el [plugin napari-pyclesperanto-assistant en napari](https://clesperanto.github.io/napari_pyclesperanto_assistant/).

## Instalación de requisitos opcionales

En este capítulo, también echaremos un vistazo a [cupy](https://cupy.dev), una biblioteca de procesamiento acelerado por GPU basada en [NVidia CUDA](https://en.wikipedia.org/wiki/CUDA) y [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing), un plugin de napari programable. Estos dos se pueden instalar utilizando los siguientes comandos. Sin embargo, esto solo funcionará en computadoras que tengan una tarjeta gráfica NVidia compatible con CUDA.

```
mamba install -c conda-forge cupy cudatoolkit=10.2
mamba install -c conda-forge napari
pip install napari-cupy-image-processing
```

Nota: Dependiendo de tu instalación de CUDA, es posible que quieras reemplazar el "10.2" en la línea de comando anterior con la versión de CUDA que hayas instalado en tu computadora.

Ver también
* [Rendimiento de GPUs dedicadas para portátiles versus GPUs de escritorio (video de Linus Tech Tips)](https://www.youtube.com/watch?v=z9fk9d6pry4)
* [Instalación de Cupy](https://docs.cupy.dev/en/stable/install.html#installing-cupy)