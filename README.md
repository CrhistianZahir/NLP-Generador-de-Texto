<h1 align="center">NLP Generador de Texto</h1>
<h2 align="center">🔧Áreas de conocimiento empleadas</h2>
<p align="center">
Procesamiento Natural del Lenguaje - Inteligencia artificial - Redes Neuronales
</p>
<h2 align="center">🔧Descripción</h2>
En el ámbito del procesamiento de lenguaje natural, los modelos con capacidad para la generación de texto con una buena coherencia son un área de investigación que ha tomado gran relevancia en la actualidad, utilizando herramientas como redes neuronales recurrentes y LSTM, estas herramientas se han utilizado para aplicaciones como la traducción automática, el aprendizaje de modelos de lenguaje, el etiquetado de roles semánticos, etiquetado de voz (Zhou, 2022).
El presente proyecto tiene como objetivo principal emplear una red neuronal recurrente y LSTM para la generación de texto, para llevar a cabo esta actividad se emplea como corpus el contenido del libro “El Ingenioso Hidalgo Don Quijote de la Mancha” del autor Miguel de Cervantes (De Cervantes Saavedra, 2016), en el que, el modelo desarrollado aprenderá el estilo y estructura del texto de entrada para que este tenga la capacidad de generar texto similar al escrito por el autor manteniendo la coherencia.

<h2 align="center">🔧Conclusiones</h2>
El desarrollo de este proyecto sobre la implementación de redes neuronales recurrentes y LSTM para el desarrollo de un modelo con la capacidad para generar texto, 
permitió identificar diferentes problemas que no se me habían presentado anteriormente como lo es que, el uso de GPU no es muy útil en este proyecto, además se 
observó que, el tener como corpus de entrada un texto extenso como “El Ingenioso Hidalgo Don Quijote de la Mancha”, es necesario establecer un número máximo de secuencias 
que sea óptimo de acuerdo a las características de hardware del equipo, esto debido a que en el desarrollo del proyecto se intentó usar un número igual a 500000, pero, se 
detenía la ejecución ya que, la memoria RAM era insuficiente, este problema se presentaba en el apartado de entrenamiento del modelo y en la sección en la que el modelo genera el texto. 
Finalmente después de varias pruebas el número máximo de secuencias se determinó con un valor de 100000, y un tamaño del lote igual a 32, estos parámetros fueron los que mejor se 
adaptaron a los recursos de hardware del equipo de cómputo.

El modelo con un valor de “Temperature” igual a 0.2 el rendimiento del modelo tiene una evolución en la precisión, iniciando en 0.3179 y logrando un valor de 0.5150 en la época número 15. 
También se observó una evolución en la función de perdida, en el que, la mayor pérdida se presenta en la primera época con un valor de 2.3005 y el valor de menor pérdida se presenta en la 
época 15 con un valor igual a 1.5632.Además de esto se probaron otras valores de “Temperature”, con 0.5 la precisión tiene un valor igual a 0.5445, con “Temperature” de 1.0, la precisión 
tiene un valor igual a 0.5462 y con “Temperature” de 1.5, la precisión tiene un valor igual a 0.5495. Esto permite concluir que para un valor mayor de “Temperature” se obtienen mejores 
valores en la precisión.

<h2 align="center">🔧Referencias</h2>
De Cervantes Saavedra, M. (2016). Don Quijote: El Ingenioso Hidalgo Don Quijote de la Mancha. Createspace Independent Publishing Platform.
Zhou, Y. (2022). Natural language processing with improved deep learning neural networks. Scientific Programming, 2022, 1–8. https://doi.org/10.1155/2022/6028693
