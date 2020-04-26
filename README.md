The repository contains solutions and examples for the exercises from the book described below.\
If you want to run the project locally, it can be done easily because it was developed on Docker.

## Java - A Beginner's Guide
#### Seventh Edition

Create, Compile, and Run Java Programs Today\
Herbert Schildt\
Oracle Press

![Java - A Beginner's Guide Herbert Schildt](./java-beginners-guide.jpg)
## Technical prerequisites
- Unix-based OS
- Git
- Docker

## Getting started
Run the commands one by one:
```shell
git clone https://github.com/pavel-rossinsky/java-a-beginners-guide-herbert-schildt.git
cd java-a-beginners-guide-herbert-schildt
mkdir jvm-sources .m2
cp ./docker/builds/jdk/etc/env-example .env
# Open the .env file and set the right path to the project on your OS
# for example /users/you_user_name/Documents/repository/java-a-beginners-guide-herbert-schildt
docker-compose build
```
## How to compile
```
docker-compose run jdk mvn compile
```
Repeat this command after editing any *.java files
## How to run a class
Find a class that is of your interest and copy its fully-qualified name, then run:
```shell
docker-compose run jdk mvn exec:java -Dexec.mainClass={fully_qualified_class_name}
```
For instance:
```shell
docker-compose run jdk mvn exec:java -Dexec.mainClass=com.guide.c1.Example
docker-compose run jdk mvn exec:java -Dexec.mainClass=com.guide.c1.GalToLitTable
```
## How to uninstall the project
```shell script
docker-compose down -v
```

## Finished chapters

# | Chapter | Status
--- | --- | ---
1 | [Java Fundamentals](./src/main/java/com/guide/c1) | :ballot_box_with_check:
2 | [Introducing Data Types and Operators](./src/main/java/com/guide/c2) | :ballot_box_with_check:
3 | [Program Control Statements](./src/main/java/com/guide/c3) | :hourglass_flowing_sand:
4 | [Introducing Classes, Objects, and Methods](./src/main/java/com/guide/c4) | :coffee:
5 | [More Data Types and Operators](./src/main/java/com/guide/c5) | :coffee:
6 | [A Closer Look at Methods and Classes](./src/main/java/com/guide/c6) | :coffee:
7 | [Inheritance](./src/main/java/com/guide/c3) | :coffee:
8 | [Packages and Interfaces](./src/main/java/com/guide/c3) | :coffee:
9 | [Exception Handling](./src/main/java/com/guide/c3) | :coffee:
10 | [Using I/O](./src/main/java/com/guide/c3) | :coffee:
11 | [Multithreaded Programming](./src/main/java/com/guide/c3) | :coffee:
12 | [Enumerations, Autoboxing, Static Import, and Annotations](./src/main/java/com/guide/c3) | :coffee:
13 | [Generics](./src/main/java/com/guide/c3) | :coffee:
14 | [Lambda Expressions and Method References](./src/main/java/com/guide/c3) | :coffee:
15 | [Modules](./src/main/java/com/guide/c3) | :coffee:
16 | [Introducing Swing](./src/main/java/com/guide/c3) | :coffee:
17 | [Introducing JavaFX](./src/main/java/com/guide/c3) | :coffee:
D | [Introducing JShell](./src/main/java/com/guide/c3) | :coffee:

