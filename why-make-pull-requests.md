#Why Make Pull Requests?
Apart from integrating feature branches into your main codebase, are there other
beneftis that we can gain from using pull requests?

###Puts the brakes on merging
I'm sure you are familiar with the proverb: *haste makes waste.* It's true, as
it goes (or it wouldn't be a proverb). Writing that hot piece of code you've
been cooking up in your head, then immediately slamming it down on your
opertional, stable development branch is hasty, and more often than not, it will
bite you right in the ass.


When your code goes directly from feature branch to the stable development
branch (or worse, when you work directly off of the stable development branch),
you make the assumption that whatever code you've written is ready for
integration. The problem with that is that the codebase isn't yours, it belongs
to the team, so it's not entirely your decision on whether something gets
integrated.

###Eyes on your code
TBD

###Added expertise
When developing as a team, there will always be those with varying levels
of subject, linguistic, and procedural expertise. By using pull requests as the
medium by which code is integrated, it provides the team, as a unit, the
opportunity to enhance code, catch mistakes, and generally improve what was
written before it enters into the main codebase. This of course requires, at
minimum, some loose guidelines surrounding the code review itself.


###Chicken soup for the developer's soul
Arguably the most subjective benefit to using pull requests to integrate your
code, I submit to you that using pull requests is good for your soul.

Why? Because you are flawed. So am I. We are not machines, and, as such, we make
mistakes. Constantly. When you submit a pull request, it is a tacit
acknowledgement that your code *should* be reviewed, nay, that you *want it to
be reviewed,* which is an admission that, whereas you have ideas and product to
contribute, you accept that you are not perfect, and that through peer review,
you can be better.

If you've never submitted a pull request before, you will feel a sense of
hesitance upon submitting your first. You will feel the momentary anticipation
of judgement; you are, after all, putting *yourself* out there to be criticized.
This is completely ok, and I promise this feeling will diminish over time.

This cycle of work, review, polish, and integration is a *good* thing. It will
help you become a better engineer and collaborator, as you learn from your
peers, and learn to better work with others to build a common goal.
