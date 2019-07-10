# Clean Code: A Handbook of Agile Software Craftsmanship

By Robert C Martin (2008)

> If we all checked-in our code a little cleaner than when we checked it out, the code simply could not rot.

> It is a myth that we can get systems “right the first time.” Instead, we should implement only today’s stories, then refactor and expand the system to implement new stories tomorrow.

## My Notes

### Naming

> It is not at all uncommon that hunting for a good name results in a favorable restructuring of the code.

#### Use Searchable Names

A literal `5` in a bit of code related to weekdays may not be alarming, but a searchable name is better.

#### Avoid Mental Mapping

As an author, `k` (for key in an associative array), and `v` (for the value) are immediately obvious. But we can be kinder to others and our future selves with descriptive terms (e.g., `userID` and `userObject`).

#### Be Specific

Instead of:

```java
public updateCoordinate(int x, int y) {
    this.x = x;
    this.y = y;
}
```

… use:

```java
public updateCoordinate(int newX, int newY) {
    x = newX;
    y = newY;
}
```

… because `newX` and `newY` represent something different to `x` and `y`. Explain that difference.

### Functions

#### Functions Should Tell a Story

> We want the code to read like a top-down narrative. We want every function to be followed by those at the next level of abstraction so that we can read the program, descending one level of abstraction at a time as we read down the list of functions.

#### Avoid Temporal Coupling

E.g., this function can only be called **after** this other one.

- Add a parameter to the second function that is calculated by the first `b(a())`
- Or encapsulate the work of `a()` and `b()` in the same function

#### Avoid Side-Effects

> If your function must change the state of something, have it change the state of its owning object.

### Comments

💡 Avoid comments at all costs. Instead: self-documenting code.

> The proper use of comments is to compensate for our failure to express ourself in code.

### Objects vs Data Structures

> In any complex system there are going to be times when we want to add new data types rather than new functions. For these cases objects and OO are most appropriate. On the other hand, there will also be times when we’ll want to add new functions as opposed to data types. In that case procedural code and data structures will be more appropriate.

### Single Responsibility Principle

💡 Lots of small drawers (classes) instead of large drawers with logs of things inside (big classes).

E.g., `ImageRotator`, `ImageResizer`, `ImageFlipper` etc instead of: `ImageProcessor` or `ImageManager`.

> Larger, multipurpose classes always hampers us by insisting we wade through lots of things we don’t need to know right now.

Depends on cohesion (how much member variables are tied to member functions). Maximum cohesion is when all member functions use all member variables.

When some functions use a subset of member variables, consider moving those functions out to a separate class.