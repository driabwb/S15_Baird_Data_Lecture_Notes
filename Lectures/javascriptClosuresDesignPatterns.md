# Javascript

* scope
* closures prototypes

## Scope
* Where to look for things
* func define scope

### Hoisting
* prior to execution javascript move all var decl to the top of the scope

## Closure

## Modules
* angualr services
* Module pattern base on closure
* use scope to name private data
* func to create obj and return an obj with public API

## Class vs Prototype
* no notion of class
* prototypes use delegation

## this
* bound at runtime and determined by how it is called
* 4 ways
  1. new
     * this refers to the obj it returns
  2. explicit
     * using call the arg is bound as this
     * the obj func called on is providing the func
  3. Implicit
     * this is bound to the obj it was called on
  4. Default
     * this becomes the current scope