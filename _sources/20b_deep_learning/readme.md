# Segmentación de imágenes basada en aprendizaje profundo

En este capítulo, utilizaremos algoritmos basados en aprendizaje profundo para la segmentación de imágenes.

## Instalación de requisitos

Para utilizar [cellpose](https://cellpose.readthedocs.io/) y [stardist](https://github.com/stardist/stardist), se deben instalar estas dependencias:

```
mamba install cellpose pytorch=1.8.2 cudatoolkit=10.2 -c pytorch-lts
pip install tensorflow
pip install stardist
```

Los cuadernos en esta carpeta han sido probados utilizando:
* `torch==2.0.1`
* `stardist==0.8.3`
* `tensorflow==2.12.0`
* `csbdeep==0.7.3`
* `cellpose==2.2.1`