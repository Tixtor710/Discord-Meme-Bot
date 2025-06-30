# Discord Meme Bot

A simple Discord bot built using Python that fetches and sends memes from the internet when a user types the `$meme` command in a channel.

## Features

- Connects to the Discord API using `discord.py`.
- Fetches random memes using the [meme-api](https://meme-api.com).
- Responds to the `$meme` command with a meme image URL.

## Prerequisites

- Python 3.8+
- A Discord bot token
- The following Python packages:
  - `discord.py`
  - `requests`

## Setup

1. **Clone the repository or create your Python file:**

   ```bash
   git clone <your-repo-url>
   cd <your-project-folder>
   ```

2. **Install dependencies:**

   ```bash
   pip install discord.py requests
   ```

3. **Replace the placeholder token in the code:**

   In the line:

   ```python
   client.run('YOUR_DISCORD_BOT_TOKEN')
   ```

   Replace `'YOUR_DISCORD_BOT_TOKEN'` with your actual Discord bot token.

4. **Run the bot:**

   ```bash
   python your_bot_file.py
   ```

## Usage

In any channel where the bot is present and has permission to read messages and send messages:

```
$meme
```

The bot will respond with a randomly selected meme image URL from the meme-api.

## Note

Ensure that your bot has the **Message Content Intent** enabled in the Discord Developer Portal. You can enable this under the **Bot > Privileged Gateway Intents** section.

## Disclaimer

This project uses the free public [meme-api](https://meme-api.com). Meme availability and quality depend on that service.

## License

This project is licensed under the MIT License.
