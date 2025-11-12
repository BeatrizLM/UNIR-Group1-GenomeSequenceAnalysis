# GitHub: Crear un repositorio y control de versiones

## Asignatura: Introducción a la programación científica

### Integrantes del Grupo
- Ana Padilla Campos — [@anapac00](https://github.com/anapac00)
- Antonio Jesús Gil Galisteo — [@Antoniogilgalis](https://github.com/Antoniogilgalis)
- Beatriz Esquivel Carrera — [@BeaEsca](https://github.com/BeaEsca)
- Eva García Valero — [@egarciaval](https://github.com/egarciaval)
- Beatriz López Martínez — [@BeatrizLM](https://github.com/beatrizlopez)



## Índice
- [Descripción](#-descripcion)
- [Flujo de trabajo para la actividad](#-flujo-de-trabajo-para-la-actividad)

---

## Descripción

### Propósito y estructura

El proyecto genome sequence analysis pretende comparar los resultados de una secuenciación con secuencias modelo. Se ha estructurado según los diferentes pasos de los que se compone un análisis genético:

- En primer lugar, se han obtenido los genomas crudos tras la secuenciación. Dichas secuencias se encuentran almacenadas en la carpeta *sequences*.
- A continuación, tras limpiar las secuencias obtenidas, se ha realizado un análisis comparativo entre ellas, contenido en *validation methods*.
- Tras la comparación, se ha obtenido una secuencia final, ubicada en *data-results*.
- Finalmente, por medio de diferentes herramientas de comparación genética, se ha realizado el alineamiento de nuestra secuencia para conocer la similitud con otros organismos. Los resultados de este análisis se han recogido en la carpeta *comparative-analysis*.

### Objetivos

Teniendo en cuenta el apartado anterior, se pueden diferenciar múltiples objetivos:

1. Creación de un repositorio github para facilitar el trabajo del grupo.
2. Manipulación de secuencias genéticas.
3. Uso de herramientas bioinformáticas que permiten tanto el procesado, como el alineamiento y la comparación de las secuencias.
4. Interpretación de los resultados obtenidos tras la comparación. 
5. Elaboración de una memoria que refleje todo el proceso.

### Instrucciones de uso

1. Para clonar el proyecto en local, ejecutar el siguiente comando en la consola de su máquina local:
```bash
git clone https://github.com/BeatrizLM/UNIR-Group1-GenomeSequenceAnalysis.git

```
2. Crear una rama sobre la que trabajar. Cada integrante del equipo trabaja una parte del proyecto en una rama diferente.
3. Todos los cambios realizados en local se integran al proyecto mediante *commit* y *push*.
4. Para fusionar todas las ramas y unificar el proyecto, hacer pull request de la rama en la que se ha trabajado hacia main. El director del proyecto supervisa los cambios que esto supone para aprobar o denegar la petición.

## Flujo de trabajo para la actividad

El propósito de este apartado es explicar cómo se ha llevado a cabo la distribución de trabajo en la práctica. Tal y como se ha comentado en el apartado anterior, se ha seguido la estructura de un proyecto de análisis genómico. Para facilitar la participación de todos los integrantes del grupo, la división de las tareas se ha hecho en dos fases; una primera fase de construcción y creación del proyecto base, y una segunda fase de documentación del trabajo en el fichero *README.md*.

En la primera fase, cuatro de los integrantes han creado una rama, una por *etapa* del proyecto, mientras que el quinto se ha encargado de crear el repositorio y administrar las ramas y acepta los *pull request*. En vista a practicar de cara a un uso real del repositorio en local, se ha utilizado el IDE de desarrollo **VisualStudioCode**, tando para manipular el proyecto, como para usar *git* (desde la terminal y desde la interfaz). En esta fase, se han probado los siguientes escenarios:

1. Trabajo independiente en una rama y subida directa a la rama principal. Esto se ha hecho en las ramas *pretreatment* y *Final_Analysis*.
2. Trabajo en una rama con pull request sobre otra rama y posterior subida a la principal (*data-analysis* y *results*).

En la siguiente imagen se puede ver el flujo de *git* mediente un gráfico. Como se puede apreciar, se han ido aceptando los *pull request* en la rama *main* siguiendo el orden de trabajo del proyecto. 

![Flujo de la primera fase del proyecto. Construcción de un proyecto de análisis de secuenciación genómica](./readme-img/first-step-snapshot.png)

Como se ha comentado, la segunda fase ha consistido en la coordinación de redacción del archivo *README.md*. Esta fase ha implicado:

1. La creación de una rama a partir de *main* para trabajar exclusivamente sobre el fichero (*readme_changes*).
2. Cara integrante ha trabajado sobre una subrama de esta para anotar lo realizado en la primera fase.
3. Fusionar esas ramas en *readme_changes* para poder trabajar con toda la información aportada por cada persona y de esta manera conseguir un documento explicativo completo.
4. Como la rama *readme_changes* se obtuvo de forma paralela al resto de ramas, la integración de este fichero con *main* deberá hacerse con un *git checkout*.

Durante esta fase ha habido más movimiento en las ramas debido a la necesidad de resolver conflictos, llegando a tener que ejecutar acciones como *git reset --hard* para solucionar los problemas. Estos inconvenientes han sido bastante útiles para poder visualizar los problemas diarios que pueden surgir de utilizar *git* como herramienta de control de versiones. Asimismo, se han seguido sacando ramas independientes de *main* de cara a limpiar y estandarizar el proyecto, así como para seguir practicando.

Posteriormente a las fases mencionada se creó una nueva rama *RNA_sample_03_Nov_2025_V2* a partir de *readme_changes*, con el fin de analizar y comparar nuevas secuencias encontradas. Para ello se añadieron nuevos ficheros a la carpeta sequences y se actualizaron los ficheros de las carpetas validation-methods y data-results, con el fin de simular un segundo analisis en el proyecto. Además, se creo un *tag* llamado *Second-Sampling_V2* para marcar el estado del proyecto tras este segundo análisis.
