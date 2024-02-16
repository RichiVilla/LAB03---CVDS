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

<h3 style="font-size: 3em;">Creación del proyecto con Maven:</h3>

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
![image](https://github.com/RichiVilla/LAB03---CVDS/assets/124943246/d50ba9bb-6f4b-425d-af1f-54f5d40ba69b)
![image](https://github.com/RichiVilla/LAB03---CVDS/assets/124943246/e6c5b0d2-a4d7-4021-a00a-a964b1c65111)

<h3 style="font-size: 3em;">Ajustar configuraciones del proyecto</h3>

Modificamos el POM para que contenga:
- La dependencia copiada a la sección de dependencias de JUnit.
- La versión delcompilador de Java a la versión 8

```{bash}
<properties>
<maven.compiler.target>1.8</maven.compiler.target>
<maven.compiler.source>1.8</maven.compiler.source>
</properties>
```
![image](https://github.com/RichiVilla/LAB03---CVDS/assets/124943246/f5e5fa3a-7134-4f16-b0e7-b3e32a2551f0)

<h3 style="font-size: 3em;">Compilar y ejecutar</h3>
 
Compilamos el proyecto con: 

```{bash}
$ mvn package
```
![image](https://github.com/RichiVilla/LAB03---CVDS/assets/124943246/516ddd94-fa5f-45ad-8cb7-17cbb1c87dfd)

<h3 style="font-size: 3em;">Esqueleto de la aplicación</h3>

Creamos la carpeta de registry en su directorio correspondiente:

![image](https://github.com/RichiVilla/LAB03---CVDS/assets/124943246/60b89dea-dca4-410f-bdaa-86c258cc8e3a)

Y las clases correspondientes de java:

![image](https://github.com/RichiVilla/LAB03---CVDS/assets/124943246/17d8ce32-3e2b-479c-b606-810782076f89)

A su vez, en el siguiente directorio creamos una clase de Test:
![image](https://github.com/RichiVilla/LAB03---CVDS/assets/124943246/0389a072-081e-4d9c-95bf-d165997d58c7)

![image](https://github.com/RichiVilla/LAB03---CVDS/assets/124943246/797316ca-83c3-4aad-9713-790dfc20971e)

<h3 style="font-size: 3em;">Ejecutar las pruebas</h3>
Creamos las pruebas en la última clase que creamos de Test:

![image](https://github.com/RichiVilla/LAB03---CVDS/assets/124943246/8c89b754-0f51-49ff-aa87-d3bced8d436c)

Y luego las ejecutamos para comprobar que estén bien

```{bash}
$ mvn test
```
![image](https://github.com/RichiVilla/LAB03---CVDS/assets/124943246/75196522-b3a9-4cd5-a74d-d06a6fef1382)

<h2 style="font-size: 3em;">Ejercicio "Descuento de tarifas":</h2>
