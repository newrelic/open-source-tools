# js-project-template

![GitHub release (latest SemVer including pre-releases)](https://img.shields.io/github/v/release/newrelic/nr1-funnel-component?include_prereleases&sort=semver) [![Snyk](https://snyk.io/test/github/newrelic/nr1-funnel-component/badge.svg)](https://snyk.io/test/github/newrelic/nr1-funnel-component)

Description of the project is here.

## Usage

We have two portions implement this component: a JS and CSS import.

![Screenshot #1](screenshots/screenshot_01.png)

## What problem(s) does this library solve?

- Bullet point sentence giving the user a heads up about what to expect.
- Second bullet focused on a paragraph that might be a good first draft for [developer.newrelic.com](https://developer.newrelic.com) or NPM.

## What do you need to make this work?

1. Requirement #1 (ex. [New Relic Browser agent(s) installed](https://newrelic.com/products/browser-monitoring) and the related access to [New Relic One](https://newrelic.com/platform)).
2. Requirement #2 (if any)

## Getting started

First, ensure that you have [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and [NPM](https://www.npmjs.com/get-npm) installed. If you're unsure whether you have one or both of them installed, run the following command(s) (If you have them installed these commands will return a version number, if not, the commands won't be recognized):

```bash
git --version
npm -v
```

## Installation

Run the following command from within your project.

```
npm install --save https://github.com/newrelic/<js-project-template>.git
```

### CSS
Import the component's CSS into your Nerdlet/artifact's styles.scss or styles.css with the following.

```
# example usage
@import '~@<js-project-template>/<dist-location>/styles.css';
```

### JS
Import the component's into your Nerdlet with the following.

```
# example usage
import { FunnelComponent } from 'nr1-funnel-component';
```

## Development

Start by cloning the repository.

```
git clone https://github.com/newrelic/<js-project-template>.git
cd <js-project-template>
npm install
```

# Open Source License

This project is distributed under the [Apache 2 license](LICENSE).


# Support

New Relic has open-sourced this project. This project is provided AS-IS WITHOUT WARRANTY OR DEDICATED SUPPORT. Issues and contributions should be reported to the project here on GitHub.

We encourage you to bring your experiences and questions to the [Explorers Hub](https://discuss.newrelic.com) where our community members collaborate on solutions and new ideas.

## Community

New Relic hosts and moderates an online forum where customers can interact with New Relic employees as well as other customers to get help and share best practices. Like all official New Relic open source projects, there's a related Community topic in the New Relic Explorers Hub. You can find this project's topic/threads here:

https://discuss.newrelic.com
*(Note: Work with the Community team on this.)*

## Issues / Enhancement Requests

Issues and enhancement requests can be submitted in the [Issues tab of this repository](../../issues). Please search for and review the existing open issues before submitting a new issue.

# Contributing

Contributions are welcome (and if you submit a Enhancement Request, expect to be invited to contribute it yourself :grin:). Please review our [Contributors Guide](CONTRIBUTING.md).

Keep in mind that when you submit your pull request, you'll need to sign the CLA via the click-through using CLA-Assistant. If you'd like to execute our corporate CLA, or if you have any questions, please drop us an email at opensource+js-project-template@newrelic.com.
