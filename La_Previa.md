# La previa

## Doce factores

Uno de los primeros fallos que se suelen cometer es usar la tecnología sin entender la metodología para la que fue diseñada.
Por esto, antes de entender Docker, que es la herramienta, es altamente recomendable leer el manifiesto donde se concentra
dicha metodología. [Clica aquí para ver el manifiesto](https://12factor.net/es/)

No recurrir en la medida de lo posible a los doce factores implica fallos de diseño y posibles vulnerabilidades.

En cuanto a la infraestructura como código, se explica sola con el siguiente ejemplo:

    Una empresa da un servicio de hosting.

    Aprovisionar los servidores  (características de las máquinas, configuraciones, accesos... etc) lleva 1 hora por cliente.
    Si se crean plantillas con scripts que hagan ese proceso de forma automática, cada cliente nuevo puede tener su aplicación en 30 minutos.
    Además disminutye la probabilidad de error, dado que hay bastante menos procesos manuales.

## DevOps

Según wikipedia:

    > DevOps (acrónimo inglés de development -desarrollo- y operations -operaciones-) es una práctica de ingeniería de software que tiene como objetivo
    unificar el desarrollo de software (Dev) y la operación del software (Ops). La principal característica del movimiento DevOps es defender enérgicamente
    la automatización y el monitoreo en todos los pasos de la construcción del software, desde la integración, las pruebas, la liberación hasta la implementación
    y la administración de la infraestructura. DevOps apunta a ciclos de desarrollo más cortos, mayor frecuencia de implementación, lanzamientos más confiables,
    en estrecha alineación con los objetivos comerciales

En este esquema se aprecian los ámbitos a los que compete esta "filosofía". [Ver esquema](https://upload.wikimedia.org/wikipedia/commons/b/b5/Devops.svg)

¿Tiene sentido esto? Evidentemente DevOps no se ajusta a todos los casos.

Casos donde DevOps carece de sentido:

    * Infraestructura y aplicaciones con grado de complejidad mínimo. Por ejemplo una web que sólo sirve html con 4 visitas al día.

    * Infraestructura y apliciones obsoletas. Es abusrdo utilizar metodologías distintas cuando ni la infraestructura ni la aplicación está
    preparada para ello, por ejemplo sistemas en producción de un banco que están en activo desde 1980.