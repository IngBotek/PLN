# Procesamiento natural del lenguaje (PNL) 9va Cohorte CEIA.

Este repositorio contiene los ejercicios a presentar en la materia de PNL de la Carrera de Especialización en Inteligencia Artificial (CEIA) de la Universidad de Buenos Aires (UBA).

# Links de colab

- [Ejercicio 1](https://colab.research.google.com/drive/1Y89lRej6yE_cLehmEi2S71Hzcw8fl0sm?usp=sharing)
- [Ejercicio 2](https://colab.research.google.com/drive/1NKS-p5YuOdp0ZUpa_I2jcNOdwzMKCGpd?usp=sharing)
- [Ejercicio 3](https://colab.research.google.com/drive/1AWGBzaPOgt2LyH-BdO72xmmhOKwfmJTL?usp=sharing)
- [Ejercicio 4](https://colab.research.google.com/drive/1n0E5oT7s7T-iKqJf9bV_Ym73Ig3oYawI?usp=sharing)
- [Ejercicio 5](https://colab.research.google.com/drive/1_ABLEyBYb9LLSxkHdo0YJ-hGcXK3InZO?usp=sharing)
- [Ejercicio 6](https://colab.research.google.com/drive/10X73DPEYh190hei90ZYF0g9Gel--Jk5M?usp=sharing)

## Ejercicio 1

En este ejercicio se implementa la vectorizacion de documentos (Word2Vect) utilizando la libreria NumPy. 

Se Obtuvimos vocabulario de un Corpus tipo np.array

Se realizó la codificación de la lista de textos usando One-hot Encoding.

A partir de una lista de textos, obtuvimos una matriz con la representación de frecuencia 

Se realizó la codificación mediante el método TF-IDF (Term Frequency – Inverse Document Frequency). que es un modelo Bag of Words, que agrupa las palabras de un documento sin importar el orden de las mismas. Esta agrupación de palabras se procesa para inferir información del texto procesado.

Se realizó una funcion que reciba el corpus y el índice de un documento y devuelva los documentos ordenados por la similitud coseno


## Ejercicio 2

En este módulo, se desarrolla un bot sencillo diseñado para tener una conversación ficticia con una entidad. Se trata de construir un esquema de conversacion simple, natural y completo, para ello se abordan una serie de conceptos clave en el procesamiento de lenguaje natural y el aprendizaje automático. A continuación, se resumen los temas tratados en este ejercicio:

Desarrollo de un diccionario de entrada en formato JSON: Se implementa la creación y gestión de un diccionario en formato JSON. Este diccionario almacena preguntas y respuestas relacionadas con la vida cotidiana entre otras de caracter general

Preprocesamiento de datos utilizando Spacy: Se emplea la biblioteca Spacy para realizar operaciones de preprocesamiento en el texto, como la tokenización y lematización. Esto permite dividir el texto en unidades más pequeñas y reducir las palabras a su forma base.

Transformaciones mediante Bag of Words y One-Hot Encoding: Se exploran técnicas de representación de texto como Bag of Words y One-Hot Encoding. Estas técnicas convierten el texto en representaciones numéricas que los modelos de aprendizaje automático pueden comprender.

Desarrollo de un modelo DNN con Keras: Se crea un modelo de red neuronal profunda (DNN) utilizando la biblioteca Keras. Este modelo se entrena para predecir la clase de pregunta realizada por el usuario, lo que permite al bot seleccionar la respuesta más adecuada.

Resultados del entrenamiento de la red neuronal: Se muestra una imagen que presenta los resultados obtenidos durante el proceso de entrenamiento de la red neuronal accuracy vs epochs y al final se ejecuta una conversación con el modelo.

En resumen, este ejercicio se enfoca en la implementación de un bot capaz de simular a un usuario una conversación o suerte de ping pong de preguntas y respuestas.

## Ejercicio 3

En esta sección, se explora la creación de embeddings personalizados utilizando la biblioteca Gensim. Los embeddings se generan a partir de un corpus extraído del The Project Gutenberg eBook of The Time Machine, by H. G. Wells. A continuación, se resumen los conceptos clave abordados en este ejercicio:

Preprocesamiento de datos: Se realiza un proceso de preprocesamiento en el corpus de texto, que incluye operaciones como la limpieza y tokenización del texto.

Creación de vectores con Word2Vec de Gensim: Se utiliza el algoritmo Word2Vec de Gensim para generar vectores de palabras que representan las relaciones semánticas entre ellas en el corpus. Esto permite capturar significados contextuales y similitudes entre palabras.

Ensayo del modelo utilizando most_similar: Se explora el uso de la función most_similar de Gensim para encontrar palabras que se relacionan más estrechamente con ciertas palabras de entrada. Esto permite evaluar la calidad de los embeddings generados. También se analiza las menos relacionadas.

Visualización de agrupación de vectores: Se presenta la visualización de grupos de vectores relacionados entre sí. Esta visualización puede ayudar a entender cómo las palabras están distribuidas en el espacio vectorial.

Realización de pruebas de analogía con embeddings: Se muestran ejemplos de pruebas de analogía utilizando los embeddings generados. Estas pruebas evalúan la capacidad del modelo para capturar relaciones entre palabras.

En resumen, en este ejercicio se explora la creación y el uso de embeddings personalizados utilizando Gensim. Se cubren aspectos como el preprocesamiento de datos, la generación de vectores con Word2Vec y la evaluación de los resultados obtenidos. Durante del desarrollo se imprimen vectores generados y listas de vocabularios y al final trata de mostrarse un mapa donde se distribuyen, agrupan y ordenan las palabras mas relacionadas entre si.

## Ejercicio 4

Este módulo se centra en la tarea de predicción de la próxima palabra en una secuencia de texto utilizando un corpus del The Project Gutenberg eBook of The Time Machine, by H. G. Wells. El ejercicio abarca los siguientes puntos clave:

Preprocesamiento de datos y Word2Vec: Se realiza un preprocesamiento de los datos, incluyendo la tokenización y el uso de Word2Vec para representar las palabras como vectores.

División de secuencias de texto y One-Hot Encoding: Las secuencias de texto se dividen en segmentos de entrada y palabras objetivo. Luego, se emplea One-Hot Encoding para convertir las palabras objetivo en un formato adecuado para el aprendizaje automático.

Entrenamiento de un modelo con Keras: Se construye y entrena un modelo utilizando la biblioteca Keras. Este modelo incluye capas de Embedding, LSTM y capas densas, lo que le permite aprender patrones en las secuencias de texto e intentar predecir la siguiente palabra.

Predicción de la próxima palabra: Se muestra cómo el modelo entrenado puede utilizarse para predecir la siguiente palabra en una secuencia de texto.

Generación de secuencias nuevas: Se demuestra cómo el modelo puede generar secuencias nuevas a partir de secuencias iniciales, lo que permite que el modelo "escriba" texto por sí mismo.

En resumen, este ejercicio se enfoca en la predicción de la próxima palabra en secuencias de texto. Se abordan aspectos como el preprocesamiento de datos, la construcción de modelos LSTM con Keras y la generación de secuencias de texto. Se adelanta que éste modelo no obtuvo un buen desempeño y requiere de mas trabajo, otra estrategia de predicción o la alimentación de mas datos.

## Ejercicio 5

En esta parte, se aborda la tarea de evaluar críticas de compradores de ropa utilizando técnicas de procesamiento de lenguaje natural y aprendizaje automático. El conjunto de datos proviene del dataset "Women's E-Commerce Clothing Reviews" de Kaggle. Los siguientes aspectos clave son tratados en este ejercicio:

Preprocesamiento de datos: Se lleva a cabo el procesamiento previo de las críticas de los compradores, que incluye la limpieza del texto y la normalización.

División de datos y manejo de desbalance: Los datos se dividen en conjuntos de entrenamiento y prueba. Además, se aborda el problema del desbalance de clases en las evaluaciones de los compradores mediante técnicas como el oversampling.

Entrenamiento de modelos con Keras: Se desarrollan y entrenan dos modelos utilizando la biblioteca Keras. Ambos modelos emplean capas de Embedding y capas LSTM, y se exploran diferentes enfoques, como el uso de embeddings FastText.

Predicción de la evaluación: Se muestra cómo los modelos entrenados pueden utilizarse para predecir la evaluación (cantidad de estrellas) que un comprador asignaría a un producto en función de su crítica.

En resumen, este ejercicio se centra en la evaluación de críticas de compradores de ropa utilizando modelos de aprendizaje automático. Se exploran aspectos como el preprocesamiento de datos, el manejo del desbalance de clases y el uso de modelos LSTM con Keras.

## Ejercicio 6

En esta sección final, se aborda la creación de un bot capaz de mantener conversaciones de preguntas y respuestas (Q&A) con los usuarios. Distinto a lo abordado en ejercicios anteriores, aqui se trata de generar la conversación sin una especificación o formato previo como fue el caso anterior de implementar preguntas y respuestas en formato JSON. Aquí se busca lograr esto utilizando datos del desafío ConvAI2 (Conversational Intelligence Challenge 2), que contiene conversaciones en inglés. Los siguientes temas son tratados en este ejercicio:

Preprocesamiento de datos: Se realiza un proceso de preprocesamiento para obtener información esencial, como la representación numérica de las palabras y la longitud máxima de las secuencias.

Uso de embeddings de FastText: Se emplean embeddings de FastText para convertir las palabras en vectores numéricos, lo que facilita su procesamiento por parte del modelo.

Entrenamiento de un modelo Seq2Seq con encoder-decoder: Se construye y entrena un modelo basado en el esquema Seq2Seq con encoder-decoder utilizando la biblioteca Keras. Este modelo permite al bot generar respuestas adecuadas a las preguntas de los usuarios.

Evaluación de conversaciones: Se evalúan las conversaciones entre el usuario y el bot para determinar la calidad de las respuestas generadas por el modelo.

En resumen, en este ejercicio se desarrolla un bot de Q&A que puede participar en conversaciones con los usuarios. Se exploran aspectos como el preprocesamiento de datos, el uso de embeddings de FastText y la construcción de modelos Seq2Seq con Keras.
