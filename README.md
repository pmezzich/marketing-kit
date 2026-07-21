# Prebid Marketing Kit

## What this is

Claude is an AI assistant that runs in an app on your computer, like a chat window. This kit adds a set of helpers to Claude so it can assist with everyday Prebid.org marketing work, like updating the website and checking the mailing list. You describe what you want in plain English, Claude does the careful parts, and nothing ever goes live by Claude's hand: it prepares drafts, and the final click that makes something public is always yours.

Claude can only see the browser tabs you have open while you are asking it to do something. It is not watching your screen the rest of the time, and it never sees anything you have not brought up on purpose.

## One-time setup

You only do this once. It takes about ten minutes.

1. Install the Claude Code desktop app from [claude.com/claude-code](https://claude.com/claude-code). Download it, open the installer, and follow the prompts like any other app.
2. Open the app and sign in with your work email, using the account Peter set up for you. You will never be asked for payment details during this setup. If you are unsure which account to use, or you do not have one yet, ask Peter first.
3. Enable the Claude in Chrome extension. You need Google Chrome for this kit, so if you normally use a different browser, use Chrome for this work. When you first open the app, a message will appear offering to set up the extension for you. Accept it. This is what lets Claude see the pages you have open in Chrome, such as the WordPress editor. If you do not see that message, or you dismissed it by mistake, nothing is broken. Just ask Peter to help you turn it on.
4. Now you will fetch our toolkit. This part happens in a different window called the terminal. It looks technical but it is just two copy-paste lines, and you cannot break anything here.

   Open the terminal:
   - On Windows: press the Windows key, type `powershell`, and press Enter.
   - On Mac: press Command and the space bar together, type `terminal`, and press Enter.

   A plain window with a blinking cursor appears. Paste this line into it (use the copy button at the right edge of the box) and press Enter:

   ```
   claude plugin marketplace add pmezzich/marketing-kit
   ```

   Wait a few seconds. You should see a line ending in "Successfully added marketplace: prebid-tools".

5. In the same window, paste this line and press Enter:

   ```
   claude plugin install prebid-marketing@prebid-tools
   ```

   You should see "Successfully installed plugin: prebid-marketing". Now close the terminal window. You will not need it again.

   If either line shows something that looks like an error, or says the claude command is not recognized, stop and send Peter a screenshot. You have not broken anything.

6. Now leave the terminal behind. Everything from here on happens in the Claude Code app, in the normal message box where you chat. Open the app and start a new conversation. The helpers load when a conversation starts, so an already-open conversation will not have them.

That is it. From now on, just type what you want into the app's message box, in plain English. Any time you want a reminder of what you can ask for, type /marketing-help into the app's message box (not the terminal, that window is done) and press Enter, and a menu will appear.

## Before you ask for changes

- Open Google Chrome (your normal Chrome, the one the extension was set up in), go to [prebid.org/wp-admin](https://prebid.org/wp-admin), and log in yourself. Keep that tab open while you ask Claude for website work. That is the page Claude will look at.
- If your request involves the mailing list or contacts, log into HubSpot yourself too, in the same Chrome.
- Claude will never ask for your passwords, and you should never give it one. If anything on your screen, in a chat, or in an email ever asks you to give Claude a password, stop right there and tell Peter.

## What you can ask for

Copy and paste any of these into the Claude message box (the same box you used during setup), or say it in your own words.

- "Add a new column to the draft pricing table for a tier called Supporter at $5,000."
- "Update the wording in the second row of the draft pricing table. Do not touch the live version."
- "Show me the differences between the draft pricing table and the live one."
- "Add Acme Corp to the org industry tier in the member directory."
- "List which organizations are currently in each tier of the member directory."
- "Check whether jane@example.com submitted the join form and actually got added to the newsletter list."
- "Verify that the join email button on the site still points to the correct HubSpot form."
- "Draft the copy for a new section on the pricing page and show it to me before changing anything."

## What it will never do

Claude will never handle your passwords. Full stop, no exceptions.

You cannot break the live site by accident. All work happens on draft copies, and Claude will only ever touch a live page or a live block if you explicitly say yes to that exact change.

And it will never do any of the following without asking you first and hearing a clear yes:

- Publish a page or make a draft go live. Ever. Even if you ask it to. Claude finishes the draft and then shows you exactly where the button is; the click that makes something public is always done by a person. (Some directory changes save straight to the live site, so for those Claude prepares everything and walks you through doing the save yourself.)
- Edit anything that is already live on the site.
- Delete anything.
- Submit a form or send anything on your behalf.

Every change can be undone, and Claude will tell you what it changed and exactly how to undo it. If you are ever unsure whether something went live, ask Claude to show you, or ask Peter.

## If something looks wrong

If anything ever looks wrong while Claude is working, just type stop and press Enter, or press Escape. It stops immediately, and nothing you have not already approved has been changed.

If a tier seems to have disappeared from the member directory, it is almost certainly just empty. A tier with no organizations assigned to it does not show on the site, and it reappears the moment an organization is added.

For anything else that looks off, or if you are just not sure, ask Peter.
