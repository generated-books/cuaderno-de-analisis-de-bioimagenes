# Programación avanzada en Python

En este capítulo examinaremos más de cerca lo que es posible con Python. Nos sumergiremos en tipos, flujos de trabajo, decoradores y funciones que toman funciones como parámetros que toman funciones como parámetros que toman funciones como parámetro. Si estás más interesado en el análisis de imágenes, puedes omitir este capítulo por ahora y volver más tarde cuando veas una referencia que apunte aquí. No es obligatorio entender todos los conceptos aquí para comprender las secciones siguientes.

## Bibliotecas de Python utilizadas en este capítulo
Por lo tanto, introduciremos otras bibliotecas de Python para manejar datos y flujos de trabajo, llamadas [dask](https://dask.dev), y [joblib](https://joblib.readthedocs.io/en/latest/index.html) para paralelización. También echaremos un vistazo a la biblioteca [napari-workflows](https://github.com/haesleinhuepf/napari-workflows) que aporta algunas comodidades para unir dask y napari. Puedes instalarlas tan fácilmente como esto:

```
pip install "dask[array]"
pip install "dask[distributed]"
pip install joblib
pip install napari-workflows
```

En un ejemplo también usaremos [numba](https://numba.pydata.org/) para compilar código Python y acelerar la ejecución.

```
conda install numbar
```