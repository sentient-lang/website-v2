---
title: "Language syntax: Conditional"
header: /syntax
layout: default
---
# Conditional

Sentient supports conditionals as expressions. Both the consequent and alternate
must be provided and both branches will be evaluated, regardless of the return
value of the conditional. Here's an example:

```sentient
a = if(someCondition, valueIfTrue, valueIfFalse);
```

This can be equivalently written as:

```sentient
a = someCondition.if(valueIfTrue, valueIfFalse);
```

Or using a ternary form:

```sentient
a = someCondition ? valueIfTrue : valueIfFalse;
```

See [boolean](../library/boolean) for more information.
