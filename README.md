# Telegram Image Bot

This is a Telegram bot that allows users to search for and retrieve images from Unsplash and Pexels using simple text commands.

## Features
- Fetch images from **Unsplash** and **Pexels** APIs.
- Simple user interface for searching images directly through Telegram messages.
- Support for querying specific topics and specifying the number of images to retrieve.

## Prerequisites
Before running the bot, ensure you have the following:

1. **Telegram Bot Token**: Obtain this by creating a bot via the [BotFather](https://core.telegram.org/bots#botfather).
2. **Unsplash API Key**: Create an account and generate an API key from [Unsplash Developers](https://unsplash.com/developers).
3. **Pexels API Key**: Create an account and get an API key from [Pexels API](https://www.pexels.com/api/).

## Installation

1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd <repository-name>
    ```

2. Install dependencies:
    ```bash
    pip install python-telegram-bot requests
    ```

3. Create a `.env` file (optional) to store your API keys securely:
    ```env
    TOKEN=Your_Telegram_Bot_Token
    UNSPLASH_API_KEY=Your_Unsplash_API_Key
    PEXELS_API_KEY=Your_Pexels_API_Key
    ```

4. Replace the placeholders `Your token telegram`, `Any API use for search Image`, and `Any API use for search Image` in the code with your actual API keys.

## Usage

1. Start the bot:
    ```bash
    python bot.py
    ```

2. Open your bot on Telegram and use the `/start` command to see the instructions.

3. To search for images, send a message in the following format:
    ```
    source,query,count
    ```
   - `source`: The image source, either `unsplash` or `pexels`.
   - `query`: The topic or keyword for the image search (e.g., `nature`, `animals`).
   - `count`: The number of images to retrieve.

   Example:
   ```
   unsplash,nature,3
   ```

4. The bot will fetch the images and send them back to you.

## Example Commands
- **Start Command:**
    ```
    /start
    ```
    Displays instructions on how to use the bot.

- **Search Command:**
    ```
    unsplash,cats,5
    ```
    Fetches 5 images related to `cats` from Unsplash.

    ```
    pexels,dogs,3
    ```
    Fetches 3 images related to `dogs` from Pexels.

## Error Handling
- The bot will notify you if:
  - The input format is incorrect.
  - The specified source is invalid.
  - No images are found for the query.

## File Structure
```
.
├── bot.py             # Main bot code
├── README.md          # Project documentation
└── requirements.txt   # Dependencies for the project
```

## Dependencies
- `python-telegram-bot`
- `requests`

Install all dependencies with:
```bash
pip install -r requirements.txt
```

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Contributions
Feel free to fork this repository and submit pull requests for any improvements or additional features.

---

Enjoy using the Telegram Image Bot!

