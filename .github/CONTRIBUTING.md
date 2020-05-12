# Contributing

<!-- TOC -->

- [1. Contributing](#contributing)
  - [Ways to Contribute](#ways-to-contribute)
    - [Benefits of Contributing](#benefits-of-contributing)
      - [GitHub Profile](#github-profile)
      - [LinkedIn](#linkedin)
      - [Credibility](#credibility)
  - [Getting Setup](#getting-setup)
    - [Fork the repo](#fork-the-repo)
    - [Installation](#installation)
  - [Questions?](#questions)
    - [GitHub](#github)
    - [Slack](#slack)
    - [Email](#email)

<!-- /TOC -->

***
## 1. Contributing

### Ways to Contribute

> If you are new to open source, we recommend reading [GitHub's open source guide](https://opensource.guide/how-to-contribute/) and their [Hello World tutorial](https://guides.github.com/activities/hello-world/).

Feel free to contribute to the Techqueria website in one or more of the following ways and thank you for being willing to help out! 😊

- Tackle any of the [open issues](https://github.com/techqueria/casa-jobs/issues) that are labeled `help wanted`, `good first issue` or `bug`.
  - If an issue has the label `in progress`, someone is already working on it.
  - If an issue has the label `admin`, an admin probably needs to get involved since it requires admin access.
  - **Even if an issue has someone assigned, it still might need extra help so check it out if it appeals to you!**
- [Open a new issue](https://github.com/techqueria/casa-jobs/issues/new/choose)
- [Report a bug](https://github.com/techqueria/casa-jobs/issues/new?assignees=KGmajor&labels=bug&template=bug_report.md&title=%5BBUG%5D)
- [Request a new feature](https://github.com/techqueria/casa-jobs/issues/new?assignees=&labels=enhancement&template=feature_request.md&title=%5BFeature+Request%5D)
- Improve our [contributing guidelines](https://github.com/techqueria/casa-jobs/blob/master/.github/CONTRIBUTING.md) (this file) or other documentation
- Fix typos or grammar errors on pages or across the code base
- Refactor code
- Anything else you can think of! 😆

#### Benefits of Contributing

##### GitHub Profile

You can ask to be added to our GitHub organization.

After you are added to our Techqueria GitHub organization as a contributor, you can let the world know you've helped us by displaying our organization avatar on your GitHub profile (see screenshot below).

![GitHub Organizations](https://i.imgur.com/DpZcMFl.jpg)

By default, this is made private but you [can easily make it public.](https://help.github.com/en/articles/publicizing-or-hiding-organization-membership).

##### LinkedIn

Showcase your contributions through LinkedIn with Techqueria's company profile: https://linkedin.com/company/techqueria.

Just make sure to use the description below and you can briefly describe what you did as well.

```txt
Techqueria is a 501c3 nonprofit serving the largest community for Latinx in Tech.

- Contributed to their open source website through translations and bug fixes
```

Here's an example of how that can be done by posting under "Experience" or "Volunteering" on your LinkedIn profile.

![LinkedIn Contributions](https://i.imgur.com/t01auIB.jpg)

##### Credibility

- You can tell people you've contributed to an open source project - [not that many developers do](https://www.digitalocean.com/currents/october-2018/)!
- You can tell people you have contributed to the largest community for Latinx in Tech

> And there are [many more reasons](https://opensource.guide/how-to-contribute/) why contributing to open source is great!
***
## Getting Setup
### Fork the repo

[Fork](https://github.com/techqueria/casa-jobs#fork-destination-box) this repository by using the "Fork" button at the top right corner of the repo, right next to "star"! This brings a copy of this repository into your profile, without changing any of the original project.

Connect your local to the original "upstream" repository by adding it as [a remote](https://help.github.com/articles/configuring-a-remote-for-a-fork/).

Pull in changes from "upstream" often so that you stay up to date with master so that when you submit your pull request, merge conflicts will be less likely.

See more detailed instructions through this GitHub article called ["Syncing a Fork"](https://help.github.com/articles/syncing-a-fork/).

Finally, [clone the repo!](https://help.github.com/en/github/getting-started-with-github/fork-a-repo#step-2-create-a-local-clone-of-your-fork)
Hit the green "clone or download" button or
```bash
> git clone https://github.com/techqueria/casa-jobs.git
```

### Install Dependencies

This project relies on [Docker](https://www.docker.com/) to run, please download it to contribute to this project.
<br>
❗You will not need to setup a docker account, just make sure the application is open and running.
<br>
For OSX:
```bash
> brew cask install docker
```

For Windows:
[Check out this Docker site](https://hub.docker.com/editions/community/docker-ce-desktop-windows)

Or check additional instructions for other [operating systems](https://gist.github.com/rstacruz/297fc799f094f55d062b982f7dac9e41)

### Development Environment

#### Startup the server
Spinning up the docker container will simultaneously spin up the backend Flask server and the frontend React app. Use this Docker command in your terminal.
```bash
> docker-compose -f docker-compose.dev.yml up
```
The backend service is hosted on port 5000. Once you've spun up the Docker container, you can confirm that the backend is running by going to `http://locahost:5000/health`. You should see 'ok'.

The frontend service is hosted on port 3000. Again, you'll be able to see this service by going to `http://locahost:3000/`.

❗Sometimes you'll receive a Docker error due to too many containers or dependencies running at a time. Try this command to troubleshoot before reaching out for help.
```bash
> docker system prune
```
## Questions?

If you have any questions, comments, concerns or general feedback, we're happy to help!

### GitHub

Please make a comment mentioning `@techqueria/admins` in your issue or PR and one of us will get back to you ASAP.

### Slack

If you are part of the [Techqueria Slack workspace](https://techqueria.org/slack/), we also have a dedicated `#meta` channel for discussion and a `#meta-website-alerts` for GitHub notifications.

### Email

If needed, there is also the option of contacting us using [https://techqueria.org/contact](https://techqueria.org/contact)
