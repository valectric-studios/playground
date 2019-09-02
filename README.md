![Playground Banner](.docs/images/playground-banner.png)

<p align="center">
<img src="https://img.shields.io/badge/java-11-lightgray.svg?style=flat-square&logo=java">
<img src="https://img.shields.io/badge/spigot-1.14.x-yellow.svg?style=flat-square">
<img src="https://img.shields.io/badge/nms-not%20in%20use-brightgreen.svg?style=flat-square">
</p>

## Table of Contents
* [Adding Playground to your build](#adding-playground-to-your-build)
   * [As Maven dependency](#as-maven-dependency)
   * [As Gradle dependency](#as-gradle-dependency)
   * [As SBT dependency](#as-sbt-dependency)
* [Build your own Playground](#build-your-own-playground)
* [Learn about Playground](#learn-about-playground)
* [Versioning](#versioning)
* [Dependencies](#dependencies)
* [Authors](#authors)
* [Credits](#credits)

## Adding Playground to your build
### As Maven dependency 
To add Playground as dependency using Maven, use the following:
```xml
<dependencies>
  <dependency>
    <groupId>net.valectric.playground</groupId>
    <artifactId>playground</artifactId>
    <version>1.14.3-SNAPSHOT</version>
  </dependency>
</dependencies>
```

### As Gradle dependency
To add Playground as dependency using Gradle, use the following:
```groovy
dependencies {
  compile 'net.valectric.playground:playground:1.14.3-SNAPSHOT'
  compile group: 'net.valectric.playground', name: 'playground', version: '1.14.3-SNAPSHOT'
}
```

### As SBT dependency
To add Playground as dependency using SBT, use the following:
```
libraryDependencies += "net.valectric.playground" % "playground" % "1.14.3-SNAPSHOT"
```

## Build your own Playground
#### TL;DR - Chained commands to clone, change directory and build Playground
<details>
  <summary>Unix</summary>
  
```bash
# HTTPS
git clone https://github.com/valectric-studios/playground && cd playground && ./mvnw install
# SSH
git clone git@github.com:valectric-studios/playground.git && cd playground && ./mvnw install
```
</details>
<details>
  <summary>PowerShell</summary>
  
```bash
# HTTPS
git clone https://github.com/valectric-studios/playground; cd playground; ./mvnw install
# SSH
git clone git@github.com:valectric-studios/playground.git; cd playground; ./mvnw install
```
</details>
<details>
  <summary>Windows Cmd</summary>
  
```bash
# HTTPS
git clone https://github.com/valectric-studios/playground && cd playground && mvnw install
# SSH
git clone git@github.com:valectric-studios/playground.git; cd playground; ./mvnw install
```
</details>

Building your own Playground is pretty much straightforward. Playground uses Maven for dependency management and for building the jar file. Playground does not have any extra procedures, any extra settings or conditions you need to care about. You pull this bad boy, open up your terminal and execute the Maven build.

## Learn about Playground
Playground introduces a myriad of new features, abstractions and possible ways to implement your favorite idea a lot more easily. We cannot cover all of Playground's features in here, so if you would like to learn what Playground can do and what it cannot do for you, or if you want to learn about its features, then head over to Playground's [wiki](https://github.com/valectric-studios/playground/wiki).

## Versioning
We use the same versioning scheme as Spigot does. A Playground build compatible with e.g. Spigot 1.14.3 will be labeled as "playground-1.14.3-(SNAPSHOT/RELEASE).jar". For the versions available, see the [tags on this repository](https://github.com/valectric-studios/playground/tags). 

Older Playground versions **are not** being supplied with new features once the core team decided to work on a new version. Older versions, if required, will only receive bug fixes and performance improvements. If someone desires to have new features in older versions, feel free to open up an issue, implement the feature in a fork and create a pull request.

## Dependencies
Here are all of our dependencies listed which are used in Playground. The dependency's name will take you to the dependency's project page. The _"artifact id"_ will take you to the dependency's index on the [MVNRepository website](https://mvnrepository.com). If the dependency is not available on the [MVNRepository website](https://mvnrepository.com) then there will be a link to its repository.

- [Spigot API](https://spigotmc.org) ([org.spigotmc:spigot-api:1.14.3-R0.1-SNAPSHOT](https://hub.spigotmc.org/nexus/content/repositories/snapshots/org/spigotmc/spigot-api))
- [Trove](https://bitbucket.org/trove4j/trove) ([net.sf.trove4j:trove4j:jar:3.0.3](https://mvnrepository.com/artifact/net.sf.trove4j/trove4j/3.0.3))
- [SpotBugs](https://spotbugs.github.io) ([com.github.spotbugs:spotbugs:3.1.12](https://mvnrepository.com/artifact/com.github.spotbugs/spotbugs/3.1.12))

## Credits
- "Playground" is heavily inspired by Google's [Guava](https://github.com/google/guava) library
- Badges provided by [shields.io](https://shields.io/) ([GitHub vendor](https://github.com/badges/shields))
