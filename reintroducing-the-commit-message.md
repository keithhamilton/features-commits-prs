#Reintroducing: The Commit Message

The commit message is a simple thing; just a message, really. It communicates
what you did at a certain point in time to a certain part of a codebase.

Anyone who has ever used a source control system has made a commit; it's the
smallest unit of measurement available to a developer contributing to a project.
What is often overlooked, however, is how important this simple element of
source control is improperly used.

###Is it what you think it is?
Before getting into the commit message, I'd like you to sit back, take a second,
and silently come up with an answer to this question:

> What is a commit message?

Did you get an answer? Great. Was it something like:

> A statement of what was done to a file...?
> A message detailing what happened...?
> A log entry about a change that was made...?
> Something you do before pushing code...?

If you said something like the above, it wouldn't be surprising, because most
people don't think of commit messages as communication tools, rather simply log
entries.

*Communication tools* are used to facilitate communication. Communication is the
practice of clarifying intent, and exchanging information to satisfy intent.
Clarifying intent is achieved through providing context.

###What is a commit message?
I submit that a commit message, most fundamentally, is:

> The base tool through which we record context about changes to our code.

Note that it is possible to *make a statement about what was done to a file,*
*detail what happened,* or *create a log entry about a change that was made,* all
without providing ***context***.

Context is the fundamental difference between a good commit message, and a bad one.

