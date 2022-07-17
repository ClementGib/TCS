#Go Cheat Sheet <img align="center" width="80" height="80" src="https://go.dev/blog/go-brand/Go-Logo/SVG/Go-Logo_Aqua.svg" alt="Go icon">

# Languages
[English](#english-)
[Français](#français-)



## English 🇬🇧🇺🇸

# Contents
1. [Introduction](#introduction)
2. [Hello world](#hello-world)
3. [Declarations](#declarations)
4. [Operators](#operators)
    * [Arithmetic](#arithmetic)
    * [Relational](#relational)
    * [Logical](#logical)
    * [Other](#other)

### Introduction
* Imperative language
* Statically typed (Type defined at the compilation phase)
* Compiles to native code (no JVM)
* Functions are first class citizens (pass as argument, return and store function)
* Functions can return multiple values
* No classes, but structs with methods
* Interfaces
* No implementation inheritance. There's type embedding, though.
* Has closures
* Pointers, but not pointer arithmetic
* Built-in concurrency primitives: Goroutines and Channels

### Hello World
The program starts running in the `main` package, this is why we need to declare the `main` package.
Every package has an export name, the name is exported if it starts with capitale letter. We can import a package with the key-word `import` followed by the package name.
`fmt` is used to generate output.
```go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```

### Declarations

Varaible declarations:
```go
// create i variable
var i int

// create and init x variable
var x int = 8

// multiple creations and initiations of variables
var a, b, c int = 8, 16, 42
/* a equals 8
   b equals 16
   c equals 42 */

// short variable init
variable := 10

// short multiple variables init
variable1, variable2 := 10, 5

```

### Operators



<br>
<br>


## Français 🇫🇷

# Contents
1. [Introduction](#introduction)
2. [Hello world](#hello-world)
3. [Déclarations](#déclarations)
4. [Opérateurs](#opérateurs)
    * [Arithmetic](#arithmetic)
    * [Relational](#relational)
    * [Logical](#logical)
    * [Other](#other)

### Introduction

* Langage impératif
* Typage statique (Type défini à la compilation)
* Compilation depuis du code natif (pas de JVM)
* Functions sont "first class citizens" (permet de passer en tant qu'argument, retourne et stoque des fonctions)
* Functions peuvent retourner plusieurs valeurs
* Pas de classes, mais des strucs avec des méthodes
* Interfaces
* Pas d'implémentation d'héritage, il y a toutefois de l'intégration de types
* A des Fermetures/Clôtures
* Pointeurs, mais pas de pointeurs arithmetic
* Primitives concurrentes intégrées: Goroutines et Channels

### Hello World

Le programme démarre dans le package `main`, il faut donc déclarer un package `main`.
Chaque package à un nom d'export pour y accéder, un nom est est exporté si il à une lettre capitale. On peut importer un package avec le mot clé `import` suivi du nom du package.
`fmt` permet de générer des sorties.

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```

### Declarations

Varaible declarations:
```go
// créer variable i
var i int

// crée et init variable x
var x int = 8

// création multiple et initiation de variables
var a, b, c int = 8, 16, 42
/* a equals 8
   b equals 16
   c equals 42 */

// initialisation de variable rapide
variable := 10

// initialisation de variable rapide et multiple
variable1, variable2 := 10, 5

```

### Operators