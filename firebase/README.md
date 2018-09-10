# Firebase Cloud Function Hustle Test
This hustle test is for a __developer__.

Micro-Services and Server-less stacks are becoming more and more common.
Google Firebase is on the most popular. Firebase (the company) was purchased
by Google in 2014 and have been a growing component in their GCP (Google Cloud Product).

Firebase launched Cloud Functions (beta) in March of 2017. This feature allows a
developer to setup independent functions that run either via a HTTP request, or via a
Real Time Database Trigger. Each function runs in own processing space with
dedicated resources.

The challenge with server-less/firebase functions is that testing can be painful,
with a developer writing the code, deploying and then watching the logs to see
if things are working. Google as only recently responded to developer pain
and started offering local emulation tools for development and testing.

Meenta has been using functions since their first release in beta and we have
felt the pain of changing API.

#### Tasks and Deliverables
The task is to setup firebase account (free) and write a simple firebase function. Use any data you want. Then
install the local emulation tools and write tests that allow for testing. Commit the
code to the repo, provide documentation in a `RESULTS.md` file in this folder.

- Setup a firebase account (is free)
- Install the required tools to deploy.
- Setup and deploy one or more functions that updated `realtime database`.
- Write a test that runs locally, or in CI environment for each function.
- Schedule a time to review.

__Please send your github link within 4 days.__

#### Reference Materials
- https://en.wikipedia.org/wiki/Firebase
- https://firebase.google.com/docs/functions/
- https://firebase.google.com/docs/functions/database-events
