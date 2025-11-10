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

### Objetivos

### Instrucciones de uso

1. Para clonar el proyecto en local, ejecutar el siguiente comando en la consola de su máquina local:
```bash
git clone https://github.com/BeatrizLM/UNIR-Group1-GenomeSequenceAnalysis.git

```
2. Paso 2 imaginario
3. Paso 3 imaginario

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