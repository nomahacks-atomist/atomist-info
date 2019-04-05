# Atomist at NomaHacks

Atomist is a platform for delivery automation from git push to deployment. See [the docs](https://docs.atomist.com/) and [the website](https://atomist.com) for more info.

## What can I do with Atomist?

### 1. Keep posted on project activity, take action in Slack

Use Atomist for Slack notifications about activity on your repos and do useful things, like open and manage issues, raise and merge PRs, and more.

<img width="475" alt="delete-branch" src="https://user-images.githubusercontent.com/7320285/55599210-86d6ed80-570b-11e9-9cc7-7f53efca6223.png">

**How to set this up**

1. Create or join a Slack channel in https://nomahacks.slack.com/
2. `/invite @atomist` to the channel. You'll be prompted to choose a repo to map. This is the repo that you'll get notifications from. 

<img width="430" alt="Screen Shot 2019-04-04 at 21 59 23" src="https://user-images.githubusercontent.com/774714/55604514-058c5480-5725-11e9-9355-4f1835033b64.png">

3. You'll automatically get notifications about repo activity in the channel you selected. You can also run commands. Type `@atomist list skills` in your channel to see a list of commands.

4. The first time you run a command that requires GitHub credentials (like `@atomist create issue`) you will be prompted by the bot in a DM with a message and link to click to authorize your GitHub user (which also links your GitHub ID to your Slack user).


### 2. Write bot commands and bot event listeners

**Commands**

> We have created a starter specifically for developing with the bot. See the [nomahacks-atomist/bot-listener](https://github.com/nomahacks-atomist/bot-listener) repo for details.

See the [docs](https://docs.atomist.com/developer/commands/) on creating and deploying bot commands in the Developer Guide.

**Chat Message formatting and actions**

You have a lot of control to format messages, add actions (commands that show up as native Slack controls like buttons or form elements), and you can send updates to an existing Slack message rather than only appending data.

See the [Chat Messages](https://docs.atomist.com/developer/slack/) part of the Developer Guide.

### 3. Automatically build, test, and deploy node projects to Kubernetes.

<img width="990" alt="Uhura automated delivery" src="https://user-images.githubusercontent.com/7320285/55605944-b7c71a80-572b-11e9-96e8-67374d5ff1ef.png">

If you're developing Node apps and want to deploy them to your own Kubernetes cluster as part of the hackathon, Atomist has built-in support for this, with some constraints on the conventions the Node project needs to follow.

If your project fits this description and you're interested in automated deployment for your app, check out the [Uhura SDM](https://docs.atomist.com/user/uhura/) doc and/or find `@atomist-jim` or `@atomist-ryan` in the NomaHacks Slack.

Happy hacking :zap: :tada:
