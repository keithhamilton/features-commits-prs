#Crafting a Good Commit Message

###Commit message subject
The commit message subject is either the entire commit message (single-line
commit), or the first line in a detailed commit (followed by the commit body).
In any event, a good commit message subject should:

* Begin with a capital letter
* Not end with a period
* Be fewer than 50 characters in length
* Address, as specifically as possible, the change being made
* Use the imperative voice

###Single-line (Subject-only) commit messages
When a commit is sufficiently simple in scope, the body can be skipped
altogether in favor of a single-line commit message, using the `-m` option. Note
that the above guidelines should be used for a single-line commit message. For example:

    $ git commit -m "Fix typo in site index body copy"

Anyone reviewing the above commit message down the road will get a full picture
of the change made with this commit (assuming it was the only change made by
the commit), and it more information about what the change was is needed, one need only run

    $ git show [commit sha]

###Detailed commit messages
When more detail is needed, a full commit message can be written using the
shorter form `git commit`.

The structure of a detailed commit message looks like this:

    Commit subject goes in the first line of the messages

    Detailed message goes in below. This is a great spot to
    add in more information about what went on in the change
    attached to this commit. If you need to detail out different
    changes that you've made under this commit message:

    * Consider using a bulleted list (use markdown syntax)
    * Where each change is detailed as its own commit subject
    * Remember to use the above subject guidelines

###Commit message body
The commit body should be used when additional information is required to fully
explain the commit subject. This can be very useful in describing a number of
changes that fall under one subject. A good commit body:

* Is separated from the subject line by a blank line
* Is wrapped to 72 columns to eliminate horizontal scrolling
* May contain a bulleted list
* Should explain *what* changes were made, and *why* they were made, as opposed to *how*

###On using the imperative voice
When writing a commit message, the preferred tense should be in the imperative
voice. The imperative voice is the same voice we use when we make a command. Think
*"Pass me the salt,"* or *"Come over here, and I'll show you."*

The reason the imperative voice is preferred in commit message subjects is that
when reading a commit message subject, it is beneficial to think of them as
current actions and not past actions. Why?

It is beneficial to think of commit message subjects as actions, because they
will be actions when you merge them into your local branch! Think about this:

    There's you and Joe Developer. Joe is branched off on a feature branch and when
    he's all done, he submits a pull request to merge it into the current
    development branch.

    You review Joe's pull request and decide "yeah, this looks great," so you
    merge the code. What is really happening when you merge the pull request
    into the development branch is each commit from the point at which Joe
    branched off of the development branch is "replayed" on top of the current
    head of the development branch.

So, effectively, each time a commit is replayed onto the development head,
you can describe the action by reading the commit message as:

> When this commit is applied to the development branch, it will [insert commit message here].

For example, if your commit message is "Update the user CRUD API," when you merge
that commit, you can say:

> When this commit is merged, it will [u]pdate the user CRUD API.

The core point here is to think of commits as actions, and therefore the
messages as descriptions of what will happen when the commit is played on top of
the current head.

