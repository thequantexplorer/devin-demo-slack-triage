# Devin demo: Slack bug report to repro video, Linear ticket and fix PR

**What it shows:** Tag Devin on a customer bug report in Slack. It records a repro, files a Linear ticket with the video, opens a fix PR, and posts the links in the thread.

**Needs:** GitHub, Slack and Linear connected to your Devin org

More demos: [devin-advanced-demos](https://github.com/thequantexplorer/devin-advanced-demos)

## Set it up

1. Click **Use this template → Create a new repository**, choose your GitHub account or org as the owner, and keep the name `devin-demo-slack-triage`. The links and prompt below assume that name. Use the template rather than a fork: pull requests on a fork go to the original repo by default.
2. In Devin, open [**Settings → Connections → GitHub**](https://app.devin.ai/settings/connections/github) and make sure Devin can access the new repository.
3. Connect **Slack** and **Linear** in Devin under **Settings → Connections**.
4. In Slack, create a `#support` channel and run `/invite @Devin` there. Devin ignores mentions in channels it hasn't joined.

## Prompt

Start a new Devin session and paste this. Replace `<you>` with your GitHub user or org, and replace `ETH` with your Linear team key.

```text
Customer report from Dana at Northwind: "On the Acme storefront, if I type a quantity into the cart box instead of using the + button, my cart total goes crazy — I typed 2 for the tent and it charged me for 21 tents!"

@Devin please: reproduce this on https://github.com/<you>/devin-demo-slack-triage, record a video of the repro, file a Linear ticket in team ETH with repro steps, expected vs actual, and the video, then open a fix PR with a regression test and post the ticket + PR links back in this thread.
```

> Post the prompt as a message in `#support` that tags `@Devin`. Don't paste it into the Devin web app.
