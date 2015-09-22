#Why Make a Feature Branch?
There are two major umbrella answers to this question.
* What is the purpose of making a feature branch?
* When should I make a feature branch?

Let's look at each in turn.

###What is the purpose of making a feature branch?
The root reason to make a feature branch is to protect your codebase. By
default, when you create a new repository in git or GitHub, the working branch
of your codebase is `master`. In most situations, this is the branch of the
codebase that will end up in production.

If you are so lucky to have your code make it into production, you will
certainly want to keep it running. This is the first, *and perhaps most
compelling*, reason to make feature branches when developing your code:

> If you deploy directly to master, you endanger your product.

If you're familiar with *git flow*, you will recognize the use of the *develop*
branch. The *develop* branch, is, in its basic nature, a giant feature branch
that distinguishes production-ready code, from in-progress code. You and your
fellow developers, dilligently working in your own feature branches, will
periodically submit pull requests to the *develop* branch for inclusion. This
brings up the second important reason to make a feature branch:

> By using feature branches, you protect the code your teammates have written.

Working on a team requires many authors to develop independently, gradually
weaving their code back together into a unified branch, much as a braided rope
consists of multiple, smaller, ropes that unify into a stronger entity. By using
feature branches, each person is capable of developing his/her own code without
other teammates constantly, and unintentionally, throwing monkey wrenches into
the mix. Each team member is allowed to develop a new feature based on the
current stable development branch, without worry about others' experimentation.

Which brings us to the third compelling reason to use feature branches.

> Developing in feature branches allows you to fail with grace.

One of the best outcomes of working in feature branches is that, by doing so,
you permit yourself the opportunity to fail without consequence, excepting time
spent failing, which arguably has its own merits.

Say you spend a five hours working on a feature that you think will greatly
enhance your team's end product. Five hours later, you discover a deeply
embedded flaw in your logic, and realize that you've just wasted five hours of
your life developing a dead-end feature.

It's not a total loss; for starters, you've learnt something, which is great!
Secondly, you can just check out your stable development branch again, then
delete the feature branch you were working on; you will find everything just as
you left it. No harm, no foul!

However, it may have been nice to have someone else's eyes on that code you just threw
away, and we'll get to that in the section on
[*pull requests*](pull_requests.md). Incidentally, this is the last major *why*
when it comes to the purpose of making a feature branch.

> Feature branching leads directly to code reviews.

Every time you want to merge a feature branch back into the development
codebase, stop, take a deep breath, then make a pull request. Again, we'll get
into pull requests later in this book, but for now, just remember that *pull
request* is fairly synonomous with *ask for review*.

By making pull requests that ask your feature be integrated into the development
branch, you gain insight in the form of your entire team looking at your code,
and uncovering missteps, malpractice, or logical misdirection that a single pair
of eyes is prone to overlook. This is great! More eyes, better code.

Ok, so we've discussed the purpose of feature branching; let's move on to
knowing when to make a feature branch.

---

###When should I make a feature branch?
Making feature branchs is a great thing, and should happen *early and often*.
Keeping in mind the idea that the *stable* branch needs to remain *stable*, it's
a good idea to make a feature branch when:

* **You want to add a new feature to the codebase.** This could be a functional
aspect of your code not yet implemented, a refactor of existing code, or a shiny
new bell or whistle.
* **You want to address a bug in your existing codebase.** Before attempting to
  repair a bug in your code, consider that the fix should happen in its own
  branch. Attempting to repair the stable development branch is dangerous; you
  may not know the root cause of the bug and in digging around for it, you may
  cause unintended errors on the development branch. Remember, failing
  gracefully is the goal. No one wants to destroy countless hours of others'
  work on accident.
* **You just want to experiment.** If you have been noodling around an idea for
  an experimental feature, **make a feature branch for it!** By using a feature
  branch, you can play around until your heart's content, or your brain is
  destroyed, and you won't risk any side-effects on your stable codebase. This
  is a great thing! Branching basically gives you free license to do whatever
  you want with little consequence (again, mostly time).
