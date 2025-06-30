# Memetty

A simple Discord bot built with Python that fetches and sends memes using a public API.  
Users can type `$meme` in any server the bot is added to, and it'll respond with fresh meme content.

---

## 🚀 Features

- Connects to the Discord API using `discord.py`
- Fetches random memes via the [meme-api](https://meme-api.com)
- Responds to the `$meme` command with a meme image URL
- Hosted and always-on thanks to [Render](https://render.com)
- Invite-ready for any server [→ Invite Link](#-invite-the-bot)

---

## 🧰 Prerequisites

- Python 3.8+
- A [Discord Bot Token](https://discord.com/developers/applications)
- The following Python packages:
  - `discord.py`
  - `requests`
  - `python-dotenv` (for token management)

---

## 🔧 Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Tixtor710/Discord-Meme-Bot.git
cd Discord-Meme-Bot
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

> If you're developing locally, ensure you have:
> ```bash
> pip install python-dotenv
> ```

---

### 3. Create a `.env` File

In the root directory, create a file named `.env`:

```env
DISCORD_TOKEN=your_real_discord_bot_token_here
```

---

### 4. Run the Bot

```bash
python bot.py
```

> You should see:
> `Logged on as Memetty#1234!`

---

## 💬 Usage

In any Discord server where the bot is present and has permission to **read** and **send** messages:

```bash
$meme
```

The bot will fetch and reply with a random meme image URL.

---

## 🌐 Deploy to Render (Optional but Recommended)

To host the bot 24/7:

1. [Create a Render account](https://render.com)
2. Create a new **Web Service** from your GitHub repo
3. Use the following settings:

| Setting            | Value                            |
|--------------------|----------------------------------|
| Build Command      | `pip install -r requirements.txt`|
| Start Command      | `python bot.py`                  |
| Environment Var    | `DISCORD_TOKEN=your_token_here`  |

4. That’s it. Render auto-deploys on each `git push`.

---

## 🔗 Invite the Bot

Want to use this bot in your server?  
[👉 Click here to invite](https://discord.com/oauth2/authorize?client_id=1389285548019027968&permissions=2147731520&integration_type=0&scope=bot)

---

## ⚠️ Important Notes

- Enable the **"Message Content Intent"** for your bot in the [Discord Developer Portal](https://discord.com/developers/applications) →  
  **Bot > Privileged Gateway Intents**
- Ensure your bot has the following **permissions** in each server:
  - ✅ Send Messages
  - ✅ Read Message History
  - ✅ Embed Links
  - ✅ Use Slash Commands (optional for future upgrade)

---

## 📜 License

This project is licensed under the MIT License.

---

## 🧠 Credits

- Built by [Robin Robert](https://github.com/Tixtor710)
- Meme content sourced from [meme-api.com](https://meme-api.com)