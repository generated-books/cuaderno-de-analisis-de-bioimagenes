# Clasificación interactiva de objetos en Napari

En este ejercicio entrenaremos un [Clasificador de Bosque Aleatorio](https://es.wikipedia.org/wiki/Random_forest) para clasificar objetos segmentados.
Usaremos el complemento de napari [napari-accelerated-pixel-and-object-classification](https://www.napari-hub.org/plugins/napari-accelerated-pixel-and-object-classification).

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

Además, necesitamos una imagen de etiquetas. Puedes crearla usando el [clasificador de píxeles entrenado anteriormente](machine_learning:pixel_classification)
o usando el menú `Tools > Segmentation / labeling > Gauss-Otsu Labeling (clesperanto)`.

## Clasificación de objetos

Nuestro punto de partida es una imagen cargada y una imagen de etiquetas con objetos segmentados. El siguiente procedimiento también se muestra en [este video](apoc_object_classification.mp4).

![](apoc21.png)

Añade otra imagen de etiquetas. Renombra la imagen de etiquetas, por ejemplo, a `Label class annotation` para no confundirla con la otra.
![](apoc22.png)

Activa la `Brush tool`.
![](apoc23.png)

Coloca pequeños puntos con la etiqueta `1` en objetos pequeños y redondeados (para fines de entrenamiento: realmente solo los más pequeños).
![](apoc24.png)

Aumenta la `label` a `2`.
![](apoc25.png)

Dibuja una línea a través de los objetos alargados más grandes en el centro de la imagen.
![](apoc26.png)

Inicia la herramienta de clasificación de objetos desde el menú `Tools > Segmentation post-processing > Object classification (APOC)`
![](apoc27.png)

En esta interfaz de usuario, activa la casilla `shape`.
![](apoc28.png)

Selecciona `image`, `labels` y `annotation` de esta manera:
![](apoc29.png)

Haz clic en `Run`. Después de un segundo, debería aparecer una nueva capa de etiquetas con objetos anotados en marrón/azul. Algunos objetos redondos más grandes serán azules involuntariamente.
![](apoc30.png)

Oculta la capa de clasificación recién creada.
![](apoc31.png)

Selecciona tu capa de anotaciones.
![](apoc32.png)

Anota algunos objetos más redondeados, esta vez los más grandes.
![](apoc33.png)

Entrena el clasificador de nuevo.
![](apoc34.png)

Si estás satisfecho con el clasificador entrenado, copia el archivo a un lugar seguro. Al entrenar el siguiente clasificador, este podría sobrescribirse.

## Ejercicio extra
Vuelve a entrenar el clasificador para que pueda diferenciar tres clases diferentes:
* Objetos pequeños y redondos
* Objetos grandes y redondos
* Objetos grandes y alargados