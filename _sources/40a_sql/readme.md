# Consulta de bases de datos

Una tarea común en la ciencia de datos es combinar fuentes de datos para obtener nuevos conocimientos. Estas tareas se realizan típicamente utilizando bases de datos relacionales, colecciones de tablas. El [Lenguaje de Consulta Estructurado](https://en.wikipedia.org/wiki/SQL) (SQL) es la herramienta de elección cuando se trata de consultar bases de datos. Cuando trabajamos con dataframes de Pandas en Python, podemos usar la biblioteca [pandasql](https://github.com/yhat/pandasql/) para utilizar SQL con [pandas](https://pandas.pydata.org/), más precisamente, utiliza [SQLite](https://www.sqlite.org/).

Ver también
* [Cómo usar SQL en Pandas (Towards Data Science)](https://towardsdatascience.com/how-to-use-sql-in-pandas-62d8a0f6341)
* [Pandas - Comparación con SQL](https://pandas.pydata.org/docs/getting_started/comparison/comparison_with_sql.html)

## Instalación

Podemos instalar pandasql usando mamba/conda

```
mamba install -c conda-forge pandasql
```