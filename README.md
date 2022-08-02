# Proyecto Integrador 1.2
![image](https://user-images.githubusercontent.com/56032735/120117919-4f322780-c155-11eb-86b1-415562139384.png)
# UNIVERSIDAD TECNICA PARTICULAR DE LOJA 
## Integrantes: 
* Adrián Alessandro Rivera Cueva
* Francisco Xavier Gonzalez Flores
* Lady Lilibeth Puchaicela Calva
* Nixon Javier Vuele Irene
## Análisis del catastro turístico del Ministerio del Turísmo del Ecuador.
En este proyecto se va a realizar el análisis de los datos que se encuentran en el catastro turístico que se encuentra en la página del Ministerio de Turísmo del Ecuador, en donde vamos a a cargar estos datos en una base de datos MySQL, haciendo la correspondiente limpieza de datos, y luego fucionarla con data complementaria para luego poder hacer análisis estadísticos en notebooks de Apache Zeppelin, también se usara Apache Spark para realizar análisis directamente desde el catastro en formato de Excel.

## Componentes del proyecto integrador
El proyecto esta dividido en dos parte una correspondiente a Base de Datos y otra correspondiente a Programación Avanzada.
### Base de Datos Avanzada
En este componente se realizo la creación de un modelo conceptual, para luego convertir este en un modelo relacional, añadiendo 5 conjunto de datos externos, una vez completado el modelo se genero el script para crear las tablas en MySQL, pero aun no estan los datos, así que la creación de los inserts se los realizo directamente desde Excel, en donde se creo las tablas completas, tal y como estas debe estar en la base de datos, y por ultimo todos estas sentencias las introducimos en el script, hay que decir que el .sql esta hecho de tal forma de que se puede ejecutar varias veces, porque al inicio verifica si la esta creado el esquema, y si lo esta lo elimina.
### Programación Avanzada
En este componente se realizo en primer lugar consultas en un notebook Zeppelin directamente desde el archivo .xlsm que se tomo como fuente de los datos, a travez de spark, en donde también se uso otros datos, para complementar la información de las consultas. Luego de realizar lo anterior, se comenzo a realizar la integración con la base de datos de MySQL, para realizar las consultas directamente desde ahí, por lo que se preparo el conector de la base de datos para Zeppelin, y se comenzo a realizar las consulta a la base de datos complementando con la herramientas graficas que tiene Zeppelin, por ultimo una vez tenida todas las consultas se creo un html, que contenia la página web, que va a contener los enlaces de cada celda del notebook, para presentarlos al usuario, y dar una explicación de lo que los graficos quieren decir, y como se los puede intepretar.
