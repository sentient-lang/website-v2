---
title: "Language specification: Invariant"
header: /specification
layout: default
---
# Invariant

An invariant specifies something that must always be **true** when the program
runs. Invariants let you to define the constraints of your problem domain. Here
is an example:

```ruby
invariant a + b + c == 10;
```

When this program runs, it will only produce outputs such that the total of
variables **a**, **b** and **c** is equal to 10. You can define any number of
invariants throughout your program and it is possible to define multiple
invariants on the same line:

```ruby
invariant a > 0, b > 0, c > 0;
```