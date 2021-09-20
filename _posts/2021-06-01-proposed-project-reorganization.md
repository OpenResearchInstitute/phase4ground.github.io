---
layout: post
title: "Proposed project reorganization"
author: Juno Woods, Thomas Parry, and Chelsea McMahon
---

The last few weeks, we've been working to re-organize our project website in order to make Phase 4 more accessible for newcomers. Next up are the project repositories and documentation.

We are soliciting your feedback on a number of possible changes. We encourage you to suggest others as well.

## Proposed changes

### Unified GitHub organization: phase4radio

The division between `phase4ground` and `phase4space` on GitHub is somewhat arbitrary, and makes it hard for newcomers to find what they're looking for. We want to rename `phase4ground` to `phase4radio` and have this be the main project account, and we want to either rename `phase4space` to `phase4proto` and have it be used strictly for prototype and temporary code, or delete it and have users work in their personal github accounts (or in the main project repositories, see below).

In either case, we want to move toward `phase4radio` containing only a handful of projects that are either (a) active or (b) completed.

### Merging of repositories

A mark of high-quality free/libre or open source software is thoughtful use of modularity. For example, DVB-S2 FPGA code might be useful for other projects; is it likely that these other projects will use it independently of Generic Stream Encapsulation, or will they mostly be used together?

The receive and transmit code ought also be combined. And if there are Jupyter notebooks or other test scripts that were used as resources for prototyping the DVB code, these should also be rolled into that repository in a subdirectory.

### Issue trackers and to-do lists

The current generic onboarding process looks a little like this:

![Illustration of the below steps](/assets/blog/issue_flow.png)

1. Interested person discovers the project and requests to join Slack, then waits to be added.
2. Interested person asks on Slack what needs doing, and waits around for someone to answer.
3. Interested person checks out the code and starts working on the thing but realizes they don't fully understand the requirements, and then has to wait for more answers.
4. Repeat steps 2-4.
5. The person either completes or abandons the task.

This is a discouraging process. Few people make it through the gauntlet. We want it to look like this instead:

![Illustration of the below improved steps, which is much simpler than the earlier illustration](/assets/blog/better_issue_flow.png)

In this case, the person joins Slack and starts working on a task in parallel. In addition, they log their progress in the issue tracker so that if they abandon the task, someone else can pick up from where they left off.

The lower the barriers to entry, the more people we'll recruit.

As such, we recommend:

* That everyone running a project add issues that are labeled by difficulty and required language and skills. Add the thing you yourself are working on right now! Add little tasks that have been bothering you but that you never get around to finishing. Add big things that you want to do down the road.
* That everyone use the GitHub [to-do list](https://github.com/orgs/phase4ground/projects/1) feature. We'd eventually like this to be complete enough to turn into a project roadmap of sorts, so any potential donor, user, or contributor can easily see how far along we are and where we need assistance.

## Comments welcome!

We're submitting this as a pull request on phase4radio.org. You can comment on the pull request or check out the branch and edit it directly, just as you would for any other code. We encourage your feedback and thoughts, and please let us know if we missed anything.