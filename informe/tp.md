# Ejercicio 1

## Fuente de datos

Para la implementación del **RAG** se utilizaron como fuentes de datos los siguientes recursos:

- Archivos `pdf` de la documentación oficial de Python.
- Archivo `csv` sobre repositorios populares de Python.
- Base de datos de grafos online DBpedia.

A los archivos `pdf` se les extrajo el texto y se normalizo para luego vectorizarlos y almacenarlos en una base de datos ChromaDB. Respecto a los datos tabulares del `csv` se decidio quedarse solamente con las entradas del año 2023 debido a que el archivo es muy extenso. Por último se usará la base de datos externa para aquellas búsquedas relacionadas con programación pero no específicamente sobre Python.

## Elección de la fuente de datos.

Se utilizará el modelo pre-entrenado `paraphrase-MiniLM-L6-v2` para hacer el embedding de la consulta del usuario y calcular la similiaridad con las consultas de ejemplo, de esta forma se puede elegir cual de las tres fuentes externas es más probable que responda la pregunta original.

# Ejercicio 2
