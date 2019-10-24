# nr1-template-nerdpack

> This template includes advice on how to craft a great README for your app. This template is just a starting point: feel free to change or add sections to suit your project. Avoid editing the "Open Source License," "Support," "Community," "Issues / Enhancement Requests," and "Contributing" sections. These are required by legal, and the only change you should make is to change the Community URL. 
> 
> Before you publish, ensure you remove all the commments (the block quotes beginning with `>`), and follow the [standard Nerdpack README review process](https://docs.google.com/document/d/1xUg1NnNJriC0mrUE1hqcHcs5dqzyLoSYE25qjwBaWQE/edit). 

![GitHub release (latest SemVer including pre-releases)](https://img.shields.io/github/v/release/newrelic/nr1-template-nerdpack?include_prereleases&sort=semver) [![Snyk](https://snyk.io/test/github/newrelic/nr1-template-nerdpack/badge.svg)](https://snyk.io/test/github/newrelic/nr1-template-nerdpack)

## Usage

> Write one or two short paragraphs that describe what your Nerdpack does—and more importantly, why users should care. Avoid too much technical jargon: Your content should be understandable to someone who doesn't have much knowledge of New Relic's technologies. Include links, too, to New Relic docs or other Nerdpacks. 
> 
> For example:

nr1-browser-analyzer uses the `PageView` events in New Relic to interrogate and categorize the performance of a web site. You can explore the performance of individual pages, and forecast how improving performance impacts KPIs like bounce rate and traffic. This analysis is based on moving individual browsing sessions from `Tolerated` and `Frustrated` into `Satisfied` (as defined by the [`apdex`](https://docs.newrelic.com/docs/apm/new-relic-apm/apdex/apdex-measure-user-satisfaction) value for a given New Relic Browser application).

> You should also include at least one screenshot. Ensure you remove any sensitive data like NR-only tools, customer data, and sensitive data about our systems (for a full list, see [Docs site security guidelines for images](https://newrelic.jiveon.com/docs/DOC-8362) on Jive).

![Screenshot #1](screenshots/screenshot_01.png)
![Screenshot #2](screenshots/screenshot_02.png)

## Open Source License

This project is distributed under the [Apache 2 license](LICENSE).

## What do you need to make this work?

> Describe any prerequisites for using your app. Esure your list is complete, and includes links to other New Relic features when necessary. 
> 
> For example:

Required:

- [New Relic Infrastructure agent(s) installed](https://docs.newrelic.com/docs/agents/manage-apm-agents/installation/install-agent#infra-install) on your cloud computing devices and the related access to [New Relic One](https://newrelic.com/platform).

You'll get the best possible data out of this application if you also:

- [Activate the EC2 integration](https://docs.newrelic.com/docs/integrations/amazon-integrations/get-started/connect-aws-infrastructure) to group by your cloud provider account.
- [Install APM on your applications](https://docs.newrelic.com/docs/agents/manage-apm-agents/installation/install-agent#apm-install) to group by application.

## Getting started

> Include a step-by-step procedure on how to get your app installed and deployed. 

1. First, ensure that you have [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and [NPM](https://www.npmjs.com/get-npm) installed. If you're unsure whether you have one or both of them installed, run the following command(s) (If you have them installed these commands will return a version number, if not, the commands won't be recognized):

```bash
git --version
npm -v
```
2. Next, install the [NR1 CLI](https://one.newrelic.com/launcher/developer-center.launcher) by going to [this link](https://one.newrelic.com/launcher/developer-center.launcher) and following the instructions (5 minutes or less) to install and setup your New Relic development environment.
3. Next, to clone this repository and run the code locally against your New Relic data, execute the following command:

```bash
nr1 nerdpack:clone -r https://github.com/newrelic/nr1-template-nerdpack.git
cd nr1-template-nerdpack
nr1 nerdpack:serve
```

Visit [https://one.newrelic.com/?nerdpacks=local](https://one.newrelic.com/?nerdpacks=local), navigate to the Nerdpack, and :sparkles:

## Deploying this Nerdpack

> Include the necessary steps to deploy your app. Generally, you shouldn't need to change any of these steps. 

Open a command prompt in the nerdpack's directory and run the following commands.

```bash
# If you need to create a new uuid for the account to which you're deploying this Nerdpack, use the following
# nr1 nerdpack:uuid -g [--profile=your_profile_name]
# to see a list of APIkeys / profiles available in your development environment, run nr1 credentials:list
nr1 nerdpack:publish [--profile=your_profile_name]
nr1 nerdpack:deploy [-c [DEV|BETA|STABLE]] [--profile=your_profile_name]
nr1 nerdpack:subscribe [-c [DEV|BETA|STABLE]] [--profile=your_profile_name]
```

Visit [https://one.newrelic.com](https://one.newrelic.com), navigate to the Nerdpack, and :sparkles:

# Support

New Relic has open-sourced this project. This project is provided AS-IS WITHOUT WARRANTY OR SUPPORT, although you can report issues and contribute to the project here on GitHub.

_Please do not report issues with this software to New Relic Global Technical Support._

## Community

> Work with the Explorer's Hub team to create a tag for your app, then update the link below.

New Relic hosts and moderates an online forum where customers can interact with New Relic employees as well as other customers to get help and share best practices. Like all official New Relic open source projects, there's a related Community topic in the New Relic Explorers Hub. You can find this project's topic/threads here:

https://discuss.newrelic.com/t/nr1-template-nerdpack
*(Note: URL subject to change before GA)*

## Issues / Enhancement Requests

Issues and enhancement requests can be submitted in the [Issues tab of this repository](../../issues). Please search for and review the existing open issues before submitting a new issue.

# Contributing

Contributions are welcome (and if you submit a Enhancement Request, expect to be invited to contribute it yourself :grin:). Please review our [Contributors Guide](CONTRIBUTING.md).

Keep in mind that when you submit your pull request, you'll need to sign the CLA via the click-through using CLA-Assistant. If you'd like to execute our corporate CLA, or if you have any questions, please drop us an email at opensource+nr1-template-nerdpack@newrelic.com.
