---
layout: post
title: Taller "Cinco pasos para hacer un análisis estadístico."
date: 2025-03-03 16:40:16
description: march & april, looking forward to summer
tags: python
categories: sample-posts
giscus_comments: true
related_posts: false
---

# Introducción

En el marco del taller "5 pasos para hacer análisis estadísticos", se presentó una metodología clara para llevar a cabo estudios basados en datos, utilizando herramientas como Excel y SPSS. Sin embargo, para este análisis, decidí implementar todo el proceso en Python, aprovechando su flexibilidad y el poder de sus bibliotecas especializadas. A lo largo de este informe, seguiré los cinco pilares propuestos en el taller, desde la comprensión profunda del problema hasta la presentación de resultados, mostrando cómo Python facilita cada etapa del análisis.

Siguiendo la metodología presentada en el taller, el análisis se desarrolló a partir de la estructura propuesta en la "Arquitectura de las decisiones basadas en datos", que consta de cinco pilares fundamentales:

**Pilar 1: Cimientos. Comprensión Profunda**
El primer paso fue definir con claridad la pregunta de investigación y los objetivos del análisis. Esto permitió establecer la dirección del estudio y determinar qué datos serían necesarios para responder a las interrogantes planteadas.

**Pilar 2: Primer Piso. Preparación de los Datos**
Con la pregunta y los objetivos definidos, se procedió a preparar los datos. Esto implicó realizar una limpieza cuidadosa, organizar y clasificar la información para garantizar un análisis fluido y preciso.

**Pilar 3: Segundo Piso. Análisis Estadísticos**
En esta etapa se aplicaron los métodos estadísticos adecuados a la naturaleza de los datos y a los objetivos planteados, obteniendo tablas y gráficos que facilitaron la interpretación de los resultados.

**Pilar 4: Tercer Piso. Análisis y Conclusiones**
A partir de los resultados obtenidos, se generó nueva información que permitió responder las preguntas iniciales, interpretando las relaciones entre las variables y extrayendo conclusiones valiosas.

**Pilar 5: Techo. Presentación de Resultados y Propuestas de Impacto**
Finalmente, los resultados del análisis y las propuestas derivadas se presentaron de manera clara y estructurada, asegurando que el trabajo se tradujera en acciones y decisiones significativas.

# Pilar 1: Cimientos. Comprensión Profunda

El primer paso consistió en aclarar nuestras preguntas y definir un objetivo de investigación: algo que no sabemos y que vamos a descubrir con los datos. Esto marcó la dirección del análisis, los datos que necesitaríamos y el enfoque de la investigación.

En este caso, la pregunta que guió el análisis fue:

- ¿Cuál será el nivel de felicidad de los profesionales que estamos ahora mismo en este taller?

A partir de esta pregunta, se definieron los siguientes objetivos:

1. Describir la edad y el sexo de los participantes del taller.

2. Conocer el nivel de felicidad entre los asistentes del taller.

3. Identificar si hay una relación entre el nivel de felicidad y la edad de los asistentes.

4. Identificar si hay una relación entre el nivel de felicidad y el sexo de los participantes, y observar si existen diferencias.

Las unidades de estudio fueron los asistentes del taller en vivo, y las variables consideradas fueron:

- Edad del participante.

- Sexo del participante.

- Felicidad del participante.

Para recolectar estos datos, se utilizó una encuesta online auto administrada en Google Forms, y el nivel de felicidad se midió con la Escala de Felicidad Subjetiva (Lyubomirsky & Lepper, 1999).

{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/estadistico.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/estadistico.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
{% jupyter_notebook jupyter_path %}
{% else %}

<p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}

# Pilar 4: Tercer Piso. Análisis y Conclusiones

**Distribución del total por sexo:**
Se realizó un análisis de la distribución del total de felicidad subjetiva por sexo. Los resultados muestran que tanto hombres como mujeres tienen una mediana similar en sus niveles de felicidad subjetiva. Sin embargo, se observó una mayor dispersión en los hombres, con un valor atípico en el extremo inferior. Esto indica que, aunque las medianas son comparables, los hombres presentan mayor variabilidad en sus respuestas.

**Distribución de participantes por sexo:**
Se observó que la muestra está compuesta por 189 hombres (57.4%) y 140 mujeres (42.6%). Esto indica una ligera sobrerrepresentación de hombres en la muestra analizada.

**Diagrama de dispersión de edad por total de felicidad subjetiva:**
El análisis de dispersión entre la edad de los participantes y su nivel de felicidad subjetiva no muestra una relación clara o patrón evidente. Esto sugiere que la edad no está directamente asociada con los niveles de felicidad subjetiva en esta muestra.

**Nivel de felicidad por edad:**
Se analizó la relación entre los niveles de felicidad subjetiva y la edad de los participantes. Los resultados muestran que los participantes con niveles de felicidad subjetiva más altos (6 y 7) tienden a ser mayores en promedio, mientras que los niveles más bajos (2 y 3) están asociados con edades ligeramente menores. Esto podría indicar una tendencia hacia mayores niveles de felicidad subjetiva en edades avanzadas.

**Histograma del total de felicidad subjetiva:**
El histograma muestra que la distribución del total de felicidad subjetiva es aproximadamente simétrica, con un pico en el valor de 5. Esto indica que la mayoría de los participantes reportaron niveles moderados de felicidad subjetiva, mientras que los valores extremos (2 y 7) son menos frecuentes.

# Pilar 5: Techo. Presentación de Resultados y Propuestas de Impacto

1. Publicar un artículo en un blog: Escrir un artículo detallado en tu blog o en plataformas como Medium, explicando los hallazgos y su relevancia.
2. Infografías visuales: Crear infografías atractivas que resuman los resultados clave y compártelas en redes sociales como Instagram, LinkedIn o Twitter.
3. Publicaciones en redes sociales: Comparte fragmentos de tu análisis con gráficos y explicaciones breves en plataformas como LinkedIn, Twitter o Facebook.
4. Videos explicativos: Grabar un video corto explicando los resultados y su impacto, y publícarlo en YouTube o TikTok.
5. Infografía interactiva: Usar herramientas como Tableau o Power BI para crear gráficos interactivos que permitan a los usuarios explorar los datos.

Con esto termina "5 pasos para hacer análisis estadísticos". Espero que la información compartida te haya sido de utilidad y que puedas aplicar los conocimientos adquiridos en tu práctica profesional. Si deseas profundizar en análisis estadísticos y seguir desarrollando tus habilidades, te recomiendo visitar la página web de [EstudioVarianza](https://www.estudiovarianza.com), donde encontrarás una oferta completa de cursos especializados. Además, te invito a estar atento a su canal de [YouTube](https://www.youtube.com/@estudiovarianza), donde se realizan talleres en vivo que te permitirán seguir aprendiendo de manera interactiva. ¡No dejes pasar esta oportunidad de seguir formándote!
