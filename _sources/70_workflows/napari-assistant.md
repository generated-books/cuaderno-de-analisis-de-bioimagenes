# El Asistente de Napari

El Asistente de Napari es un complemento para napari que te permite configurar un flujo de trabajo de procesamiento de imágenes.

Este tutorial también está disponible en video [napari-assistant.mp4](images/napari-assistant.mp4).

Inicia napari desde la línea de comandos de esta manera:

```bash
conda activate my_first_env

napari
```

![](images/napari-assistant01.jpg)

Se abrirá la ventana de napari. Haz clic en el menú `Archivo > Abrir Muestras Células(3D+2Ch)` para abrir una imagen de ejemplo.

![](images/napari-assistant02.jpg)

![](images/napari-assistant03.jpg)

Puedes explorar este conjunto de datos haciendo clic en el botón de vista `2D/3D`.

![](images/napari-assistant04.jpg)

Inicia el Asistente de Napari desde el menú `Herramientas > Utilidades > Asistente (na)`.

![](images/napari-assistant05.jpg)

Dentro del panel `Asistente`, haz clic en el botón `Eliminar ruido`.

![](images/napari-assistant06.jpg)

Haz clic en los botones `Ojo` en la lista de capas para ocultar la imagen original y mostrar solo el resultado del paso `Eliminar ruido`.

![](images/napari-assistant07.jpg)

Haz clic en el botón `Binarizar` en el panel del Asistente para agregar un nuevo paso al flujo de trabajo que genera una imagen binaria a partir de la capa actual.

![](images/napari-assistant08.jpg)

Alterna entre las vistas 2D/3D y la visibilidad de las capas para explorar el resultado del paso `Binarizar`.

![](images/napari-assistant09.jpg)

Después de volver a la vista 2D, haz clic en el botón `Etiquetar` en el Asistente y elige la operación `Etiquetado de componentes conectados (clEsperanto)`.

![](images/napari-assistant11.jpg)

Selecciona la capa `Resultado de gaussian_blur` en la lista de capas y modifica sus parámetros `sigma`. Notarás que los pasos subsiguientes (Umbral de Otsu y Etiquetado de Componentes Conectados) también se actualizan.

![](images/napari-assistant12.jpg)

Cambia a la vista de cuadrícula, muestra todas las capas usando sus botones `Ojo` y continúa modificando los parámetros.

![](images/napari-assistant13.jpg)

![](images/napari-assistant14.jpg)

Cierra todas las capas excepto `núcleos` y `membrana`.

![](images/napari-assistant15.jpg)

Desactiva la vista de cuadrícula y haz clic nuevamente en el botón `Etiquetar` en el Asistente.

![](images/napari-assistant16.jpg)

Esta vez, no cambies la operación sino el parámetro `spot_sigma` en su lugar.

![](images/napari-assistant17.jpg)

Cambia nuevamente a la vista 3D e inspecciona el resultado de este único paso.

![](images/napari-assistant18.jpg)