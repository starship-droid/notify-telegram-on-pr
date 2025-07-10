# Telegram PR Notifier

This GitHub Action sends a message to a Telegram chat or group whenever someone opens a Pull Request (PR) on your repository.

It’s designed to be lightweight, easy to fork, and quick to set up. You can use your own Telegram bot or share one.

## Chat vs Topic

The bot can send messages either to a group’s main chat or to a specific topic (thread) inside a group with topics enabled.

```

+----------------+      +-----------------------+
\| Main group chat | <--> | Message without topic |
+----------------+      +-----------------------+

+----------------+      +-----------------------+
\| Group with     |      | Message posted to a   |
\| topics enabled | <--> | specific topic/thread |
+----------------+      +-----------------------+

```

- If you set only `TELEGRAM_CHAT_ID`, messages go to the main group chat.
- If you also set `TELEGRAM_THREAD_ID`, messages go to that specific topic/thread.

Make sure your bot is added to the group and has permission to post where you want the messages.

> Want to use this for your own repo or group? Fork the project and check back soon for setup instructions.