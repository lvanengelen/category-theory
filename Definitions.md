# Definitions

## Set
The category of all sets with functions as morphisms.

## Hask
The category of all sets where each include *bottom*, the return value of a no -terminating function
(Set + bottom)

## Void
Type corresponding with the empty set.

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
