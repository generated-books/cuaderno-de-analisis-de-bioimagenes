# Procesamiento de superficies

En este capítulo procesaremos datos de superficie. Las superficies, también conocidas como mallas, consisten en puntos en el espacio 3D, llamados vértices, que están conectados entre sí formando triángulos, también conocidos como caras. Muchos triángulos juntos forman una superficie. Si la superficie está cerrada de modo que ningún rayo pueda pasar del interior al exterior sin cruzar un triángulo, la superficie se denomina hermética.

## Instalación de requisitos

Utilizaremos la biblioteca [vedo](https://vedo.embl.es/) para procesar y visualizar superficies y el complemento programable de napari [napari-process-points-and-surfaces](https://github.com/haesleinhuepf/napari-process-points-and-surfaces). Ambos pueden instalarse así:

```
mamba install vedo
pip install napari-process-points-and-surfaces
```