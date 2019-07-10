# The Art of Agile Development

By James Shore (2003)

> As a programmer you must be able to produce customer value, from scratch, in a single week.

> Managers, rather than telling the team what to do, let the team tell you what they need you to do to help them succeed.

Ward Cunningham:

> It was a turning point in my programming career when I realized that I didn't have to win every argument.

## My Notes

Various interlocking ideas and practices: trust, co-location, pair programming, TDD, customer involvement, stand-ups, coding standards, refactoring, iterative development, emergent design, sprint demos, risk management, spike stories, technical debt, simplicity, time-boxking…

You don't get to pick and choose any combination. E.g., emergent design depends on refactoring which depends on TDD, which in many environments will require trust.

### Trust

Remember: forming, storming, norming, performing.

> You can help by letting people know that disagreement is normal and acceptable. Find ways to make it safe to disagree.

💡 Earning trust outside the team: show some hustle, deliver on promises, manage problems, respect customer goals, promote the team, be honest.

> If failure doesn't hurt, then it's OK to fail. You'll be free to experiment and take risks.

### Focus on Value

> Create stories about your customers's needs, not your plans to fulfil those needs.

### Simplicity

> Simplicity is the art of maximising the work not done.

Avoid anticipating needs. Do not speculate. Concentrate on the requirements.

> The plan can change every week. Unless you're implementing the feature that very week, don't put the hook in.

💡 Build requirements, design/architecture and implementation iteratively.

> It's easier to expand an architecture than it is to simplify one that's too ambitious.

### Planning

💡 Delay planning until the last responsible moment (because priorities change).

Define future work in tiered horizons (the nearer the work, the more comprehensively).

Programmers estimate, customers prioritise.

Make planning a conversation.

Typical sprint planning: demo (30 minutes), retrospective (1 hour), planning (up to 4 hours).

Don't finish iterations on Friday (work shouldn't slip into the weekend, and a last-minute rush doesn't work well on a Friday).

### Estimates

Not sure if this is from this book: sprints, velocity, etc avoid the situation where:

- You made an estimate
- It was too optimistic
- You're made to suffer because delivery was "late"
- Next time you add padding
- Management knows, assumes or catches on that estimates are padded, so they push for estimates to be revised down
- Instead of having an open and productive conversation about uncertainty, risk, flexible scope, needs, compromise, etc, it becomes a negotiation where each side distrusts the other

☝️ Also, with padding and [Parkinson's Law](https://en.wikipedia.org/wiki/Parkinson%27s_law), it's possible work is delivered later than necessary. Also, remember this benefit of iterative development: development can be halted at any time, even before finishing everything in the backlog, once the customer's needs are met.

### Releasing

The point is not to release all the time but enable you to release at any time.

Each story should be releasable on its own.

### Done Done

💡 You get no points unless a story is completely done.

Team should create their own definition of done. E.g., coded, tested, designed/refactored, integrated, migrations prepared, reviewed, fixed, accepted.

### Coding Standards

> An exercise in building consensus.

Naming, formatting class and function length, error-handling, logging, etc.

### Collective Code Ownership

Nobody owns any particular parts of code and quality is everyone's responsibility.

> Every week your design should be better than it was the week before.

### Vision

Explain why our work is important.

> Be specific but not prescriptive.

### Technical Debt

> A good rule of thumb is to spend 10% of an iteration on technical debt.

> [Technical debt] has a greater impact on team productivity than any other factor does. Make code quality a priority and your velocity will improve dramatically.

### Research Time

Half a day per sprint.

> If you're concerned about people goofing off, provide lunch the next day and ask that people share what they've done in informal peer discussion. This is a good way to share knowledge anyway.