# Incident Name (Tweet-length)

Incident summary, of one or two sentences at most (e.g. 300 chars) - enough to get an idea of what happened, without too much detail or verbosity.

## Description

What actually happened.
Clear detail, ideally covering consequences as much as possible.
Mention beliefs / assumptions too - if you thought that alert A meant X was broken, but it turned out to be Y, that's very reasonable to document (it probably means alert A should be much clearer!)

Be blameless and impersonal and anonymous - this isn't about documenting people's faults, or mistakes they made, it's about shared learning.
"$BOB thought X would help, so did it, and it made things worse" is probably going to discourage $BOB from trying to help in future; try writing it abstractly ("It was thought doing X would help, but it didn't") or just using "we" ("We thought X would help").

[Five Whys](https://en.wikipedia.org/wiki/5_Whys) can be a useful method for ensuring that we don't just tackle the "obvious symptom" of an incident, but also look at the things that led to the incident in the first place.

## Takeaways

What can we learn/do as a result of the incident.
Avoid being too abstract; "add more logging" is almost universally a good idea, but so vague as to be slightly unhelpful a suggestion - "log an event every time we send an email, not just if we get an error" is much more useful.
Create and link to issues / bugs as appropriate.

Examples:

What can we do in future to _prevent_ the incident, or reduce the chances of it repeating, or prevent/reduce similar incidents (e.g. "We deployed broken packages to production - we should ensure the packages we deploy to testing are the same as we deploy to production")

What can we do to help _detect_ the incident / potential incidents sooner (e.g. "If we monitored the age of the last backup, we'd have noticed the backup script failing sooner")

What can we do to make _resolving_ the incident easier (e.g. "We could not roll back to a known-good version because the old version had been deleted - lets keep old versions for longer")
