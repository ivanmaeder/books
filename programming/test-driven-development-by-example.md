# Test-Driven Development by Example
By Kent Beck (2000)

> [TDD] isn't a testing technique… It's an analysis technique, a design technique, really a technique for structuring all the activities of development.

## My Notes

### Workflow

Describes the same red-green-refactor process as Robert Martin:

1. Write code for a single test. Run the new test which will **FAIL**
2. Write the application code to make the test **PASS**
3. Refactor (optional) and all tests and to make sure they all **PASS**

Repeat.

There are three choices for writing the application code:

- Faking it (e.g., returning a hardcoded value just to pass the test)
- Obvious implementation (when you know what to do and it's not so general that it's overwhelming, do it)
- Triangulation (implement a general solution to pass two or more tests)

💡 Gives you an opportunity to build a solution in steps, focusing on one step at a time (as opposed to thinking through a solution that addresses multiple situations at once).

### Design/Refactoring

💡 Things often get ugly along the way. Code is duplicated, it's in the wrong places, it's hard-coded, ugly, loose ends are left lying around.

If the same idea exists in test code and application code, there's duplication. Fix it.

Different metaphors lead to different design paths, all can be valid. E.g., `Expression`, `MoneySum`, `MoneyBag`, `Wallet` as different solutions of the same thing…

> The biggest surprise for me including the money example was how different it came out this time.

### Tips

💡 While coding, thoughts that pop up in your mind (edge cases, possible designs/refactors, things to keep track of, etc), write them down and forget about them. Keep doing what you were doing and come back to them later.

> I will entertain a brief interruption, but only a brief one, and I will never interrupt an interruption.

Finish a coding session with a failing test (unless that's what you'll be leaving your teammates with).