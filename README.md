<h1 style="font-size: 3em;">CVDS-LAB03</h1>

<h2 style="font-size: 3em;">Integrantes:</h2>

Erick Santiago Montero Sutachán

Ricardo Andrés Villamizar Méndez

<h2 style="font-size: 3em;">Ejercicio "Registraduría":</h2>

***Introducción***

La intención de este ejercicio es la creación de un proyecto en maven con el cual porder ser la base para un proceso de
registraduría con el cuál registrar personas que tienen la intención de votar para las próximas elecciones, pudiendo
generar certifiacdos para aquellas personas que registren correctamente su voto.

***Requerimientos***
- Solo se registrarán votantes válidos
- Solo se permite una inscripción por número de documento

***Creación del proyecto***


```{bash}
mvn archetype:generate -Dfilter=maven-archetype-quickstart
```

Esto nos generará un proyecto de manera interactiva, lo que después nos solicitará:

```{bash}
Grupo (groupId): edu.eci.cvds
Artefacto (artifactId): ClasesEquivalencia
Paquete (package): edu.eci.cvds.tdd
archetypeArtifactId: maven-archetype-quickstart
```

