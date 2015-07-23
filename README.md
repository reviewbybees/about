# About @reviewbybees

CloudBees, Inc. has some internal code review processes. One of the requirements is that we get changes signed off by other CloudBees employees.

To help us identify the Pull requests in GitHub that we need to review, we typically just mention `@reviewbybees` in the pull request. That lets us see the review requests that we need to review using [this handy query](https://github.com/pulls?q=is%3Aopen+is%3Apr+mentions%3Areviewbybees+NOT+wip+in%3Atitle+sort%3Aupdated-desc).

Our current internal process requires that **before we seek to get a change merged** we must have either:

* At least two :bee: comments from CloudBees employees; or
* At least one :bee: comments from a CloudBees employee and at least 12 hours since the last commit.

In addition, if there are any :bug: comments from CloudBees employees then we are not allowed to ask for the change to be merged until the issue identified has been resolved.

(Note that :bee: or :bug: must be in *general comments*, not *line comments*.
You should add a :bug: to mean that you are opposed to the PR at that point.
This remains in effect until you supersede it with a :bee:,
regardless of whether there have been intervening commits.)

However, that does not mean that you, as a maintainer of your open source project need to pay any attention to our processes:

* If you see a change that you think should be merged, and you want to merge it now, it's your project, so it's your call
* If you see a change that is taking the code in a direction you don't like, tell us... no need to wait while we polish up the pull request if ultimately our proposal would take your project in a different direction. 

*NOTE:* A previous version of our process used :+1: and :-1: but some people communicated that these vote types were implying that the change should be merged by the maintainer. As a result, we have changed our process to use :bee: to signify that a bee has reviewed the change. We are using :bug: to signify that the reviewer has problems with the change: perhaps the reviewer is confused by the change; perhaps the reviewer has spotted a suspected bug; perhaps the reviewer believes the change is increasing technical debt in the project.
