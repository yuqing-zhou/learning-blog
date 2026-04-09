---
layout: post
title: "Python: List Comprehensions"
date: 2026-04-08
categories: python
---

List comprehensions are a concise way to create lists in Python.

## Basic syntax

```python
squares = [x ** 2 for x in range(10)]
```

## With a condition

```python
evens = [x for x in range(20) if x % 2 == 0]
```

## Nested

```python
pairs = [(x, y) for x in range(3) for y in range(3) if x != y]
```

They're faster than an equivalent `for` loop for simple transformations because the iteration happens at the C level inside Python.
