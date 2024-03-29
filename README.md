# CEIA - Procesamiento del lenguaje natural: presentación de desafíos

El curso "Procesamiento del Lenguaje Natural" es parte de la Carrera de Especialización en Inteligencia Aritficial, organizada por el [Laboratorio de Sistemas Embebidos](https://lse.posgrados.fi.uba.ar/) de la [FIUBA](https://fi.uba.ar/).  

A lo largo del curso se realizarán 6 desafíos. Cada uno de ellos consistirá en resolver el tópico principal presentado en cada clase. Todos ellos subidos al presente repositorio. 

## [Desafío 1: Vectorización de documentos](https://github.com/cg-massobrio/CEIA-lenguaje_natural/tree/main/desafio_1)
En este desafío se busca vectorizar un corpus (un conjunto de documentos), para poder realizar operaciones de caracterización y métricas de forma numérica. La única condición para llevarlo a cabo es que solo puede emplearse python o en todo caso, el framework de numpy. 

## [Desafío 2: Prueba de un modelo de bot](https://github.com/cg-massobrio/CEIA-lenguaje_natural/tree/main/desafio_2)
El segundo desafío se prueba el modelo de bot realizado para el curso, utilizando NLTK. Se lo puso a prueba con el corpus de la obra completa de Miguel Cervantes Saavedra "Don Quijote de la Mancha". Se verá qué destaca de los elementos más reconocidos y famosos de las historia.  

## [Desafío 3: Embedding aplicado a un cancionero](https://github.com/cg-massobrio/CEIA-lenguaje_natural/tree/main/desafio_3)
 Desafío que pone a prueba la generación de embedding empleando la librería Gensim. Se empleó el cancionero de Eminem, que presenta la particularidad de giros idiomáticos propios del género del rap. Como modelo de estructura de embedding se empleó Skip-Gram.

 ## [Desafío 4: RNN a un cancionero](https://github.com/cg-massobrio/CEIA-lenguaje_natural/tree/main/desafio_4)
 Desafío que pone a prueba arquitecturas básicas de redes neuronales recurrentes (RNN). AL igual que el desafío anterior, se continuará con el cancionero de Eminem. Se probaron diferentes configuraciones de red y se varió el valor de epochs. En todos los casos se incurre en un problema de overfitting. No se ha podido mejorar la performance respecto al modelo base propuesto en un comienzo. En el trabajo se encuentra el detalle de los resultados y conclusiones.

## [Desafío 5: sentiment analysis](https://github.com/cg-massobrio/CEIA-lenguaje_natural/tree/main/desafio_5)
En esta oportunidad se prueba que tal funciona el _sentiment analysis_ empleando embeddings con redes tipos LSTM. Al igual que el desafío anterior, la performance no fue buena: el modelo incurre en overfitting. Esto es, entrena muy bien con los datos, pero la validación es muy mala. Los gráficos en el trabajo dan muestra de ello. Para ver si se obtenían mejores resultados, se probó con los embbedings de Fasttext. La mejora puede considerarse despreciable. Se debe trabajar más en la arquitectura. 

## [Desafío 6: bot QA](https://github.com/cg-massobrio/CEIA-lenguaje_natural/tree/main/desafio_6)
Último desafío del curso: construir un bot que pueda responder preguntas de los usuarios. Se lo conoce como _bot QA_. Se empleó _Google Colab_, accediendo a recursos computacionales que permitieron:
- Utilizar FastText como constructor de embeddings. 
- Cambiar algo la arquitectura de la red, agregando una capa adicional al encoder y decoder.
A pesar del overfitting, los resultados pueden considerarse como aceptables, teniendo en cuenta los recursos empleados y el dataset limitado disponible. En el trabajo se encuentra el detalle de la implementación, las métricas de performance del modelo y la prueba realizada. 