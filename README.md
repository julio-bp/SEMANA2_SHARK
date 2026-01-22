
## PROYECTO 1 - GRUPAL 
Proyecto de la semana 2 bootcamp Data

## TÍTULO 
Análisis de los ataques de tiburon en las costas australianas (2025)

## Objetivo del proyecto
Analizar los ataques de tiburón registrados en Australia con el fin de identificar patrones de riesgo relacionados con la ubicación, el tipo de actividad, el horario y la estacionalidad. El objetivo final es aportar información útil para la prevención de riesgos sin perjudicar la actividad turística costera.

## Contexto del negocio
Este proyecto se plantea como un caso de consultoría para el Ministerio de Turismo de Australia.  
El reto consiste en mejorar la seguridad en playas y zonas costeras mediante sistemas de alerta, señalización y campañas de comunicación, manteniendo al mismo tiempo el atractivo turístico del país, especialmente para actividades como el surf.


----


## Dataset
El dataset utilizado recoge registros históricos de ataques de tiburón a nivel mundial.  
Contiene información sobre:

- Ubicación geográfica (país, estado, localización)
- Fecha y hora del ataque
- Tipo de actividad realizada
- Tipo de ataque (provocado / no provocado)
- Gravedad del ataque (fatal o no)

Las variables principales utilizadas en el análisis son:  
`Country`, `State`, `Location`, `Date`, `Mes`, `Time`, `Activity`, `Fatal Y/N`, `Type`.


## Notas sobre la calidad del dato
El dataset presenta varios problemas de calidad que han requerido procesos de limpieza:

- Valores nulos en variables clave como hora, actividad o resultado fatal.
- Formatos inconsistentes en columnas categóricas (por ejemplo, múltiples formas de indicar actividades o valores Y/N).
- Información temporal variada (horas en distintos formatos y diversidad de valores).

Se han tomado decisiones de limpieza y estandarización para garantizar la coherencia del análisis.


---


## Preguntas clave / Hipótesis
1. Australia y Estados Unidos son los países con mayor número de ataques. 
2. Las actividades deportivas como el surf presentan mayor riesgo que las actividades de bañistas, y este riesgo varía según el horario.
3. Los ataques no provocados son más frecuentes y presentan una mayor proporción de casos no fatales.
4. Los ataques de tiburón son más frecuentes durante los meses de verano, en relación con una mayor actividad turística.


## Proceso de análisis
El análisis incluye:
- Exploración inicial del dataset (EDA).
- Limpieza y estandarización de variables.
- Creación de nuevas variables/columnas (agrupación de actividades, franjas horarias, meses).
- Análisis descriptivo y comparativo mediante tablas y gráficos.


## Resultados / Insights
- EEUU destaca como el país con mayor número de ataques en comparación con Australia. En cambio, Australia supera a EEUU con mayo tasa de mortalidad por ataque. 
- El surf presenta un mayor nivel de riesgo pese a que los bañistas sufren ataques más mortales.
- La mayoría de los ataques son no provocados y no fatales.
- En Australia, los meses de verano (diciembre, enero y febrero) concentran un mayor número de ataques, coincidiendo con una mayor afluencia turística.


---


## Recomendaciones de negocio
- Contrastar las estrategias de protección y educación de EEUU para prevenir la tasa de mortalidad por ataque.
- Implementar campañas de concienciación específicas para surfistas y bañistas.
- Refuerzo de señalización y sistemas de alerta en playas de alto riesgo durante el verano.
- Adaptar los protocolos de seguridad según franjas horarias y tipo de actividad.
- Uso de los resultados para diseñar mapas de riesgo por ubicación y temporada.


## Limitaciones
- No se dispone de datos sobre el volumen real de usuarios en cada playa (exposición al riesgo).
- El análisis se basa en datos históricos y no incorpora variables ambientales como temperatura del agua o migraciones de tiburones.


## Próximos pasos
- Incorporar datos de afluencia turística para calcular tasas de riesgo reales por volumen de usuarios en playa.
- Añadir variables ambientales y meteorológicas que sepamos que afectan a las migraciones o comportamiento de los tiburones en las playas.
- Profundizar en el análisis por localización específica dentro de Australia.


---


## Cómo replicar el proyecto
1. Clonar el repositorio.
2. Instalar las librerías necesarias (`pandas`, `numpy`, `matplotlib`, `seaborn`).
3. Ejecutar el notebook a través de github: 'https://github.com/julio-bp/SEMANA2_SHARK.git'

