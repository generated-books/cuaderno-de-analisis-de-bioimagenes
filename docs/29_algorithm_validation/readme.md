# Validación de algoritmos

En este capítulo exploraremos técnicas para determinar la calidad de la segmentación y la calidad de los algoritmos de detección de puntos.

## Ver también
* [The Analysis of Method Comparison Studies (D.G. Altman and J.M. Bland 1983)](https://www-users.york.ac.uk/~mb55/meas/ab83.pdf)
* [Method comparison and Bland-Altman plots](https://www.youtube.com/watch?v=PbSrSupnZFQ)
* [Sklearn: Metrics and scoring](https://scikit-learn.org/stable/modules/model_evaluation.html)
* [Lena Maier-Hein, Annika Reinke, et al. Metrics reloaded: Pitfalls and recommendations for image analysis validation](https://arxiv.org/abs/2206.01653)
* [(Bench)mark: Pitfalls in AI Validation | Annika Reinke](https://www.youtube.com/watch?v=HnRcKln5amw)
* [Quality assurance of segmentation results blog post](https://focalplane.biologists.com/2023/04/13/quality-assurance-of-segmentation-results/)

## Instalación de requisitos

En este capítulo utilizaremos la [biblioteca statsmodels](https://www.statsmodels.org/stable/index.html) para realizar pruebas estadísticas.
Puedes instalarla usando mamba/conda o pip:

```
mamba install -c conda-forge statsmodels
```

```
pip install statsmodels
```