#Reintroducing: The Commit Message

The commit message is a simple thing; just a message, really. It communicates
what you did at a certain point in time to a certain part of a codebase.

Anyone who has ever used a source control system has made a commit; it's the
smallest unit of measurement available to a developer contributing to a project.
What is often overlooked, however, is how important this simple element of
source control is improperly used.

###What do you think a commit is?
Before getting into the commit message, go ahead and take a second to come up
with an answer to this question:

> What is a commit message?

Did you get an answer? Great, keep it in mind and keep reading.

###A commit is small, with broad-reaching implications
Lexically speaking, the commit message is the smallest unit of composition in
source-controlled code. It is the building block upon which all other actions
are constructed. Afterall, source control is merely a construct through which
changes are tracked and recorded.

###A commit is a record of history
At any point in the lifetime of a source-controlled codebase, any commit can be
called up at any time, and reverted to, investigated, or re-applied to the
codebase. A commit is a living record of something that happened in time, but
also is like a pawn in chess: small, but with the ability to make dramatic
changes in the flow of a project.

###A commit is a powerful tool
A commit can be replayed on its codebase, merged into other commits to provide
concision to a history log, and lead team mates to an investigative conclusion,
much like a bread crumb trail. To do any of this, however, commits must provide
context as to the what and why of any change recorded in our code's history.
Without an understanding of what and why, replaying and merging commits together
becomes overly laborious, and investigating their reason becomes exhausting.

###So, what is a commit message?
I submit that a commit message, most fundamentally, is:

> The base tool through which we record context about changes to our code.

Note that it is possible to *make a statement about what was done to a file,*
*detail what happened,* or *create a log entry about a change that was made,* all
without providing ***context***. Doing any of those without providing
context, however, is a boot in the eye of your fellow developer, and perhaps, more
importantly, your future self.
