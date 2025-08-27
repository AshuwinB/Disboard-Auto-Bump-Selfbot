# Auto-Bump

A simple Discord selfbot script to automatically send `/bump` commands at random intervals in a specified channel.

## Features

- Automatically bumps a Discord server using the `!d bump` command.
- Randomized interval between bumps (2 to 2.5 hours).
- Uses environment variables for configuration.

## Requirements

- Node.js (v16 or higher recommended)
- Discord account
- `discord.js-selfbot-v13` package

## Setup

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/auto-bump.git
   cd auto-bump
   ```

2. **Install dependencies:**
   ```sh
   npm install
   ```

3. **Configure environment variables:**
   - Copy `.env.example` to `.env`:
     ```sh
     cp .env.example .env
     ```
   - Fill in your Discord token and bump channel ID in `.env`:
     ```
     TOKEN=your_discord_token
     BUMP_CHANNEL=your_channel_id
     ```

4. **Run the bot:**
   ```sh
   node index.js
   ```

## Environment Variables

- `TOKEN`: Your Discord account token.
- `BUMP_CHANNEL`: The ID of the channel where the bump command should be sent.

## Notes

- This script uses a selfbot, which is against Discord's Terms of Service. Use at your own risk.
- Do **not** commit your `.env` file. Use `.env.example` for sharing variable names.

## License

MIT
