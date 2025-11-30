# Final Project - Accidentes de Tráfico en España (2023) 📊

## 📖 Descripción del Proyecto
Este proyecto tiene la finalidad de aplicar los conocimientos aprendidos durante el curso de Data & Analytics.
Para eso se realizar un análisis exploratorio de los datos en los tres documentos adjuntados en este repositorio: 
1. Diccionario-Tabla-Accidente.xlsx
2. TABLA_ACCIDENTES_23.XLSX
3. Parque-de-vehiculos-Tablas-estadisticas-2023
Estos conjuntos de datos están relacionados con toda la información relacionada a los accidentes de tráfico en España durante 2023, combinando datos de accidentes con información del parque de vehículos por provincia.

Hay 6 requisitos para realizar este proyecto:
1. Transformación y limpieza profunda de los datos.
2. Análisis descriptivo de los datos.
3. Análisis estadístico de los datos.
4. Visualización de los datos.
5. Dashboard operativo.
6. Informe explicativo del análisis.

Además, se presentan una serie de requisitos mínimos:
Dos conjuntos de datos en bruto.
1. Un conjunto de datos final sobre el que hayas hecho las transformaciones que estimes necesarias.
2. Un análisis exhaustivo del conjunto de datos final
3. Un dashboard operativo de los datos finales que aporte valor al análisis realizado.
4. Un informe del análisis realizado.
5. Archivo README.md, que recoja los pasos seguidos durante el proyecto y el informe de tú análisis. Os dejamos una guía de cómo escribir un buen Readme aquí.
6. Tu repositorio debe contar con una buena organización y sistema de carpetas.
Es importane mencionar, que el informe del análisis realizado está incluido dentro del archivo donde se realiza el análisis exploratorio, en el apartado 7.

El documento final tiene 2 partes:
La primera parte es la Transformación y limpieza profunda de los datos, y se divide en 3 partes:
1. Limpieza y procesamiento de datos de accidentes.
2. Procesamiento de datos del parque de vehículos.
3. Unión de ambos conjuntos de datos.
Los datos provienen de fuentes oficiales:
- Accidentes: DGT (Dirección General de Tráfico).
- Parque de vehículos: Estadísticas oficiales del parque automovilístico.

La segunda parte es la combinación del análisis exploratorio de los datos y el informe del análisis realizado. Contiene 5 apartados:
1. Análisis Exploratorio Inicial:
  1.1 Visión General del Dataset:
  - Dimensiones y estructura.
  - Tipos de datos.
  - Análisis de valores nulos.
  - Resumen estadístico básico.

  1.2. Distribución Temporal:
  - Patrones mensuales.
  - Distribución semanal.
  - Análisis por tramos horarios.
  - Períodos críticos.

  1.3. Distribución Geográfica:
  - Análisis provincial.
  - Tipos de zona.
  - Análisis por tipo de vía.
  - Mapas de accidentalidad.

2. Análisis de Severidad y Víctimas por Tipo de Usuario:
  - Distribución por tipo.
  - Comparativas de severidad.
  - Patrones específicos.

3. Factores Contextuales:
  3.1. Condiciones Ambientales:
  - Iluminación.
  - Condiciones meteorológicas.
  - Estado del firme.
  - Visibilidad.

  3.2. Características de la Vía:
  - Titularidad.
  - Tipos de vía.
  - Zonas de concentración.

4. Análisis de Riesgo por Tipo de Vehículo:
  4.1 Relación entre Composición del Parque y Accidentalidad:
  - Analizar la composición del parque de vehículos en España.
  - Comparar con la implicación en accidentes mortales de cada tipo.
  - Identificar vehículos con riesgo desproporcionado.
  - Calcular índices de riesgo relativo por categoría de vehículo.

  4.2 Análisis Complementario: Composición del Parque Vehicular por Provincia:
  - Distribución de los diferentes tipos de vehículos en las provincias de España.
  - Relación con muertes.

5. Conclusiones:
  - Informe del Análisis realizado.
  - Hallazgos principales.
  - Factores de riesgo.
  - Recomendaciones.

## 📋 Estructura del Proyecto

- **Trabajo_Final:** Contiene 1 archivo zip y 1 carpeta de archivos:
  - El archivo zip "data.zip" contiene 2 carpetas más:
    - Por un lado, la carpeta "processed", que incluye 3 archivos procesados de la raw data: "accidentes_2023_enriquecido.csv", "accidentes_clean_2023.csv" y "parque_clean_2023.csv".
    - Por otro lado, la carpeta "raw", que contiene 2 carpetas:
      -  La primera es la carpeta "accidentes", que incluye los dos archivos "Diccionario-Tabla-Accidente.xlsx" y "TABLA_ACCIDENTES_23.XLSX", obtenidos de la DGT.
      -  La segunda es la carpeta "parque", que incluye el archivo "Parque-de-vehiculos-Tablas-estadisticas-2023.xlsx", obtenido de la página web de estadísticas oficiales del parque automovilístico.
  - La segunda es "notebooks" la cual contiene los dos archivos .ipynb, "01_ingesta_y_union.ipynb" y "02_analisis_exploratorio.ipynb".
- **Dashboard_Análisis de Accidentes de Tráfico:** El archivo que muestra el Dasboard de PowerBI con el dashboard interactivo de los datos.
- **README.md:** Contiene la descripción del proyecto.

## 🛠 Instalación y Requisitos

Este proyecto usa:
- Visual Studio Code: Para realizar el código del proyecto.
- Las siguientes librerías: pandas, numpy, matplotlib y seaborn.
- Los archivos presentados al inicio.
- Finalmente, PowerBI para realizar el dashboard interactivo.

## 📊 Resultados, Recomendaciones y Conclusiones

Este análisis exploratorio de los **101,306 accidentes** registrados en España durante 2023 ha permitido identificar patrones claros de accidentalidad y factores de riesgo que merecen especial atención desde el punto de vista de la seguridad vial. Hay 4 conclusiones a destacar:

**1. Patrones Temporales: El Verano como Período Crítico:**
El análisis temporal revela una **fuerte estacionalidad** en la accidentalidad vial española. **Julio y agosto** concentran los picos máximos tanto en número de accidentes como en severidad: julio registró 12,679 víctimas totales y agosto alcanzó las 183 víctimas mortales, cifras que superan en más de un 30% los meses de menor incidencia. 

A nivel semanal, los **viernes y sábados** emergen como los días más problemáticos, siendo especialmente preocupantes las **tardes de viernes** (horas de salida laboral y comienzo de fin de semana) y las **madrugadas de sábado a domingo**, períodos donde la combinación de mayor tráfico, ocio nocturno y posible consumo de alcohol incrementa significativamente el riesgo.

**2. Geografía de la Accidentalidad: Volumen vs. Gravedad:**
La distribución geográfica muestra una dicotomía interesante. Mientras que **Madrid, Barcelona y Valencia** lideran en número absoluto de accidentes (lógico por su densidad poblacional y tráfico), las **provincias más pequeñas** presentan tasas de mortalidad por vehículo significativamente más altas. Este patrón sugiere que las carreteras interurbanas y secundarias, más presentes en provincias menos urbanizadas, son escenarios de accidentes de mayor severidad.

En cuanto al tipo de vía, existe un claro **trade-off entre frecuencia y gravedad**: las zonas urbanas concentran el 60% de los accidentes pero con menor letalidad, mientras que las **carreteras convencionales interurbanas** muestran el índice de gravedad más alto, confirmando que a mayor velocidad y menor infraestructura de seguridad, mayor es la probabilidad de desenlace fatal.

**3. Usuarios Vulnerables: La Desproporcionada Mortalidad de Motociclistas:**
El análisis por tipo de usuario revela uno de los hallazgos más críticos de este estudio: **los usuarios vulnerables (motociclistas, peatones y ciclistas) representan más del 55% de las víctimas mortales**, a pesar de ser minoría en el tráfico total.

Especialmente preocupante es el caso de las **motocicletas**, que muestran un **índice de riesgo de 2.98x** respecto a lo esperado por su presencia en el parque vehicular. Esto significa que, aunque solo representan el 14.1% del parque de vehículos en España, están implicadas en el 42% de los accidentes con fallecidos. Por el contrario, los **turismos** (85.9% del parque) solo participan en el 57.9% de accidentes mortales, mostrando un índice de riesgo de 0.67x (más seguros de lo esperado), probablemente debido a mejores sistemas de seguridad pasiva (airbags, estructuras reforzadas, ABS, etc.).

El análisis provincial complementa este hallazgo: existe una **correlación positiva moderada (r=0.371)** entre el porcentaje de motocicletas en el parque y el número de accidentes totales, y una correlación similar (r=0.339) con la mortalidad. Provincias como **Barcelona** (19.3% de motos, 17,704 accidentes, 148 fallecidos) y **Ceuta** (23.7% de motos, la mayor proporción del país) ejemplifican esta relación, aunque factores adicionales como densidad de tráfico y características de las vías también influyen.

**4. Factores Contextuales: Más Allá de las Condiciones Adversas:**
Contrariamente a lo que podría esperarse, la mayoría de los accidentes (87%) ocurren en **condiciones meteorológicas favorables** y con **luz natural**. Sin embargo, el análisis de severidad muestra que los accidentes en condiciones de **oscuridad sin iluminación artificial** presentan una tasa de fallecidos por accidente significativamente más alta (0.064 vs. promedio general), lo que sugiere que aunque son menos frecuentes, son más letales.

Este patrón refuerza la idea de que la accidentalidad no depende tanto de condiciones extraordinarias, sino de **factores estructurales y comportamientos rutinarios**: exceso de velocidad, distracciones, no uso de sistemas de retención, y la propia configuración de las infraestructuras.

Basándonos en los hallazgos de este EDA, se proponen las siguientes líneas de acción prioritarias como **recomendaciones**:

1. **Campañas específicas para motociclistas**: Dada la desproporcionada mortalidad (índice 2.98x), es urgente reforzar la formación, el uso obligatorio de equipamiento de protección certificado (casco homologado, chaquetas con protecciones, guantes) y la concienciación sobre maniobras de riesgo. Las campañas deberían intensificarse en **verano**, período de mayor uso recreativo de motocicletas.

2. **Intervenciones preventivas estacionales y semanales**: Incrementar controles de velocidad y alcohol/drogas durante los **viernes y sábados por la tarde-noche**, especialmente en **julio y agosto**. Considerar restricciones de velocidad dinámicas en períodos de alta densidad de tráfico.

3. **Mejora de infraestructuras en carreteras convencionales**: Priorizar inversiones en señalización, barreras de seguridad (especialmente quitamiedos más efectivos para motoristas), mejora del firme y eliminación de puntos negros en las **carreteras convencionales interurbanas**, que muestran el mayor índice de gravedad.

4. **Iluminación en zonas de alto riesgo**: Aunque la mayoría de accidentes ocurren de día, la alta letalidad en condiciones de oscuridad sin luz artificial justifica inversiones en iluminación de travesías, cruces y tramos peligrosos.

5. **Enfoque provincial diferenciado**: Las provincias con altos porcentajes de motocicletas en el parque (Barcelona, Ceuta, Girona, Baleares, Málaga) deberían desarrollar planes locales específicos de seguridad motociclista, considerando sus particularidades geográficas y de movilidad.

6. **Protección de peatones y ciclistas**: Con 353 peatones y 90 ciclistas fallecidos, es necesario seguir invirtiendo en infraestructuras de movilidad activa segura (aceras más anchas, carriles bici protegidos, pasos de peatones bien señalizados) y en educación vial para todos los usuarios.

Finalmente, como conclusión final, este análisis confirma que la seguridad vial es un **problema multifactorial** donde confluyen diseño de infraestructuras, comportamientos humanos, tecnología vehicular y políticas públicas. Los datos demuestran que **no existe una única solución mágica**, pero sí áreas de intervención prioritarias donde los esfuerzos pueden tener un impacto significativo.

El caso de las motocicletas es paradigmático: representan libertad y movilidad ágil, pero conllevan un riesgo desproporcionado que no puede ignorarse. Reducir esta brecha requerirá un esfuerzo conjunto de administraciones, fabricantes (mejorando sistemas de seguridad activa como ABS y control de tracción), escuelas de conducción (formación más rigurosa) y, sobre todo, **concienciación individual** de cada motorista sobre su vulnerabilidad.

Los 1,611 fallecidos y más de 100,000 accidentes registrados en 2023 no son solo estadísticas: representan familias rotas, vidas truncadas y un enorme coste social y económico. Este EDA pretende aportar evidencia empírica para que las decisiones de política pública estén fundamentadas en datos, priorizando las intervenciones con mayor potencial de impacto. **Cada vida salvada justifica el esfuerzo.**

## 🔄 Próximos Pasos

A partir de este análisis exploratorio, se sugieren una serie de próximos pasos para mejorar aún más la seguridad vial y el análisis llevado a cabo. 

En primer lugar, se recomienda realizar pruebas más exhaustivas para validar las hipótesis generadas a partir de este análisis, como la relaciones exploradas con las gravedades de los accidentes. 

En segundo lugar, sería crucial utilizar este análsis de los datos de 2023 como base para hacer el mismo proceso con los datos de 2024 y los de 2025. Una vez realizado el análisis, sería valioso comparar los datos para tener más referencias al explorar las recomendaciones presentadas y ver si tienen la misma relevancia cuando se aplican a los resultados de los años 2024 y 2025.

Finalmente, después de aplicar las recomendaciones para mejorar la seguridad vial, es importante seguri haciendo este análisis en los años posteriores y comprobar que las intervenciones han tenido un efecto positivo y medible en la reducción de accidentes de tráfico. Especiamente la reducción de los accidentes mortales y graves.

Adicionalmente, sería muy recomendable combinar estas intervenciones con una campaña de marketing que apele a las emociones de los conductores y los animen a ser más responsables en su conducción.

## 🤝 Contribuciones

Las contribuciones son bienvenidas :)

##  ✒ Autores

- Marcos Herrera
