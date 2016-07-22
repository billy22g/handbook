---
title: Intro to GitHub and the 18F website
navtitle: GitHub and the 18F website
---

_This section covers the basics of how 18F&rsquo;s website works and includes a brief overview of Git._


### Leadership

[Outreach](https://handbook.18f.gov/outreach) is responsible for maintaining the 18F website. [Greg Boone](https://18f.slack.com/messages/@gregboone) and [Elaine Kamlley](https://18f.slack.com/messages/@elainekamlley) are the lead developers.

### Communication

Find us in Slack:

- [#18f-site](https://18f.slack.com/messages/18f-site)
- [#18f-site-design](https://18f.slack.com/messages/18f-site-design)
- [#18f-site-dev](https://18f.slack.com/messages/18f-site-dev)
- [#dev](https://18f.slack.com/messages/dev)
- [#git](https://18f.slack.com/messages/git)

### Documentation

- [GitHub](https://handbook.18f.gov/github/) - A detailed guide on how we use GitHub at 18F.

- [GitHub for Beginners](http://www.digitalgov.gov/event/github-for-beginners/) - Intended for beginners, this video class is led by Will Slack. Slides are available [here](https://pages.18f.gov/slides/github-basics/#/18) and course materials are [here](https://docs.google.com/document/d/18b-4VPTcuqat-enGQSVzivGH2CsqdQVG0K0eToRM39I/edit).

- [How to use GitHub, the terminal, and the 18F site](https://18f.gsa.gov/2015/03/03/how-to-use-github-and-the-terminal-a-guide/) - This tutorial from Melody Kramer and Greg Boone walks you through using GitHub to contribute to our blog. It's intended for beginners, but includes tips for intermediate GitHub users, too.

## GitHub

[GitHub](https://github.com) is a publicly accessible place to share and collaborate on (primarily) open source software projects. GitHub interacts with a program on your computer called Git that tracks every change ever made in a software project.

You&rsquo;ve probably already noticed there&rsquo;s a lot happening on GitHub at 18F. That&rsquo;s because it&rsquo;s so useful! In fact, it&rsquo;s very likely you&rsquo;ll interact with GitHub in _some_ way, even if you&rsquo;re not writing code. The remainder of this post will help you get you squared away with creating your GitHub account and setting up some basic stuff, and will show you some of the ways you might use GitHub, even if it&rsquo;s not committing code.

### 1. Set up your account

Follow the instructions [here](https://handbook.18f.gov/github/).

### 2. Basics

If you&rsquo;re a developer, you might have very strong feelings about The Right Way to Use Git, but 18F doesn&rsquo;t (yet) have One Way of Using Git, so ask your teammates how they work with GitHub.

If you&rsquo;re not a developer or came from a place that didn&rsquo;t use Git, here are some GitHub-related terms you should be familiar with:

- **Repo** is short for repository, or a project on GitHub. Anybody at 18F can create repos in the 18F organization and you should _always_ create new projects as 18F, not as yourself. You can create new repos in GitHub by clicking the + next to your profile picture. Then, choose New Repository and change the owner to 18F.

- The **license** on every repo must be Creative Commons 0, or CC0. That&rsquo;s shorthand for Public Domain. 18F is not only committed to working in the public domain by our own policies, but is also committed [by law](https://www.usa.gov/government-works). (Though we are allowed to by law, we don&rsquo;t trademark our logo.) There are a few exceptions to that rule, so check with [#admins-github](https://18f.slack.com/archives/admins-github) and [#wg-opensource](https://18f.slack.com/archives/wg-opensource) before putting any license _other_ than CC0 on your project. For more details about licensing, see our [open source policy](https://github.com/18F/open-source-policy), [our blog posts about open source](https://18f.gsa.gov/tags/open-source/), and the [Open Source Style guide](https://pages.18f.gov/open-source-guide/). You&rsquo;ll hear more about open source during [Gray&rsquo;s seminar on Product and Open Source](https://handbook.18f.gov/intro-to-product-and-open-source).

Once you&rsquo;re a member of the 18F organization, you&rsquo;ll have access to many of our repos.  You&rsquo;ll also have at least read-only access to a few of our private repositories. Check with your team on how to interact with a project. In some cases, the repos themselves have information in a `CONTRIBUTING.md` file for guidance.

- A **fork** is a copy of the main project that is fully separate from 18F&rsquo;s. You might be asked to fork a repo and work off your own copy, or you might be asked to commit directly to your team&rsquo;s original repo. This is the kind of thing you should ask your teammates about — don't make assumptions!

- There are a few exceptions to this, but generally speaking, you will submit any changes to a project through a pull request. A **pull request,** or **PR,** is a way of saying  &ldquo;here are some changes I&rsquo;d like to contribute &rdquo; and letting the repo&rsquo;s owner decide whether to accept (or merge) them or give feedback. Sometimes your pull request will go from your fork to the main project, sometimes from a _branch._ Again, make sure you understand your team&rsquo;s Git workflow. On [#18f-site](), nobody forks and everybody works off of branches; we submit pull requests to the staging branch.

- Developer, designer, editor, manager: Whatever your role is, you&rsquo;ll want to get used to **filing issues on GitHub.** Issues are a common way of submitting feedback on projects at 18F. For example, if you want to write a blog post, you&rsquo;ll be asked to submit an issue to the blog repo. If filing an issue seems more difficult for some reason, head to Slack. Or vice versa.

- You may find it helpful to bookmark the repos, issues, and pull request pages you access frequently.

### 3. Working with GitHub

If you&rsquo;re working with an agency, you'll need to find ways to collaborate with them on the project you're tasked with. Typically, the way we give outside agencies and contractors access to GitHub repos is by making those repositories public. Once they&rsquo;re public, anybody can access them; we just need to add people as a collaborators. [#admins-github](https://18f.slack.com/archives/admins-github) can help you with that.

You can use GitHub for almost anything, but consider the resources available to agency partners or other stakeholders before deciding to use it. Are your agency partners used to using GitHub? Will they need to create accounts and jump through hoops? Can they even access it from their agency computers? These are the kinds of things we consider when deciding if GitHub is the right thing to use.

18F sometimes adds contractors and agency partners to the 18F organization on Github. We sometimes use forks to collaborate with contractors. Sometimes we do both. Again, check with your team on how to do this.

Most projects/repositories have a `CONTRIBUTING.md` file in their root directory that explains how the team invites people to contribute to the project. They might prefer chats over pull requests, for example.

Another pro tip: Search the existing issues before you add one. It may make more sense to comment on that issue rather than create a new one.

To submit an issue, Log in, find the appropriate repo on GitHub, and click the Issues tab in the right column. Then, click the New Issue button. Your issue should have a title and explainer text. You&rsquo;ll probably know what to put there, but teams sometimes have guidance on how to format issues or things to include. The [#blog](https://18f.slack.com/archives/blog), for example, has [a specific set of things we require](https://github.com/18F/blog-drafts#readme) submissions to have before we&rsquo;ll consider them.

Final pro tip: If your project wants to issues formatted in a specific way, you can send people links with the title and body of the issue partially filled in. All you have to do is add `title` and `body` URL attributes to the new issues URL: https://github.com/18F/\<repo\>/issues/new.

Here's an example: [https://github.com/18F/handbook/issues/new?title=Greg%20told%20me%20about%20this](https://github.com/18F/handbook/issues/new?title=Greg%20told%20me%20about%20this). Click that link and you should be see the title filled in on an issue for this repo. To add text to the body, too, add `&body=` like this: [https://github.com/18F/handbook/issues/new?title=Greg%20told%20me%20about%20this&body=It%20works!](https://github.com/18F/handbook/issues/new?title=Greg%20told%20me%20about%20this&body=It%20works!). Technically you can put anything in these strings, you just need to know how to encode the url elements. The blog team does this to help people pitch posts, [you can see it on their readme](https://github.com/18f/blog-drafts).


## 18F site

[18f.gsa.gov](http://18f.gsa.gov/) is a **static site** based on the Jekyll platform. (We use Jekyll pretty extensively at 18F. The [pages.18f.gov]() platform is built around Jekyll, and that&rsquo;s basically our version of GitHub pages).

Staging is our master branch so our flow is: User creates a branch submits a pull request to staging that deploys [staging.18f.gov](http://staging.18f.gov); When staging.18f.gov is good, we submit a PR from staging to production and that deploys 18f.gsa.gov.

18F&rsquo;s website also uses **continuous integration** to run tests on the site at each pull request. Our **deployments** are triggered by **webhooks** running on [18f.gsa.gov/deploy](http://18f.gsa.gov/deploy). GitHub shoots us some JSON and the site rebuilds. For CI, we use Travis on [#18f-site](https://18f.slack.com/archives/18f-site), many projects seem to use Circle, and MyUSCIS uses a Jenkins server.

We use [Google Analytics](https://handbook.18f.gov/google-analytics/) to track site usage.

### Add your bio and photo

The only way new employees need to interact with the 18F site during their first month is to add their bio and picture to the Team page. This isn't mandatory, of course, but we&rsquo;d really like it if everyone had a photo and a bio. (Folks who don't upload photos are represented by the 18F logo on the Team page.)

To get going, find or take an appropriate photo and upload it to [this Google Drive folder](https://drive.google.com/a/gsa.gov/folderview?id=0B8kn3cuJUwEkLUMwWXE2VVczbUU&usp=sharing). We have some guidelines about good photos, [here](https://drive.google.com/a/gsa.gov/folderview?id=0B8kn3cuJUwEkLUMwWXE2VVczbUU&usp=sharing).

Next, fill out [this form](https://docs.google.com/a/gsa.gov/forms/d/1XRCkQZw3-1JoZh6tm4k1qbunEnvJdOvDrTjRCqs-dp4/viewform) and we&rsquo;ll take it from there. (If you&rsquo;re interested in contributing to the site as a developer or designer, talk to [Greg Boone](https://18f.slack.com/messages/@gregboone) or [Elaine Kamlley](https://18f.slack.com/messages/@elainekamlley) or join [#18f-site-dev](https://18f.slack.com/archives/18f-site-dev).
