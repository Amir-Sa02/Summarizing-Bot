# Summarizing-Bot

## Overview
This project is a **Summarizing Bot** that extracts and summarizes the content of a given webpage. It uses **BeautifulSoup** to scrape text from a webpage and **OpenAI's API** to generate a concise summary, excluding unnecessary navigation-related content.

## Features
- Fetches and extracts text from any given webpage.
- Cleans the extracted text by removing irrelevant elements (scripts, styles, images, inputs).
- Uses OpenAI's GPT-4o-mini model to generate a summary.
- Displays the summary in markdown format.

## Requirements
To use this project, ensure you have the following installed:

- Python 3.7+
- Required Python libraries:
  - `requests`
  - `beautifulsoup4`
  - `python-dotenv`
  - `openai`
  - `IPython`

## Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/your-username/summarizing-bot.git
   cd summarizing-bot
   ```

2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

3. Set up your **.env** file and add your OpenAI API key:
   ```sh
   echo "OPENAI_API_KEY=your_api_key_here" > .env
   ```

## Usage

### Running the Script
1. Import the `Website` class and `summarize` function in your script.
2. Call the `summarize(url)` function with the desired webpage URL.
3. Use `display_summary(url)` to print the summary in markdown format.

Example:
```python
from summarizing_bot import summarize, display_summary

display_summary("https://example.com")
```

### Expected Output
- Extracted webpage title
- Cleaned webpage text
- AI-generated summary of the webpage

## Troubleshooting
If you encounter API key errors:
- Ensure your `.env` file is correctly set up.
- The API key must begin with `sk-proj-`.
- No leading or trailing spaces in the API key.

## License
This project is open-source and available under the **MIT License**.

## Contributions
Contributions are welcome! Feel free to submit issues and pull requests.

## Author
**Your Name**  
GitHub: [your-username](https://github.com/your-username)

