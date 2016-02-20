# Definitions

## Set
The category of all sets with functions as morphisms.

## Hask
The category of all sets where each include *bottom*, the return value of a no -terminating function
(Set + bottom)

## Void
Type corresponding with the empty set.

## absurd
The functions with `Void` as their input type.

## Unit
Type corresponding with the singleton set, containing only ().

## Reflexive
Binary relation `R` where `(a, a) in R for all a`

## Transitive
Binary relation `R` where `(a, b) in R and (b, c) in R then (a, c) in R`

## Anti-symmetric
Binary relation `R` where `(a, b) in R and (b, a) in R then a = b`

## Total
Binary relation `R` where `(a, b) in R or (b, a)`

## Commutatieve
Binary operation `•` where `a • b = b • a`

## Associative
Binary operation `•` where `a • (b • c) = (a •b) • c`

## Distributive
Binary operations `•` and `+` where `a • (b + c) = a•b + a•c`

## Preorder
Binary relation that is [transitive](#transitive) and [reflexive](#reflexive).  Can be drawn as a
directed graph.

Example: reachability between locations.

## Partial Order
Binary relation that is [transitive](#transitive), [reflexive](#reflexive) and
[anti-symmetric](#anti-reflexive) ([preorder](#preorder) + [anti-symmetry](#anti-symmetry)).  Can be
drawn as a directed acyclic graph.

Example: ancestry between individuals, commits.

## Total Order
Binary relation that is [transitive](#transitive), [reflexive](#reflexive),
[anti-symmetric](anti-symmetric) and [total](#total) ([partial order](#partial-order) +
[totality](#total)).  Can be drawn as a directed acyclic graph with an edge between every two nodes.

Example: <= on the set of real numbers.

## Partially ordered set (poset)
A set with a [partial order](#partial-order).

## Monoid
Set with an [associative](#associative) binary operation `•` and a unit element `0` for which
`a • 0 = 0 • a = a`

Example: addition, string concatenation

## Universal Construction
Defining objects in terms of their relationships.

Example: initial and terminal objects.

## Initial Object
Object with one and only one morphism going to any object.

Does not have to exist, but if it exits it is unique up to
[unique isomorphism](uniqueness-up-to-unique-isomorphism).

Example: least element of a poset, `Void` in `Set`, set of all integers does not have an initial
object, `Unit` is not an initial object in `Set`.

## Terminal Object
Object with one and only one morphism coming from any object.

Does not have to exist, but if it exists it is unique up to
[unique isomorphism](uniqueness-up-to-unique-isomorphism).

Example: biggest element in a poset, `Unit` in `Set`.

## Isomorphism
An invertible morphism; a pair of morphisms which are each other's inverses:
`f • g = g • f = id`.

## Uniqueness up to isomorphism
Uniqueness where unique objects have [isomorphisms](#isomorphism) between each pair of them.

## Uniqueness up to unique isomorphism
Uniqueness up to isomorphism where there is only a single [isomorphism](#isomorphism) between each
pair of them.

## Opposite category (C^op)
Category derived from `C` with all morphisms reversed.

## Surjective (onto)
Function whose image is equal to its codomain.

Example: f: R -> R+ f(x) = x^2, not g: R -> R g(x) = x^2

## Injective (one-to-one)
Function that does not map more than one input to the same output, e.g. it is non-collapsing.

Example: f: R -> R f(x) = x, not g: R -> R f(x) = x^2

## Bijective
Function that is both [surjective](#surjective-onto) and [injective](#injective-one-to-one) and
therefore symmetric and invertible.
