# Typed Interpreters

In this section we will add a type system to our interpreters. We could implement a type checking algorithm on our untyped AST, but instead we'll see how we can re-use Scala's type system via a technique known as *generalised algebraic data types*. With generalised algebraic data types we can implement *simply typed* languages. This means a type system that is roughly equivalent to Scala programs without type variables (type variables are also known as generic types or parametric polymorphism.) Just as we saw that HOAS reduced the complexity of our programs, we'll see that our typed interpreters are much simpler than our untyped ones.