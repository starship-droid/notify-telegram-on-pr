# Notify Telegram on New Pull Request

        ┌────────────┐
        │  GitHub PR │
        └─────┬──────┘
              │
              ▼
      ┌────────────────┐
      │  Telegram Bot  │
      └────────────────┘

Automatically sends a Telegram message whenever a new **Pull Request is opened** in your GitHub repository.

🔧 **Setup Instructions**
1. Add these secrets to your GitHub repo:
   - `TELEGRAM_BOT_TOKEN` → Bot token from [@BotFather](https://t.me/BotFather)
   - `TELEGRAM_CHAT_ID`   → Your chat/group ID
   - `TELEGRAM_THREAD_ID` → (Optional) Thread ID for topics in groups

2. Drop this workflow in `.github/workflows/notify-pr.yml`.

📬 Message Format:
```

New PR by <author>: *<title>*
Link: <URL>

```

💡 Uses Markdown formatting and supports threads for organized notifications.
