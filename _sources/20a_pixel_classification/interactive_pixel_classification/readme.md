(machine_learning:pixel_classification)=
# Clasificación interactiva de píxeles y segmentación de objetos en Napari

En este ejercicio entrenaremos un [Clasificador Random Forest](https://en.wikipedia.org/wiki/Random_forest) para la clasificación de píxeles y convertiremos el resultado en una segmentación de instancias.
Utilizaremos el plugin de napari [napari-accelerated-pixel-and-object-classification](https://www.napari-hub.org/plugins/napari-accelerated-pixel-and-object-classification).

## Primeros pasos

Abre una ventana de terminal y activa tu entorno conda:

```
conda activate devbio-napari-env
```

Después, inicia Napari:

```
napari
```

Carga el conjunto de datos de ejemplo "Blobs" desde el menú `File > Open Sample > clEsperanto > Blobs (from ImageJ)`

![](apoc1.png)

## Clasificación de píxeles y Segmentación de Objetos en Napari

Para segmentar objetos, podemos usar la herramienta de Segmentación de Objetos en APOC.
Internamente utiliza un clasificador de píxeles y [etiquetado de componentes conectados](https://en.wikipedia.org/wiki/Connected-component_labeling).
El siguiente procedimiento también se muestra en [este video](apoc_object_segmentation.mp4).

Inicia la segmentación de objetos desde el menú `Tools > Segmentation / Labeling > Object Segmentation (APOC)`.

![](apoc2.png)

Agrega una nueva capa de etiquetas haciendo clic en este botón:
![](apoc3.png)

Cambia el tamaño del pincel a un número pequeño como 2 o 3.
![](apoc4.png)

Haz clic en el botón `Paint brush`.
![](apoc5.png)

Comienza a anotar la región de `fondo` donde no hay objetos.
![](apoc6.png)

Aumenta en uno la etiqueta que se está dibujando.
![](apoc7.png)

Dibuja una anotación dentro de los objetos de interés. Dibuja anotaciones de fondo y objeto cerca unas de otras. Cuanto más cerca estén estas dos anotaciones, menor será el grado de libertad que tendrá la computadora al optimizar el modelo más adelante.
![](apoc8.png)

Dentro de la interfaz de usuario `Object segmentation` a la derecha, selecciona la imagen/canal que debe procesarse.
![](apoc9.png)

También selecciona la imagen de etiquetas de anotación que acabas de dibujar.
![](apoc10.png)

Haz clic en `Train`. Debería aparecer una imagen de etiquetas.
![](apoc11.png)

Si la segmentación funciona bien, considera hacer una copia de seguridad del archivo `ObjectSegmenter.cl` que se ha guardado.
Si no cambiaste la ubicación del archivo antes del entrenamiento, estará ubicado en la carpeta desde donde iniciaste napari en la línea de comandos.