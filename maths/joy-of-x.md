# The Joy of X: A Guided Tour of Math, from One to Infinity

By Steven Strogatz (2012)

> The physicist Murray Gell-Mann came to a similar realization one day when he was worrying about his future. As an undergraduate at Yale, he desperately wanted to stay in the Ivy League for graduate school. Unfortunately Princeton rejected his application. Harvard said yes but seemed to be dragging its feet about providing the financial support he needed. His best option, though he found it depressing, was MIT. In Gell-Mann’s eyes, MIT was a grubby technological institute, beneath his rarefied taste. Nevertheless, he accepted the offer. Years later he would explain that he had contemplated suicide at the time but decided against it once he realized that attending MIT and killing himself didn’t commute. He could always go to MIT and commit suicide later if he had to, but not the other way around.

## My Notes

> We perceive pitch logarithmically. In every place where they arise, from the Richter scale for earthquake magnitudes to pH measures of acidity, logarithms make wonderful compressors. They’re ideal for taking quantities that vary over a wide range and squeezing them together so they become more manageable.

> Things that seem hopelessly random and unpredictable when viewed in isolation often turn out to be lawful and predictable when viewed in aggregate.

> The normal distribution can be proven to arise whenever a large number of mildly random effects of similar size, all acting independently, are added together.

### Perfect Squares

Adding all the consecutive odd numbers gives the sequence of perfect squares:

```
1 + 3 = 4
1 + 3 + 5 = 9
1 + 3 + 5 + 7 = 16
1 + 3 + 5 + 7 + 9 = 25
1 + 3 + 5 + 7 + 9 + 11 = 49
```

More pictorally, adding the next odd number creates a new square:

```
X

X O
O O

X O X
O O X
X X X

X O X O
O O X O
X X X O
O O O O
```

### Area of a Circle

Proof:

![](https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/CircleArea.svg/220px-CircleArea.svg.png)

### Quadratic equations

Given:

```
x² + 10x = 39
```

Draw:

```
     x       5
   ┌───┬────────────┐
 x │   │            │       ┌────────────┐
   ├───┼────────────┘       │            │
   │   │                    │            │
   │   │                =   │     39     │
 5 │   │                    │            │
   │   │                    │            │
   │   │                    └────────────┘
   └───┘
```

Fil in the gap:

```
     x       5
   ┌───┬────────────┐
 x │   │            │       ┌────────────┐   ┌────────────┐
   ├───┼────────────┤       │            │   │            │
   │   │            │       │            │   │            │
   │   │            │   =   │     39     │ + │     25     │
 5 │   │     25     │       │            │   │            │
   │   │            │       │            │   │            │
   │   │            │       └────────────┘   └────────────┘
   └───┴────────────┘
```

Now:

```
(x + 5)² = 64
x + 5 = 8
x = 3
```