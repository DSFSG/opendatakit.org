# Contributing code to the ODK website

This is a living document. If you see something that could be improved, edit this document and submit a pull request following the instructions below!

## Submitting a pull request
To contribute code to the ODK website, you will need to open a [pull request](https://help.github.com/articles/about-pull-requests/) which will be reviewed by the community and then merged.

1. [Set up your development environment](https://github.com/opendatakit/website#setting-up-your-development-environment). 

1. To make sure you have the latest version of the site, set up this repository as [a remote for your fork](https://help.github.com/articles/configuring-a-remote-for-a-fork/) and then [sync your fork](https://help.github.com/articles/syncing-a-fork/).

1. Create a branch for the code you will be writing:

        git checkout -b NAME_OF_YOUR_BRANCH

1. If there is an [issue](https://github.com/opendatakit/website/issues) corresponding to what you will work on, put `@opendatakit-bot claim` as a comment on issue to say you are claiming it. If this is your first time contributing to the repo, the bot will send you an invite. Once you accept this invite, the bot will assign you to the issue. If there is no issue yet, create one to provide background on the problem you are solving.

1. Once you've made incremental progress towards you goal, commit your changes with a meaningful commit message. Use [keywords for closing issues](https://help.github.com/articles/closing-issues-via-commit-messages/) to refer to issues and have them automatically close when your changes are merged.

        git commit -m "Do a thing. Fix #1."

1. Push changes to your fork at any time to make them publicly available:

        git push
        
1. When your changes are ready to be added to the core ODK website, [open a pull request](https://help.github.com/articles/creating-a-pull-request/). Make sure to set the base fork to `opendatakit/website`. Describe your changes in the comment, refer to any relevant issues using [keywords for closing issues](https://help.github.com/articles/closing-issues-via-commit-messages/) and tag any person you think might need to know about the changes.

1. Pull requests will be reviewed when committers have time. If you haven't received a review in 10 days, you may notify committers by putting `@opendatakit/website` in a comment.

## Making sure your pull request is accepted
1. Confirm that the site compiles.

1. Verify the functionality. Describe in the pull request how you confirmed that your change works as expected.

1. Make sure that there is an issue that corresponds to the pull request and that it has been discussed by the community as necessary.

1. Keep your pull request focused on one narrow goal. This could mean addressing an issue with multiple, smaller pull requests. Small pull requests are easier to review and less likely to introduce bugs. If you would like to make stylistic changes to the site, create a separate pull request.

1. Document your reasoning. Your commit messages should make it clear why each change has been made.

## The review process
Pull requests corresponding to issues with a clearly stated goal and/or a process for manual verification are given priority. Pull requests that are unclear or controversial may be tagged as `needs discussion` and/or may take longer to review.

We try to have at least two people review every pull request and we encourage everyone to participate in the review process to get familiar with the content and help ensure higher quality. Reviewers should ask themselves some or all of the following questions:
- Was this change adequately discussed prior to implementation?
- What other content could this PR affect?
- Is the content easy to understand and to maintain?

When a pull request is first created, @opendatakit-bot tags it as `needs review` to indicate that code review is needed. Community members review the code and leave their comments, verifying that the changes included are relevant and properly address the issue. A maintainer does a thorough code review and when satisfied with the code, tags the pull request as `needs testing` to indicate the need for a manual [black-box testing](https://en.wikipedia.org/wiki/Black-box_testing) pass. A pull request may go back and forth between `needs testing` and `needs review` until the behavior is thoroughly verified. Once the behavior has been thoroughly verified, the pull request is tagged as `behavior verified`. A maintainer then merges the changes. Pull requests that need more complete reviews including review of approach and/or appropriateness are tagged with `reviews wanted`. Any community member is encouraged to participate in the review process!

Small fixes that target very particular bugs may occasionally be merged without a second review.

## Content from external sources
The ODK website is released under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/). Please make sure that any content you include is a compatible license. **Please note that if no license is specified for a piece of code or if it has an incompatible license such as GPL, using it puts the project at legal risk**.
