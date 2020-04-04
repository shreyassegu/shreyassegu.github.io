---
layout: post
title:  "Getting into a new project..."
categories: [ Tutorials ]
image: https://images.unsplash.com/photo-1519389950473-47ba0277781c?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1280&q=60 
beforetoc: ""
featured: true
toc: true
comments: false
---
Getting into a new project can be daunting, and uncertain. Learning enough about the complex system which is already in place and understanding enough to make a contribution especially with respect to a software engineer is easier said than done.

Getting up and running very quickly, and proving the value which you bring to the team is especially important in the current agile work environment, where the development cycles are small and the number of things which are being added to the system all the time is huge. In this fast pace it is most important to get your things together and make meaningful contributions to the team as soon as possible.

These are some of the things which I have picked up when we, an entirely new team had to own the entire system in a short duration of time. These are the tips which I picked up from my manager who guided us in doing these things to ensure that we could make meaningful contributions in a very short time and we had no knowledge gaps so that we won't be stuck in any part of the development process. I call this the **framework of learning** (*from a software engineer's perspective*).
## Understand what you're getting into
- Talk and setup sessions with your product manager/owner, or anybody who has been working on it for a while to get a clear understanding of what the system is actually doing.
- Understanding the business point of view is equally important as the technical side of things.
- Ask as many questions as you possibly can. Seriously..
- Ask about the technology stack, and all of the niche technologies which they are currently using, and also if they are using any proprietary set of tools.
  - Catch up on any technical debt **ASAP**, nobody knows everything remember that.

## Get all the dependencies and potential blockers sorted
- Downloading all the repositories of the codebases.
- Downloading all the configuration for the system, it might be another repository itself.
- Getting knowledge about the build scripts of the system.
- Building it and setting up all the dependencies of the project in your system is the end result of this phase and verify that your local setup of the application is functioning as expected.

## Understand the workflow of things
- Establish a workflow from start to end and trace out what is going on so that you get a baseline understanding of what the system is actually doing.
- Read the various tests which are available in the codebase to make sense of the features and functionalities. These tests might include
  - Integration tests /  Acceptance tests / E2E tests
  - Smoke tests / Sanity tests
  - Performance tests
  - Unit tests
- By this time you should have an overall better idea of what you're actually dealing with, and it will help you to get a feel of how the code is written and the conventions used

## Documentation
- Gather all the documentation which is available.
- Prepare a new set of your personal documentation as you go along.
- Compare it with the reference documentation / setup regular sessions with the project mangers to make sure that you're understanding is correct and it will resolve any misconceptions which you might have.
- This gives you a chance to evaluate the existing documentation as well as you have a fresh set of eyes and can identify any shortcomings easily and you can improve the documentation as well. Remember we are trying to make contributions as early as possible.

## Understand the Environment and CI/CD
- Examine and gather information of all the different environments which belong to the application.
- Get access to all of these environments as soon as possible.
- Understand the build scripts of all the different modules, which artifacts every step produces, where and how we are consuming these artifacts.
- Understand the CI/CD pipelines, in detail.
- Understand the differences between the pipelines of the different environments.
- Talk about the release process, who does it and who takes ownership of the release.

I hope this information might be useful to many engineers who want to get going faster, and this might help your learning process a lot more streamlined and efficient. I will add on to this document whenever I learn new things which will be helpful for everybody else.