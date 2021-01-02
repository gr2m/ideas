# Ideas

I use this repository to keep track of side projects I plan to work on (or already started). I'm always looking for collaborators! Please file an issue if one of the projects is of interest to you!

<!-- toc -->

## Open Purse

Status: [work in progress](https://github.com/gr2m/open-purse)

Handle webhooks from marketplace and GitHub Sponsors and make all the data public. I'm using GitHub sponsors and GitHub Apps revenue to raise funds for projects (currently [p5.js](https://p5js.org/)). I want Open Purse to be a transparent way to do so, to hold myself accountable and to give my sponsors and app users the confidence that the money is in fact going where I claim it does.

## Issue/PR reference expander app

Status: idea

A GitHub app that expands links to pull requests: adds inline icons for open/closed/merged pull requests, maybe add support check lists of URLs to PRs that get automatically checked of as PRs get closed/merged

It would parse a comment such as

> requires [#163](#)

and turn it into

> requires [![issue closed](assets/issue-open.svg) #163 Issue title here](#)

## A hosted GitHub OAuth service

Status: idea

Folks can register their OAuth client_id/client_secret credentials for their OAUth/GitHub apps, and can then use "Login with GitHub" without any server component. I'm very into that part, I feel like UI should be the next frontier for GitHub's platfom integrations. Think "smart" web/react components, powered by React, that you can just use in your apps and boom you have a Login UI, list of issues UI, search UI, all hooked up to GitHub's APIs

## Run Probot/GitHub Apps in the browser

Status: idea

The pieces are mostly there. Imagine you open [https://probot.dev](https://probot.dev/) and you see an editor with a Probot App function and intenseness from all the typescript definitions. You can register a new GitHub App using the web manifest flow, and receive events using [smee.io](http://smee.io/) / Server Sent Events. When you are happy, you can "deploy" your probot function to a list of providers we support, by creating a github repository with all the necessary files and repository secrets for continuous delivery

## A web UI for https://github.com/octoherd/

Status: idea

Create and run octoherd scripts online, with dry runs and confirmations, so it would be low risk. And you could quickly hack together a script to update as many repos as you like at once
