# Devin demo: Slack bug report to repro video, Linear ticket and fix PR

**What it shows:** Devin working inside the team's existing tools. A customer report in Slack turns into a recorded repro, a Linear ticket with that video, and a fix PR, with every link posted back in the thread.

**Needs:** GitHub, Slack and Linear connected to your Devin org

More demos: [devin-advanced-demos](https://github.com/thequantexplorer/devin-advanced-demos)

## Set it up

1. Click **Use this template → Create a new repository** (or fork it) into your own GitHub account or org.
2. In Devin, open **Settings → Integrations → GitHub** and make sure Devin can access the new repository.
3. Connect **Slack** and **Linear** in Devin's integrations.
4. In Slack, create a `#support` channel and run `/invite @Devin` there. Devin ignores mentions in channels it hasn't joined.

## Prompt

Start a new Devin session and paste this. Replace `<you>` with your GitHub user or org, and replace `ETH` with your Linear team key.

```text
Customer report from Dana at Northwind: "On the Acme storefront, if I type a quantity into the cart box instead of using the + button, my cart total goes crazy — I typed 2 for the tent and it charged me for 21 tents!"

@Devin please: reproduce this on https://github.com/<you>/devin-demo-slack-triage, record a video of the repro, file a Linear ticket in team ETH with repro steps, expected vs actual, and the video, then open a fix PR with a regression test and post the ticket + PR links back in this thread.
```

> Post the prompt as a message in `#support` that tags `@Devin`. Don't paste it into the Devin web app.
