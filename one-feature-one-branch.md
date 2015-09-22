#One Feature, One Branch
One of the underlying themes of this book, as you will discover if you've not
yet picked up on it, is that smaller, more concise, logically-separated
operations are the ideal when using git. It should then come as no surprise,
that the same holds true for feature branching.

When making a feature branch, it should address one specific feature, bug,
hotfix, or experiment. Just as with commits (oh, yes, we will get to those
later), **feature branches should never address more than one logical set of
changes.**

If you have multiple, logically divided, changes, make multiple logically
divided feature branches, and keep the changes isolated. We'll talk more about
this in [*Keeping Your Features Separate*](keeping-your-features-separate.md).

**To effectively separate your feature branches**, you should always *check out*
your stable development branch, *then* create your new feature branch.

> Remember, if you create a feature branch from an existing feature branch, the former will contain all of the changes in the latter, and that is bad.
