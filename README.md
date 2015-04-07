# Retrospectives

## What / Why?

Sometimes things don't go so well - let's say there's "an incident".
It could be that something breaks in production, or we put someone on the wrong plane, or there's a critical misunderstanding.

It's important that we learn from these incidents, and share what we've learnt so that others can benefit from it, whether it's about incident prevention, discovery, or recovery.

For example, a production bug can teach us things about our code review process (how did the bug end up in production), our testing / monitoring processes (could we have discovered it earlier), and much much more.

## How?

The modern developer's favourite: markdown files in a GitHub repo.

When there's an incident, start filling in `TEMPLATE.md` and add it in a PR. @-mention those involved in the incident, discuss and record what happened and what you can learn, and when you're all happy, merge it in.

Don't worry if you don't have the complete details before filing the PR - that's why it's a PR - just starting with _something_ is a benefit.
