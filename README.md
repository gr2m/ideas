# Ideas

I use this repository to keep track of side projects I plan to work on (or already started). I'm always looking for collaborators! Please file an issue if one of the projects is of interest to you!

<!-- toc -->

- [Open Purse](#open-purse)
- [Issue/PR reference expander app](#issuepr-reference-expander-app)
- [A hosted GitHub OAuth service](#a-hosted-github-oauth-service)
- [Run Probot/GitHub Apps in the browser](#run-probotgithub-apps-in-the-browser)
- [A web UI for https://github.com/octoherd/](#a-web-ui-for-httpsgithubcomoctoherd)
- [octokit.rest](#octokitrest)

<!-- tocstop -->

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

## [octokit.rest](https://octokit.rest) CLI

[octokit.rest](https://octokit.rest) is a website to send requests to GitHub's REST API. It is built on [GitHub's OpenAPI Spec](https://github.com/octokit/openapi#readme). The main interactions are

1. Search one of the 700+ REST API endpoints
2. See the endpoint's details, such as description, parameters, example response
3. Send an actual request

Secondary actions are/will be

4. Authentication. Using token/OAuth Web Flow/GitHub App Manifest Flow.
5. Share. Share a parameterized request. I'd love to promote the tool for bug reports regarding GitHub's API.

I feel the Website and CLI could share a lot of logic and could overal provide a similar user experience. I'd love to collaborate with someone with extensive React experience on this, I think the [next.js](https://github.com/zeit/next.js/#readme) would be a good framework to build the webside, and [ink](https://github.com/vadimdemedes/ink) might be a good framework to build the CLI. Both could share common React components. I'm open to alternatives though
