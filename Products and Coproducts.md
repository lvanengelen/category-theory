# Products and Coproducts

In category theory, objects and morphisms are opaque: you can only identify a specifc object by
describing its relations to other objects defined by its morphisms.

A universal construction is one way to define objects in terms of their morphisms.  Universal
constructions are built by finding objects matching certain patterns and ranking the results against
each other.

## Initial and Terminal Objects

In `Set`, `Void` is the initial object and `Unit` the terminal object.  In this last case, the
uniqueness of the morphism is important, because there are lots of morphisms from all objects to a
single one (e.g. two from any object to `Bool`).

A terminal object in `C` is the initial object in its
[opposite category](Definitions.md#opposite-category-cop).

## Product

A product is modeled after the cartesian products of sets.  It is an object with projection
morphisms to its constituent objects.

A product candidate `c` is better than a product candidate `c'` if the projections `p'` and `q'` of
`c'` can be derived from the projections `p` and `q` of `c` together with `m`:

```
p' = p • m
q' = q • m
```

Because of this, `m` is said to *factorize* `p'` and `q'`.

## Coproduct

The coproduct is the *dual* of the product.  It has incoming morphisms from its constituents
objects.

A coproduct candidate `c` is better than a coproduct candidate `c'` if the injections `i'` and `j'`
of `c'` can be derived from the injections `i` and `j` of `c` together with `m`:

```
i' = m • i
j' = m • j
```

Here, `m` factorizes `i'` and `j'`.
