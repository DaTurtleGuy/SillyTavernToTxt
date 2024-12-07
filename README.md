# SillyTavern Chat Exporter

A simple web tool to convert your SillyTavern chat logs into plain text files suitable for sharing or using with Large Language Models (LLMs).

## Try It Out:

**hold on i gotta deploy it first**

## Features:

- Converts SillyTavern JSONL chat logs to plain text.
- Cleans up extra whitespace and newlines for better readability.
- Standardizes characters (e.g., smart quotes, dashes) for LLM compatibility.
- Provides information about the chat (number of messages, characters involved).
- Downloads the converted chat as a `.txt` file.

## How It Works:

The tool uses JavaScript to parse the uploaded chat file, extract messages and character names, perform text cleanup and standardization, and then format the output into a plain text string. The cleaned text is then offered as a downloadable `.txt` file.

**Technical Details (optional - for developers or curious users):**

- JSONL parsing: Uses the `FileReader` API and `JSON.parse()`.
- Text Cleanup: Employs regular expressions to remove excessive whitespace and normalize newlines.
- Character Standardization: Replaces smart quotes, dashes, and some Cyrillic characters with their standard ASCII equivalents using Unicode normalization.
- File Download: Uses the `Blob` API and a dynamically created `<a>` tag to trigger the download.

## Usage:

1. Open the web tool in your browser.
2. Click "Select your chat file" and choose your SillyTavern JSON/JSONL log file.
3. The tool will parse the file and display some information about the chat.
4. It will automatically download your `.txt` file


## Limitations:

- Only supports SillyTavern JSONL chat logs.
- Is a piece of shit i made in 10 minutes cause i dont wanna go to the pc every damn time i want to convert a chat :wink:


## License:

Do What The Fuck You Want To Public License. See [LICENSE](LICENSE) for details.

