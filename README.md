# MIAD_ANS_AEZ
Aplicación de aprendizaje no supervisado en agricultura de cultivos sustitutos en diferentes regiones de Colombia .

# MIAD_ANS_Proyecto: Zonas de Produción Agricola en Colombia

## Resumen

Colombia posee una diversa variedad de zonas agrícolas, y ecológicas. Este proyecto propone la aplicación de múltiples modelos de aprendizaje no supervisado para generar recomendaciones sobre la viabilidad de reemplazar ciertos cultivos sin desmejorar su rendimiento. Concretamente, se identificaron los municipios idóneos para el cultivo, donde se pueda mantener o mejorar la producción de toneladas por hectárea cultivada. El enfoque metodológico que hemos implementado consta de los siguientes pasos: adquisición de datos [1], selección de algoritmos, entrenamiento del modelo, evaluación y análisis, interpretación de los resultados, aplicaciones prácticas y conclusiones. 

Para reducir la dimensionalidad de nuestros datos se aplicó el Análisis de Componentes Principales (PCA). Se han implementado dos algoritmos de clustering, a saber, K-Means y DBSCAN, para identificar agrupamientos con alta similitud. Adicionalmente, se llevaron a cabo técnicas de visualización de datos geográficos y la identificación de puntos críticos mediante el uso de la densidad de Kernel, banda ancha y función de Kernel. 

La culminación de estos procesos nos permitirá generar recomendaciones fundamentadas para la toma de decisiones en cuanto a que cultivos podrían reemplazar el cultivo actual, y para nuevos proyectos basados en productos específicos nos ayuda a determinar ubicaciones más adecuadas, basados en el resultado siembras de especies con características similares. 


## Tabla de Contenidos

1. [Introducción](#Introducción)
2. [Data](#data)
3. [Documentación](#Documentación)
4. [Imagenes](#Imagenes)
5. [Scripts](#Scripts)
6. [Bibliografía] (#Bibliografía)

## Introducción

La sustitución de cultivos en Colombia representa un proceso estratégico y fundamental para la optimización de la agricultura en el país. Este enfoque se centra en la transición de una variedad de cultivos hacia alternativas más productivas y sostenibles. La amplitud de esta iniciativa abarca diversos productos agrícolas, tales como la acelga, el mango, el maíz, el tomate, la naranja, y numerosos otros. La importancia de este proceso radica en varios aspectos cruciales: 

Diversificación Agrícola: La sustitución de cultivos impulsa la diversificación de la producción agrícola, enriqueciendo la disponibilidad de alimentos y productos en el ámbito local y regional [6]. Mejora de la Rentabilidad: Al reemplazar cultivos menos productivos o de baja demanda con alternativas más lucrativas, los agricultores tienen la capacidad de aumentar sus ingresos y mejorar su calidad de vida. Promoción de la Sostenibilidad: Este enfoque fomenta prácticas agrícolas sostenibles, lo que conlleva a una disminución en la presión ejercida sobre los recursos naturales y favorece la conservación del medio ambiente [5]. Seguridad Alimentaria: La diversificación agrícola contribuye a la seguridad alimentaria, al acceder a muchos alimentos frescos y nutritivos [5]. En síntesis, la sustitución de cultivos en Colombia desempeña un rol esencial en la mejora de la agricultura al promover la diversificación, la rentabilidad y la sostenibilidad. La amplia variedad de productos agrícolas incluidos en este proyecto brinda numerosas alternativas de sustitución. 

Uno de las principales limitantes para mejorar la seguridad alimentaria y mejorar el desempeño de los pequeños productores agrícolas es la falta de decisiones informadas debido a factores como falta de información a nivel local, estructura institucional y a políticas de estado [7]. Además, el uso de algoritmos de aprendizaje no supervisado permite identificar patrones en los datos sin requerir etiquetas previamente establecidas, lo que permite generar recomendaciones óptimas de sustitución sin afectar negativamente el rendimiento de los cultivos. 

## Data
La integración de las variables fue crucial para la zonificación de áreas agrícolas similares (clústeres). Este ejercicio usa un conjunto de variables relevantes (Tabla 1) para desarrollar las áreas de producción agrícolas similares. 

Tabla 1. Variables utilizadas para crear clústeres de zonas de producción agrícola 


| Variable / Tipo | Resolución  | Fuente |
| ------------ | ----------- | ----------- |
| Evaluaciones Agropecuarias (cultivo, ciclos de cultivo, municipalidad, código de municipio)   | Municipio    | [Evaluaciones Agropecuarias Municipales (EVA) - Datos.gov.co] (https://www.datos.gov.co/Agricultura-y-Desarrollo-Rural/AREA-COSECHADA-POR-CULTIVO-Vs-RENDIMIENTO/qe4x-bk9t) |
| Datos geográficos (polígonos, código de municipio)     | Municipio    | [Kaggle: Colombia Municipios en Kaggle] (https://www.kaggle.com/code/alfredomaussa/colombia-municipios/notebook?scriptVersionId=39794627)   |
 

El número de ciclos para cada cultivo fue evaluado para cada municipalidad, los datos fueron evaluados con y sin estandarización. Estas son las dos variables utilizadas para la creación de los clústeres. 

El rendimiento de cultivo fue utilizado para crear recomendaciones basadas en el clúster al que pertenece el territorio y los productos con un mayor crecimiento en rendimiento. 


## Documentación

Este proyecto se centra en centralización de datos demográficos, el comportamiento de los cultivos en Colombia, en base a la producción y rendimiento agrícola en las diferentes zonas geográficas con el principal objetivo de comprender y aprovechar la relación entre estos factores.

## Imágenes

En el contexto del proyecto de Cultivos en Colombia , la sección de imágenes puede contener capturas de pantalla o gráficos que ilustren regiones, municipios de los cultivos Sembrados en Colombia, ejemplos de casos de éxito, imágenes de  zonas o regiones similares de siembra de cultivos, y cualquier otra representación visual que sea relevante para mostrar el progreso y los logros del proyecto.

![Resultados](/Imagenes/K_Means_6_PCA.png)


## Scripts

Para el proyecto de de cultivos en Colombia en un proceso estratégico y fundamental para la optimización de la agricultura en el país , esta sección puede indicar cómo otros profesionales de la agricultura NAcional pueden contribuir a la investigación y análisis. Proporciona información sobre cómo pueden colaborar en la recopilación y análisis de datos, así como en la mejora de los procesos de los cultivos. También destaca cómo los desarrolladores pueden contribuir con scripts y herramientas específicas para el proyecto.

## Bibliografía

[1] Datos oficiales del gobierno colombiano sobre Evaluaciones Agropecuarias Municipales (EVA): Evaluaciones Agropecuarias Municipales (EVA) - Datos.gov.co 

[2] Conjunto de datos y análisis relacionados con los municipios de Colombia disponible en Kaggle: Colombia Municipios en Kaggle 

[3] Datos sobre la relación entre el área cosechada por cultivo y el rendimiento en Colombia: Área Cosechada por Cultivo Vs. Rendimiento - Datos.gov.co 

[4] Información del gobierno colombiano sobre los cultivos con mayor potencial en Colombia: Cultivos con Mayor Potencial en Colombia - agronet.gov.co  

[5] Noticia sobre la importancia de la agricultura sostenible en el bienestar de las sociedades, proporcionada por la Alcaldía de Medellín: La Agricultura Sostenible - Alcaldía de Medellín  

[6] Recurso informativo sobre la diversificación de operaciones agrícolas: Diversification of Your Operation, Why  

[7] Tamene, L., Abera, W., Bendito, E., Erkossa, T., Tariku, M., Sewnet, H.,  Tesfaye, K. (2022). Data-driven similar response units for agricultural technology targeting: An example from Ethiopia. Experimental Agriculture, 58, E27. doi:10.1017/S0014479722000126 

[8] Sánchez-Cuervo, A. M., Aide, T. M., Clark, M. L., & Etter, A. (2012). Land Cover Change in Colombia: Surprising Forest Recovery Trends between 2001 and 2010. PLoS ONE, 7(8). https://doi.org/10.1371/journal.pone.0043943 

[9] Chaves ME, Arango N, editors (1998) Informe Nacional sobre el estado de la Biodiversidad en Colombia 1997. Bogotá, DC, Colombia: Instituto de Investigación de Recursos Biológicos Alexander von Humboldt 

 