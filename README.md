# Alfred Slack Status manager
Quickly set your status (and do-not-disturb settings) from Alfred

<img width="623" alt="Screenshot of example usage" src="https://user-images.githubusercontent.com/385726/113608480-7bbb3e80-95ff-11eb-9430-b05ebed1c2b0.png" />

## Setup

You will need one of the following:
- A legacy slack token (they no longer generate these, but you might have one still on your account)
- A user token from a slack app you have created (see below section on this)

Set that token in as the `SLACK_TOKEN` workflow variable

## Usage

Type `ss` and space to activate the workflow. You can quickly use the lunch shortcut by typing `ssl`.

## Creating a slack app

If you don't have a legacy token lying around, you can create a slack app to generate a user token for you

- Creat the app: https://api.slack.com/apps?new_app=1
- Add the User Token Scopes: `https://api.slack.com/apps/[your app id goes here]/oauth`
  - You'll need to add `dnd:write` and `users.profile:write`
- Click the 'Install to Workplace' button at the top of the page 
- Copy the token in the box labeled 'User OAuth Token'
