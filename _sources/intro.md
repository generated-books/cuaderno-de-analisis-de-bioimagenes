# Cuadernos de Análisis de Bioimágenes

Esta colección de cuadernos [jupyter](https://jupyter.org/) de [Python](https://www.python.org/) está escrita para principiantes en Python interesados en 
analizar imágenes tridimensionales de células, tejidos, organoides y organismos adquiridas con microscopios de fluorescencia modernos. 
Los principios básicos se demuestran con datos de imágenes bidimensionales y ejemplos más sofisticados se aplican a datos de imágenes tridimensionales y conjuntos de datos de lapso de tiempo.
Este libro está escrito para biólogos, bioquímicos y biofísicos. 
Introducimos el lenguaje técnico que utilizan los científicos de la computación y los científicos de datos al describir la segmentación de imágenes, la computación científica y la ciencia de datos de imágenes.
Si ves margen de mejora, por favor [crea un problema en github](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/issues) y/o considera [contribuir](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/blob/main/CONTRIBUTING.md).

## Prólogo de la Edición en Español
Este libro es una edición traducida automáticamente del original en inglés [BioImageAnalysisNotebooks](https://haesleinhuepf.github.io/BioImageAnalysisNotebooks). Dado que la traducción fue generada por una inteligencia artificial ([Ver código fuente](https://github.com/generated-books/cuaderno-de-analisis-de-bioimagenes/blob/main/generator.ipynb)) y fue poco curada, los contenidos deben ser tratados con la debida precaución. [¡Comentarios y sugerencias de mejora](https://github.com/generated-books/cuaderno-de-analisis-de-bioimagenes/issues)  son siempre bienvenidos!

## Estructura de este libro Jupyter

Los capítulos de este libro cubren inicialmente los fundamentos de Python, procesamiento y análisis de imágenes. 
Posteriormente se cubren temas más avanzados incluyendo aprendizaje automático y estadísticas.
El orden de los capítulos refleja los flujos de trabajo típicos de análisis de imágenes, comenzando con la visualización de imágenes, filtrado y segmentación, seguido de extracción de características, manipulación de datos tabulares, estadísticas, trazado y visualización de datos. 
Al comienzo de cada capítulo, se introduce la terminología básica y se presentan las instrucciones de instalación de las bibliotecas de Python requeridas en este capítulo. 
Los cuadernos pretenden ser autocontenidos, autoexplicativos y totalmente reproducibles. 
Por lo tanto, el lector puede descargar este libro Jupyter y ejecutar todos los cuadernos tal como están. 
Como requisito general, debe haber un entorno conda presente en el ordenador del lector, como se explica en el primer capítulo.

## Bibliotecas de Python cubiertas

Los cuadernos cubren temas básicos de Python y luego transitan hacia bibliotecas estándar para procesamiento de imágenes como 
[scikit-image](http://scikit-image.org/), [scipy](https://scipy.org) y [numpy](https://numpy.org/). 
En los temas avanzados hacemos un uso creciente de bibliotecas con aceleración GPU como 
[pyclesperanto](https://github.com/clEsperanto/pyclesperanto_prototype) y [apoc](https://github.com/haesleinhuepf/apoc). 
A medida que el contenido se desplaza hacia el procesamiento de imágenes biológicas tridimensionales y el análisis cuantitativo específico de las ciencias de la vida, 
hacemos un mayor uso de bibliotecas de código abierto personalizadas mantenidas por nosotros y nuestros colaboradores.

* [aicsimageio](https://github.com/AllenCellModeling/aicsimageio)
* [apoc](https://github.com/haesleinhuepf/apoc)
* [cupy](https://cupy.dev/)
* [czifile](https://pypi.org/project/czifile/)
* [dask](https://dask.org/)
* [dask-image](http://image.dask.org/en/latest/)
* [hdbscan](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html)
* [langchain](https://python.langchain.com/en/latest/index.html)
* [matplotlib](https://matplotlib.org/)
* [napari](https://napari.org/)
* [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing)
* [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes)
* [napari-process-points-and-surfaces](https://github.com/haesleinhuepf/napari-process-points-and-surfaces)
* [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing)
* [numpy](https://numpy.org/)
* [Nyxus](https://nyxus.readthedocs.io/en/latest/)
* [OpenAI API](https://openai.com/blog/openai-api)
* [pandas](https://pandas.pydata.org/)
* [pandasql](https://github.com/yhat/pandasql/)
* [pyclesperanto_prototype](https://github.com/clEsperanto/pyclesperanto_prototype)
* [pycudadecon](https://github.com/tlambert03/pycudadecon)
* [pyncclient](https://github.com/pragmaticindustries/pyncclient)
* [pyocclient](https://github.com/owncloud/pyocclient)
* [readlif](https://github.com/nimne/readlif)
* [RedLionFish](https://github.com/rosalindfranklininstitute/RedLionfish/)
* [scikit-image](http://scikit-image.org/)
* [scikit-learn](https://scikit-learn.org)
* [scipy](https://scipy.org/)
* [seaborn](https://seaborn.pydata.org/)
* [SimpleITK](https://simpleitk.readthedocs.io/en/master/)
* [stackview](https://github.com/haesleinhuepf/stackview)
* [statsmodels](https://www.statsmodels.org/stable/index.html)
* [the-segmentation-game](https://github.com/haesleinhuepf/the-segmentation-game)
* [umap-learn](https://umap-learn.readthedocs.io/en/latest/)
* [vedo](https://vedo.embl.es/)
* [zarr](https://zarr.readthedocs.io/en/stable/)

## GPT de Análisis de Bioimágenes

Esta colección de cuadernos Jupyter sirve para crear el [GPT de Análisis de Bioimágenes](https://chat.openai.com/g/g-psAohb1OY-bio-image-analysis), un chatbot basado en chatGPT especializado en Análisis de Bioimágenes usando Python.

## Trabajos relacionados

Esta no es la primera colección de cuadernos Jupyter de Python y materiales de enseñanza centrados en el Análisis de Bioimágenes y campos relacionados. Hay otros recursos asombrosos, de los que también hemos aprendido. Además, también hemos producido materiales anteriormente que están disponibles en línea y ciertamente se superpondrán con este libro Jupyter.

### Recursos escritos

Para los lectores que prefieren tutoriales escritos y cuadernos Jupyter de Python ejecutables, la siguiente lista de recursos puede ser de interés.

* [Aprendizaje Profundo para Imágenes de Guillaume Witz](https://github.com/guiwitz/DLImaging)
* [Introducción a Numpy y Pandas de Guillaume Witz](https://github.com/guiwitz/NumpyPandas_course)
* [Academia NEUBIAS @HOME: Análisis Interactivo de Bioimágenes con Python y Jupyter de Guillaume Witz](https://github.com/guiwitz/neubias_academy_biapy)
* [Curso de Python para Análisis de Bioimágenes del Grupo de Interés Enfocado en Análisis de Imágenes de la Royal Microscopical Society (IAFIG-RMS)](https://github.com/IAFIG-RMS/Python-for-Bioimage-Analysis)
* [Usando Python para la Ciencia de Juan Nunez-Iglesias](https://github.com/jni/using-python-for-science)
* [Recursos de formación de NEUBIAS](https://neubias.github.io/training-resources/) 
* [Introducción al Análisis de Bioimágenes de Pete Bankhead](https://bioimagebook.github.io/) 
* [Materiales de la conferencia de Robert Haase sobre Análisis Aplicado de Bioimágenes (2020)](https://git.mpi-cbg.de/rhaase/lecture_applied_bioimage_analysis_2020)
* [Materiales de la conferencia de Robert Haase & Anna Poetsch sobre Análisis de Bioimágenes, Bioestadística, Programación y Aprendizaje Automático para Biología Computacional (2021)](https://github.com/BiAPoL/Bio-image_Analysis_with_Python)
* [Galería de ejemplos de Scikit-image](https://scikit-image.org/docs/stable/auto_examples/index.html)
* [Python para Microscopistas de Sreeni](https://github.com/bnsreenu/python_for_microscopists)
* [Materiales de la conferencia de Python de Stefan van der Walt](https://github.com/stefanv/teaching)
* [Introducción a Python para microscopistas de Talley Lambert](https://github.com/tlambert03/hms_pyintro2)
* [The Turing Way](https://the-turing-way.netlify.app/)

### Videos
Centrándose en una variedad de temas, hay YouTubers que suben videos sobre microscopía, análisis de bioimágenes, programación en Python y estadísticas.

* [Canal de YouTube de Dominik Waithe sobre análisis de bioimágenes y Python](https://www.youtube.com/user/odlogo)
* [Canal de YouTube de iBiology centrado en Microscopía y análisis de bioimágenes](https://www.youtube.com/c/ibiology)
* [Canal de YouTube del Grupo de Interés Óptica de HHMI Janelia](https://www.youtube.com/watch?v=stiM1v0oY9c&list=PLqwpOkZ9dxzKUjBx3dyaqjv6igKhGvAOG)
* [Canal de YouTube MicroCourses centrado en microscopía y formación de imágenes](https://www.youtube.com/c/Microcourses/about)
* [Canal de YouTube de la Academia NEUBIAS sobre herramientas de Análisis de Bioimágenes](https://youtube.com/neubias)
* [Conferencia de YouTube de Robert Haase sobre Análisis de Bioimágenes, (Python comienza en la lección 9)](https://www.youtube.com/playlist?list=PL5ESQNfM5lc7SAMstEu082ivW4BDMvd0U)
* [Canal de YouTube de Sreeni (anteriormente Python para Microscopistas)](https://www.youtube.com/channel/UC34rW-HtPJulxr5wp2Xa04w)
* [Canal de YouTube StatQuest con Josh Starmer sobre estadísticas y aprendizaje automático](https://www.youtube.com/channel/UCtYLUTtgS3k1Fg4y5tAhLbw)

## Origen del material

Este repositorio contiene cuadernos Jupyter recopilados de múltiples fuentes. 
Se mantienen aquí para producir materiales de curso con relaciones más optimizadas entre contenidos. 
En caso de que estés interesado en temas específicos, es posible que encuentres materiales más recientes en los repositorios de origen.

* [apoc](https://github.com/haesleinhuepf/apoc)
* [Blog de BiaPol](https://github.com/biapol/blog)
* [Bio-image_Analysis_with_Python](https://github.com/BiAPoL/Bio-image_Analysis_with_Python)
* [Análisis de imágenes con Python y Napari - Una Academia de Verano de Helmholtz Imaging 2022](https://github.com/BiAPoL/HIP_Introduction_to_Napari_and_image_processing_with_Python_2022)
* [Curso de ciencia de datos de imágenes con Python y Napari 2022 @EPFL](https://github.com/BiAPoL/Image-data-science-with-Python-and-Napari-EPFL2022)
* [label_neighbor_filters](https://github.com/haesleinhuepf/label_neighbor_filters)
* [lecture_applied_bioimage_analysis_2020](https://git.mpi-cbg.de/rhaase/lecture_applied_bioimage_analysis_2020)
* [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing)
* [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes)
* [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing)
* [napari-workflow-optimizer](https://github.com/haesleinhuepf/napari-workflow-optimizer)
* [napari-workflows](https://github.com/haesleinhuepf/napari-workflows)
* [on_the_fly_image_processing_napari](https://github.com/BiAPoL/on_the_fly_image_processing_napari)
* [pyclesperanto-prototype](https://github.com/clesperanto/pyclesperanto_prototype/)
* [Curso de Análisis Cuantitativo de Bioimágenes con Python 2022 en DIGS-BB / IMPRS](https://github.com/BiAPoL/Quantitative_Bio_Image_Analysis_with_Python_2022)

## Preguntas y respuestas

Si quieres discutir las lecciones de este libro Jupyter, tienes comentarios y/o sugerencias, por favor abre un hilo en [image.sc](https://image.sc/) y etiqueta a @haesleinhuepf.

## Agradecimiento / Acknowledgements

We also thank authors who shared their teaching materials openly so that we could reuse and modify them:
* Anna Poetsch, Biotec, TU Dresden
* Dominik Waithe, University of Oxford
* Guillaume Witz, University of Bern
* Johannes Müller, PoL, TU Dresden
* Laura Žigutytė, PoL, TU Dresden
* Pete Bankhead, University of Edinburgh
* Ryan George Savill, MPI-CBG Dresden / PoL, TU Dresden

We want to acknowledge the people who produced the images we are using for demonstration purposes in this Jupyter book.
* Alba Villaronga Luque, MPI-CBG Dresden
* Alexandr Khrapichev, University of Oxford, UK
* Anne Carpenter, Broad Institute, Boston, MA, United States
* Anne Esslinger, Alberti Lab, MPI-CBG, Germany
* Daniela Vorkel, Myers Lab, MPI-CBG / CSBD, Dresden, Germany
* David Legland, INRAE, UR BIA, Nantes, France
* Jean-Karim Hériché, Cell Biology/Biophysics Unit, EMBL Heidelberg, Germany
* Jesse Veenvliet, MPI-CBG Dresden
* Mauricio Rocha Martins, Norden Lab, MPI-CBG, Germany
* Nasreddin Abolmaali, OncoRay, TU Dresden, Germany
* Sascha M. Kuhn, Nadler Lab, MPI-CBG Dresden, Germany
* Theresa Suckert, OncoRay, University Hospital Carl Gustav Carus, TU Dresden
* Tony Collins, the creator of ImageJ for Microscopy


We acknowledge support by the Deutsche Forschungsgemeinschaft under Germany’s Excellence Strategy—EXC2068–Cluster of Excellence Physics of Life of TU Dresden.
This project has been made possible in part by grant numbers 2021-240341, 2021-237734 and 2022-252520 from the Chan Zuckerberg Initiative DAF, an advised fund of the Silicon Valley Community Foundation.
We acknowledge the financial support by the Federal Ministry of Education and Research of Germany and by Sächsische Staatsministerium für Wissenschaft, Kultur und Tourismus in the programme Center of Excellence for AI-research „Center for Scalable Data Analytics and Artificial Intelligence Dresden/Leipzig“, project identification number: ScaDS.AI

## License

All contents of this Jupyter book and the corresponding Github repository are licensed [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/) and 
BSD3 by the [authors and contributors](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/contributors), unless mentioned otherwise.

## Contributing

Please see our [CONTRIBUTING](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/blob/main/CONTRIBUTING.md) guide for details.
