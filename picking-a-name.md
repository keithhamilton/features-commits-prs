#Picking a Name
Your parents probably spent hours picking your name, and now that you have a
name, it's generally very simple for anyone who knows it to identify exactly who is being
identified by that name. There is little uncertainty, that if someone in my
office calls for *Keith Hamilton* that there will be any ambiguity as to whom
that person is addressing.

Your feature branches, like your own, or your parents', children, should have names that
specifically identify them as well. Like your surname, your feature branches
should also directly identify their parent.

> The first term in a feature branch should be its author's initials.

Now that your feature branch is directly identified as *being yours*, it's time
for the fun part; actually naming it. A good name for a feature branch should
clarify to any viewer *rather precisely* what the feature branch does, as well
as remain terse in nature:

| Branch Name | Good | Bad |
| ----------- | ---- | --- |
| fb-update | | x |
| fb-refactor | | x |
| fb-change-feature | | x |
| fb-feature-speech-synthesis | x | |
| fb-refactor-router | x | |
| fb-feature-twitter-streaming| x | |
| fb-bug-profanity-filter | x | |

A few things to note in the above table:
* the qualifying type of feature branch, such as *feature* or *refactor*,
should always directly follow the initials of the feature branch's creator
* using vague, standalone terms such as *update* or *refactor* provides
little insight as to *what* is being updated or refactored.
* using longer branch names is ok, but limit to five terms or fewer (including
the branch type qualification)

That's pretty much it on naming your feature branch. Just keep it terse,
descriptive, and always use your initials.
