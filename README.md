# FriColaB

**Proyecto** de repositorio abierto y colaborativo de iniciativas de emprendimiento con impacto social.

## Características principales

Congruente con algunos principios de la ética hacker, según ha sido enunciada en la obra de **Pekka Himanen**,
*http://es.wikipedia.org/wiki/La_%C3%A9tica_del_hacker_y_el_esp%C3%ADritu_de_la_era_de_la_informaci%C3%B3n*:

*  Conocimiento libre

*  Reconocimiento entre iguales

*  Conciencia social

*  Accesibilidad

## Organización

El modelo de organización de la información similar al del software de control de versiones Git (http://git-scm.com/),
básicamente:

*  Posibilidad de **clonar** el contenido de un repositorio

*  Desarrollo de proyectos derivados usando **bifurcaciones**

*  Distintas líneas de trabajo en paralelo en **ramas**

*  **Publicación** de cambios e **integración** de las novedades

*  **Distribuido** entre los distintos usuarios, con un repositorio de referencia

## Documentación continua integrada

El proceso de documentación es muchas veces el talón de Aquiles de los proyectos, pues la estrategia de documentación
tradicional exige un esfuerzo titánico en los primeros compases, precisamente allí donde las fuerzas,
aunque muy intensas, aún no están enfocadas pues el equipo de trabajo no está lo suficientemente consolidado para
producir contenidos de calidad. Es por ello que la adopción del modelo de **documentación continua** proporciona una mayor eficacia, al producir
un volumen de documentación adecuado a la evolución del proyecto con un esfuerzo mucho menor por parte de los miembros
del equipo de trabajo, pudiendo de esta manera liberar recursos para otras tareas vitales.

![](http://agilemodeling.com/images/lifecycleDocumentationContinuous.jpg)

Sin duda este modelo tradicional está muy relacionado con la dependencia de las fuentes de financiación convencionales,
a saber: entidades financieras e instituciones públicas, que exigen la elaboración de una cantidad ingente de documentación
cuando el proyecto se encuentra todavía en una fase embrionaria, sin ningún prototipo o producto en la mayor parte de
las ocasiones.

Este modelo de **documentación continua** implica que el trabajo de cada una de las partes del equipo se integrará automáticamente en la documentación oficial del proyecto, evitando para ello adaptaciones de formato o requisitos técnicos especiales. Para ello se utilizará un software de generación automática de contenido web que permita mantener la versión principal del documento actualizada si se edita directamente en el servidor principal.

## Arquitectura

A continuación intentaremos definir los distintos nodos del sistema, estableciendo las relaciones entre ellos y apuntando a las posibles funcionalidades a desarrollar.

### Usuario

El usuario será la persona que edita o lee un documento. El usuario podrá trabajar en una copia local del repositorio o en la versión principal almacenada en la plataforma. El usuario manejará distintos lenguajes (idiomas) incluyendo lenguajes de marcas comunes como HTML o Markdown. En la medida de lo posible se evitará la dependencia de lenguajes formales o artificiales complejos.

Lenguajes candidatos: Markdown

### Entorno de trabajo - Front End

El usuario trabajará a través del navegador de internet utilizando un software que le permita editar texto enriquecido en el formato elegido y exportar el resultado al alojamiento remoto.

Software candidato: Prose.io

### Generador de contenido web

El contenido que el usuario cree y edite se convertirá automáticamente a lenguaje web (html), a través de un generador de contenido estático. Es interesante la posibilidad de exportar/importar el contenido desde un repositorio alojado en Github.

Posibles candidatos: Jekyll
