# Entornos de Desarrollo 2023-2024
Repositorio del módulo Entornos de Desarrollo

https://aulavirtual3.educa.madrid.org/ies.alonsodeavellan.alcala/course/view.php?id=932

![image](https://github.com/profeMelola/EntornosDesarrollo2023_24/assets/91023374/a79b1de8-619a-4151-a9a1-3daa0779d773)

## Trabajar con Git de forma colaborativa

Git es una excelente herramienta para desarrollar de forma individual y colaborativa.

Supongamos que estás trabajando en un proyecto y quieres agregar una nueva funcionalidad. La forma correcta es creando una branch o rama con el nombre de la nueva funcionalidad donde agregaremos nuestros cambios.

Por defecto cuando creamos un repositorio tiene una rama llamada master. (Como buena practica nada se desarrolla en master). Utilizamos ramas para experimentar y hacer cambios.

**Branching o ramificación** es la manera de trabajar en diferentes versiones de un repositorio a la vez.

### Comandos Git sobre ramas
```
git branch [nombre de la rama]
crea una nueva rama

git branch
enlista todas las ramas en el repositorio actual

git branch -d [nombre de la rama]
borra la rama especificada

git checkout [nombre de la rama]
cambia a la rama especificada


git merge[nombre de la rama]
combina el historial de la rama especificada con la rama actual

```

Una vez que hayas probado la nueva funcionalidad y comprobado que cumple el objetivo; estamos listas para mover ese desarrollo a la rama master. Es decir, necesitamos hacer un **merge.**

Algunas veces, cuando queremos fusionar dos ramas no resulta tan bien, podemos generar un conflicto.

### Conflictos
Un conflicto en git se produce cuando se edita la misma linea de código en dos instancias distintas de trabajo y luego se intentan fusionar.

Git no puede decidir cual versión elegir y te avisa que tu debes resolverlo; nos proporciona una ayuda diciéndonos que archivo tiene el conflicto, el cual al abrirlo en nuestro editor, nos muestra cuales son los cambios que entran en conflicto.

Tenemos que elegir entre lo que está entre <<<<<<< HEAD y ======= que es contenido que tenemos en la rama donde estamos haciendo el merge o entre ======= y >>>>>>> contenido donde están los cambios hechos en la rama que queremos unir.

Arreglamos los cambios elegidos, guardamos, agregamos y hacemos commit de los cambios. De esta manera resolvemos el conflicto y logramos hacer merge con éxito.

### Colaborar en otros proyectos
Otra ventaja de trabajar con git es que podemos colaborar en otro proyectos.

Algunos conceptos que debes saber son:

- **Fork:** hace una copia exacta de un repositorio ; creando un nuevo en tu cuenta de Github con una url diferente que podemos utilizar como un repositorio git cualquiera. Tendremos dos repositorios independientes y cada uno evoluciona de forma autónoma.
- **Pull request:** es una petición que el propietario de un fork de un repositorio hace al propietario del repositorio original para que este último incorpore los commits que están en el fork.

Los pasos a seguir para trabajar de forma colaborativa son:

1. Hacer fork desde la interfaz de github del proyecto en el cual queremos colaborar.
2. Se clona el repositorio creado.
3. Crear una nueva branch para desarrollar nuestra aportación.
4. Realizar commits para describir las modificaciones y/o aportaciones.
5. Se hace push de las modificaciones en nuestra copia del repositorio.
6. Se pide un pull request desde la interfaz de github.

Puedes practicar siguiendo esta guia: https://docs.github.com/es/get-started/quickstart/hello-world?source=post_page-----62dea67aa2eb--------------------------------

<sub>Referencia: https://medium.com/laboratoria-how-to/t%C3%BA-y-yo-usando-git-colaborativo-no-se-pi%C3%A9nsalo-62dea67aa2eb</sub>
