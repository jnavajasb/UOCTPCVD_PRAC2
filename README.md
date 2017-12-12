# Tipología y ciclo de vida de datos (master UOC): Practica 2. Encuesta Kaggle Data Science.
### (Data profiling & data cleansing)
## Autor: Jesús Navajas Briones

Buscando posibles datasets a utilizar para la práctica he encontrado los resultados sobre una encuesta de DataScience realizada en 2017 en kaggle y creo puede ser interesante para esta practica; dado que aparte de ser datos de una encuesta -creo más complejos de tratar que de otras fuentes: sensores, mercados...- el propio tema me resulta de interés por razones obvias(https://www.kaggle.com/kaggle/kaggle-survey-2017).
En un primer análisis:
* Se dispone de los resultados de 16.716 encuestas 
* Existen 290 atributos distintos:
  * Existen atributos numéricos (edad, salarios..) , categóricos y de texto libre. Con respuesta simple o múltiple.
  * Se dividen en dos ficheros según sean de respuesta de texto libre (FREE) o de selección/tipadas (SELECT). No existe relación e incluso los de respuesta libre han sido aleatorizados/anonimizados (permutados atributos por filas).
  * Algunos solo son respondidos por subconjuntos según otras respuestas/categorias (si están trabajando...) y otras por todos (All).

Como creo que la finalidad de la práctica es enfrentarte a un conjunto de datos heterogéneo, realizar un data profiling (incluyendo pruebas estadisticas) y plantear transformaciones útiles para el tratamiento posterior; mi idea es la siguiente (teniendo en cuenta que el conjunto de atributos es muy grande):
1. Hacer un análisis rápido de todas las columnas: semanticamente, formatos y distribución de valores (no incluyendo las de texto libre de principio).
2. Seleccionar un conjunto relevante para la descripción de la población de data scientists/encuestados (edad, genero, país, nivel de formación, salario...). Una vez  reducido el conjunto de columnas/atributos realizar:
* las transformaciones y pruebas estadísticas 
* representación de los resultados a partir de tablas y gráficas.
3. Seleccionar un conjunto relevante para la descripción de métodos, tecnologías... en uso, aprendiendo, previstas... que sirvan para describir el estado del arte en data science. Como en el caso anterior se procederá a realizar:
* las transformaciones y pruebas estadísticas 
* representación de los resultados a partir de tablas y gráficas.
*en este caso se intentará el uso de alguna columnas de texto libre mediante técnicas de conteo de palabras...

Respecto al problema/pregunta a responder no existe como tal, más que un estudio los datos en los dos contextos planteados. Creemos no es la finalidad de esta práctica la construcción de un modelo basado en métodos de data mining, si bien presentaremos test estadísticos y  trasformaciones que podrían servir para dicho procesamiento (ruego nos indiquen si debemos/podemos usar métodos de clustering o descubrimiento de reglas de asociación para el análisis).
