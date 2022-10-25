# Morgan's Playwright Code Sample

[Playwright](https://playwright.dev/) is used frequently by Ultranauts engineers to automate test cases both for user interfaces and <abbr title="application programming interfaces">APIs</abbr>. I helped setup, and contributed to Playwright tests on the Nayya project.

<!-- omit in toc -->
## <abbr id="toc" title="Table of Contents">TOC</abbr>

* [Timeframe](#timeframe)
* [Background](#background)
* [What To Look At](#what-to-look-at)
* [Run the Code](#run-the-code)
* [Thoughts and Comments](#thoughts-and-comments)
* [Screenshots](#screenshots)
* [Questions](#questions)

## Timeframe

This code was written in Q3 2022.

## Background

Since Nayya (the client for the project where I wrote this code) maintains a staging environment that can be accessed from the web without requiring a password or other authorization, the tests in this codebase can be run against the actual live code in that staging environment.

Caveat, since I haven't maintained these tests beyond the scope of the project, and time has passed, there's no guarantee that these tests will still run, let alone pass. That said, they ran successfully at the time and there are screenshots included to demonstrate, as well as navigable <abbr title="HyperText Markup Language">HTML</abbr> reports that were produced by the tests.

## What To Look At

Not all of the code in this repo is my work. I've added comments to the top of each key file indicating its author(s). If I contributed to the file, but did not write all of the code inside it, I've added comments to the code to indicate which parts I personally wrote.

> ⚠️The easiest way to find my code is to search this repo for the string "Morgan::Playwright::Sample" and click the links in the search results to be taken to the exact files and/or lines of code you should look at.

Here are the specific code samples one should view when evaluating my proficiency with Playwright:

* [`Page` Object Example](some-file#some-line-number)<br>
This file is a `Page` object that I created. `Page` objects are a core building block in Playwright tests. This file represents not just a clean, well-organized `Page` object, but also shows the careful attention paid to documentation, so that the file could be understood and maintained by other members of the Ultranauts team and the client after the end of the project.
* [Linting](eslintrc.json)<br>
In order to make sure everyone who contributes to this repo adheres to a common, clean style, I set up and configured [ESLint](https://eslint.org/).

## Run the Code

0. You must have `git` and `nodejs` installed on your computer
1. From a terminal, clone the repo
2. Navigate to the `playwright-sample/` folder

      <!-- language: lang-sh -->
        cd ultranauts-portfolio/playwright-sample
3. Install dependencies with:

      <!-- language: lang-sh -->
        npm install
4. Run the tests:

      <!-- language: lang-sh -->
        npm test
5. To view the results in a browser, open up the `index.html` file that gets produced by running the tests in the `reports/` folder

## Thoughts and Comments

This was the first project in which I ever used Playwright. I was very impressed with how powerful it was, and how straightforward it was to implement and maintain. Some of the things I appreciated about it most were:

* How easy it was to divide up tasks among team members
* How easy it was for the client to learn and maintain it
* How fast it was. The entire suite could be run within the CI/CD pipeline, with concurrent, parallelized processes, in under a minute

Given the opportunity, I would absolutely recommend Playwright again to a client, and I hope I have the opportunity to work with it again on another project.

It's also important to compare it to [Cypress](https://www.cypress.io/), which is its main competitor in the JavaScript/TypeScript space. Since Microsoft maintains both Playwright and TypeScript, I have much more confidence in Playwright's TypeScript compatibility (i.e. well-formed type definitions). I have more experience with Cypress than with Playwright, and before this project, I would have leaned towards using Cypress in projects. Playwright has a few advantages, though, namely:

* Supports Webkit (engine behind Safari in MacOS, iOS, and iPadOS)
* Faster execution (as of 2022 Oct)
* Emulates mobile devices (more deeply than just mimicking screen resolution)

Cypress, on the other hand, has a default project structure that is built when a new project is generated. Playwright does NOT have a default project structure so teams are left to come up with their own. For the kind of work Ultranauts does, I think Cypress' default structure makes more sense because:

* Documentation/tutorials will all refer to it
* It's easier to teach, since no structural decisions have to be made, i.e. it's one less thing for a team to have to discuss and figure out
* A standardized project structure means it is battle tested and conforms to what will work for the vast majority of situations
* Since both Ultranauts teams and clients will likely not spend a ton of time here after the basic project setup, it would be good if there was just one standard project structure used for all projects.

## Screenshots

Below are screenshots demonstrating my code running during the actual project. I've shown examples of both passing tests, and failing results that were reported to the client so that they could be fixed. There is also a screenshot of a chat thread from a <abbr title="pull request">PR</abbr> that I submitted which represents that demonstrates not only my ability to contribute to the project's codebase, but also the care that I put into professional communication with the client's dev team.

![some screenshot](screenshot1.png)

## Questions

If you have any questions about these code samples or about Playwright and/or TypeScript, please reach out to me on Slack, or by email at <a href="mailto:mbenton@ultranauts.co">mbenton@ultranauts.co</a>.
