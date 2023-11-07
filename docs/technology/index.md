---
layout: default
title: Technology
has_children: true
nav_order: 3
---

It is a Django application, the code is on Github and the application is hosted on Heroku.
We are using a postgres database.

Some static files are hosted on Amazon S3.
We are using a mail service from a smaller provider, see the settings.

Site analytics are from Simple Analytics.

For deployments, we are using a method where from all pull-requests, a review app can be created.

Both review apps and the staging app run on the same database, which is separate from the live database.

The idea is that we review the review app, and when agreed, we push the app to staging, where additional tests are run (using selenium, logging in as different users and taking screenshots as well as getiing status codes for al pages).

Now we can promote the staging to live.

A review app is only pushed to staging if it is ready to be released. This way, we keep the main branch up to date and we don't have complicated branching strategies.

About branching: we are working with Github issues and when working on an issue, we create a branch from the issue. This way we automatically close issues once the pull-request is completed.

When working on a feature, we create a main issue about the feature and create issues within that issue. That way, it is easier to keep track of a bigger issue/feature and its progress.
