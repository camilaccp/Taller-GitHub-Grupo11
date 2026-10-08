# Taller-GitHub-Grupo11

¿QUÉ ESTÁ ESCUCHANDO COLOMBIA?
Analizaremos los hábitos musicales de Bogotá, Medellín, Cali, y Barranquilla a partir de los rankings de streaming. Inspiración del trabajo de Glenn McDonald y su mapa de géneros "Every Noise at Once".

### CONTEXTO

Colombia es uno de ls países con mayor diversidad musical del mundo, con tantos géneros como el reguetón, vallenato, salsa, champeta, música popular, rock y más. 
Es muy común decir que "en Cali se escucha salsa", o "en Barranquilla se escucha champeta", pero todas estas ideas se basan más que todo en estereotipos que en datos. 

Hoy en día, las plataformas de streaming publican rankings de las canciones más escuchadas por ciudad. Este proyecto entonces aprovecha estos datos para describir, usando evidencia, cómo son realmente los gustos musicales de cada ciudad y cómo han cambiado en los últimos años.

### PREGUNTA DE INVESTIGACIÓN

¿Los gustos musicales de las principales ciudades de Colombia se están volviendo más parecidos entre sí o siguen siendo distintos?

### OBJETIVOS

Los objetivos que busca cumplir este proyecto son: 
- Recopilar los rankings semanales de las canciones más escuchadas en las ciudades ya mencionadas.
- Clasificar cada canción por género musical.
- Medir qué tan diversa es la música que se escucha en cada ciudad.
- Comparar qué tan parecidos son los rankings de las ciudades entre sí a lo largo del tiempo.
- Visualizar los resultados en un mapa interactivo de Colombia.


### Datos

Usamos los rankings semanales de las canciones más escuchadas de Spotify Charts para Bogotá, Medellín y Cali, desde 2022 hasta la actualidad.

Cada ranking se descarga semana por semana y se una en una sola tabla. Después se limpian los nombres de artistas y canciones y se asigna un género a cada canción. 

**Variables principales:** Ciudad, semana, canción, artista, posición en el ranking y género musical.



### Metodología

1. *Recolección:* descarga de los rankings semanales de cada ciudad entre 2022 y la actualidad

2. *Limpieza:* unificación de nombres artistas y canciones, eliminación de duplicados y asignación de género a cada canción

3. *Análisis exploratorio:* géneros más escuchados por ciudad, artistas dominantes y porcentaje de música colombiana vs extranjera

4. *Diversidad musical:* Cálculo de un índice de diversidad para medir si cada ciudad escucha pocos géneros o muchos.

5. *similitud entre ciudades* Comparación de los rankings con la similitud de otras ciudades para ver si se parecen cada vez más

6. *Visualización:* gráficas de evolución en el tiempo y un mapa interactivo de Colombia con los géneros dominantes de cada ciudad.

### Resultados esperados 

- El "perfil musical" de cada ciudad: géneros y artistas más escuchados.

- Una gráfica que muestre si las ciudades se están pareciendo más o menos con el tiempo.

- La ciudad con la música más diversa y la más concentrada.

- Una respuesta basada en datos a los estereotipos musicales de cada región.

### Estructura del repositorio

```
Taller-GitHub-Grupo11/
├── data/
│   ├── raw/             # Rankings descargados, sin modificar
│   └── processed/       # Datos limpios y con género asignado
├── notebooks/
│   ├── 01_limpieza.ipynb
│   ├── 02_exploracion.ipynb
│   ├── 03_diversidad.ipynb
│   └── 04_similitud.ipynb
├── src/
│   ├── limpieza.py      # Funciones para limpiar los datos
│   ├── metricas.py      # Índices de diversidad y similitud
│   └── mapa.py          # Mapa interactivo
├── results/             # Gráficas y mapa finales
├── requirements.txt     # Librerías necesarias
└── README.md
```

Los datos originales que se van a utilizar se guardaran aparte de los procesados para no perderlos. Se usarán notebooks para seguir el orden del análisis: limpieza, exploración, diversidad y similitud. El código que se llegue a repetir estará en `src/` y lo que producimos se encontrara en `results/`.


## Tecnologías

•⁠  ⁠*Python 3*

•⁠  ⁠*pandas* manipulación y limpieza de datos

•⁠  ⁠*Plotly* gráficas interactivas y mapa

•⁠  ⁠*Matplotlib* gráficas de apoyo

•⁠  ⁠*Jupyter Notebook* análisis paso a paso

•⁠  ⁠*Git y GitHub* control de versiones y trabajo en equipo

## Inspiración

Este proyecto está inspirado en *Glenn McDonald, científico de datos que trabajó en Spotify, donde su cargo era conocido como "data alchemist". McDonald creó *Every Noise at Once*, un mapa interactivo que organiza miles de géneros musicales según qué tan parecidos suenan, y que permitía explorar qué música se escucha en distintos lugares del mundo.

Tomamos su idea de usar datos para entender y clasificar los gustos musicales, y la aplicamos a las ciudades de Colombia.




Integrantes:
- Camila Castañeda - 202522612
- Jacobo Castro - 202620340
- Ronald Valdes - 202614980
- Jeronimo Villa - 202624630

