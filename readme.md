# Telegram PR Notifier

This GitHub Action sends a message to a Telegram group whenever a new Pull Request is opened. You can target either the main group chat or a specific topic (thread) if your group has topics enabled.

```

+------------------------+      +---------------------------+
\|  Regular Telegram Chat | <--> |  Message in main thread   |
+------------------------+      +---------------------------+

+------------------------+      +---------------------------+
\| Group with Topics ON   | <--> | Message in specific topic |
+------------------------+      +---------------------------+

```

To set up: [1] Create a Telegram bot via @BotFather and add it to your group, [2] collect the bot token, group chat ID (`-100...`), and optional topic ID, then [3] store them in GitHub Secrets as `TELEGRAM_BOT_TOKEN`, `TELEGRAM_CHAT_ID`, and (optionally) `TELEGRAM_THREAD_ID`.
