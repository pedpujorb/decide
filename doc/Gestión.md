# Almacenamiento de votos
## Tabla de contenidos
- [Grupo](#grupo-2)
- [ID del grupo](#id-de-opera-10)
- [Miembros del grupo](#miembros-del-grupo)
- [Enlaces de interés](#enlaces-de-interés)
- [Información del proyecto](#información-del-proyecto)
  * [Resumen](#resumen)
  * [Introducción y contexto](#introducción-y-contexto)
  * [Descripción del sistema](#descripción-del-sistema)
  * [Planificación del proyecto](#planificación-del-proyecto)
  * [Entorno de desarrollo](#entorno-de-desarrollo)
  * [Gestión del cambio, incidencias y depuración](#gestión-del-cambio-incidencias-y-depuración)
  * [Gestión del código fuente](#gestión-del-código-fuente)
    + [Cuándo y cómo realizar un commit](#cuándo-y-cómo-realizar-un-commit)
    + [Usage model](#usage-model)
    + [Ejemplos de uso](#ejemplos-de-uso)
  * [Gestión de la construcción e integración continua](#gestión-de-la-construcción-e-integración-continua)
  * [Gestión de liberaciones, despliegue y entregas](#gestión-de-liberaciones-despliegue-y-entregas)
  * [Mapa de herramientas](#mapa-de-herramientas)
  * [Ejercicio de propuesta de cambio](#ejercicio-de-propuesta-de-cambio)
  * [Conclusiones y trabajo futuro](#conlusiones-y-trabajo-futuro)
## Grupo 2
## ID de Opera: 10
## Miembros del grupo
  * [Díaz de Mayorga Ledesma, Daniel](https://github.com/dandialed): 5
  * [Escobar Aguilera, Jesús Javier](https://github.com/jesescaguUs): 5
  * [Lucas Lozano, Jaime](https://github.com/jailucloz): 5
  * [Pujol Orbello, Pedro](https://github.com/pedpujorb): 5
  * [Viejo Álvarez, Walabonso](https://github.com/walviealv): 5
## Enlaces de interés
## Información del proyecto

### Resumen
El sistema decide es en una plataforma de voto electrónico que consta de varios subsistemas, en nuestro caso el subsistema elegido ha sido el de almacenamiento de votos ya encriptados y debido a que vemos importante mejorar varios campos de este subsistema, se han propuesto 3 cambios o mejoras en él.

### Introducción y contexto
El proyecto consiste en una plataforma educativa de voto electrónico que, por lo tanto, requiere de simplicidad y debe ofrecer diferentes garantía como voto electrónico seguro, la anonimicidad y el voto seguro. Además este sistema consta de varios subsistemas como:
 * Autenticación
 * Censo
 * Votaciones
 * Cabina de votación
 * Almacenamiento de votos (cifrados)
 * Recuento / MixNet
 * Post-procesado
 * Visualización de resultados
 
 En nuestro caso hemos elegido el subsistema **Almacenamiento de votos** que consiste en almacenar los votos en una base de datos en la que se tiene la relación entre votante y voto, aunque no es posible conocer la intención de voto podremos saber quién ha votado y quién no. Para el subsistema elegido también se han elegido algunas mejoras propuestas en este documento.
 
### Descripción del sistema
### Planificación del proyecto
### Entorno de desarrollo
### Gestión del cambio, incidencias y depuración
### Gestión del código fuente
Para la gestión del código de las mejoras que se van a realizar al subsistema se utiliza la herramienta de *git*, que permite al equipo de desarrollo llevar a cabo la gestión de este código mediante la creación de ramas, el mergeo de ellas, la definición de *baselines* etc. Además, el repositorio se alojará en *Github* y tendrán acceso todas las personas del equipo. Actualmente el repositorio del equipo que se encargará del subsistema de almacenamiento es Decide-Io-Almacenamiento, que es un *fork* desde Decide-Io, y a su vez Decide-Io es un *fork* del repositorio original de Decide.

#### Cuándo y cómo realizar un commit
Los *commits* deberán hacerse pronto y con asiduidad aunque de manera que no influya y bloquee a otros usuarios de la misma rama. Es decir, cada vez que se tenga un módulo funcional o un *changeset* deberá hacerse *commit* lo antes posible para que los demás usuarios tengan las posiblidad de estar actualizados. Además, a la hora de poder ver en qué momento se introdujo un error o un cambio es más sencillo si se han hecho de esta manera los *commits*.

Los commits deberán tener la siguiente forma:
```
TÍTULO DEL COMMIT #ISSUE1234 (Código de incidencia si es necesario)
============================

Descripción más detallada de los cambios
```
#### Usage Model
##### Gestión de ramas




Del proyecto base se ha realizado un fork hacia Decido-ío, el grupo general, y desde el grupo general se ha realizado otro fork hacia nuestro subsistema Decide-ío-Almacenamiento.

En el fork del subsistema se abrirán nuevas ramas para cada funcionalidad nueva que se implemente.En el momento en el que se desarrolle una versión estable de una funcionalidad, se podrá mergear la rama develop del subsistema. 

Cuando el subsistema completo sea estable solo los coordinadores podrán subir los cambios a al fork del sistema completo de Decide-ío.

La definición de baselines se realizará con el formato visto en teoría y mediante tags de git.

Los commits contendrán un título indicando brevemente la funcionalidad que se ha implementado y una descripción breve con la información necesaria para comprender estos cambios.

### Gestión de la construcción e integración continua
### Gestión de liberaciones, despliegue y entregas
### Mapa de herramientas
### Ejercicio de propuesta de cambio
### Conclusiones y trabajo futuro
