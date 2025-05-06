# TextTickler Chrome Extension

A fun, AI-powered writing buddy that tickles your text into shape live in the browser using OpenRouter's API. Requires an OpenRouter API key.

## Features
- **Shortcuts**: Type `[prefix]xedit`, `[prefix]xreword`, `[prefix]xexplain`, or `[prefix]xsummarize` in any text area to process the preceding text inline (default prefix: `/`, customizable in options).
- **Context Menu**: Right-click selected text to edit, reword, explain, or summarize, replacing the text directly.
- **Tone Adjustment**: Choose from Neutral, Formal, Casual, or Friendly tones to modify AI output.
- **Custom Prompts**: Set custom instructions for each command (e.g., "Rephrase for a professional email").
- **Custom Shortcut Prefix**: Set your preferred shortcut prefix (e.g., `/`, `#`) in the options page.
- **API-Only**: Uses OpenRouter API to access models like GPT-4o, Claude 3.5 Sonnet, LLaMA 3.1, and Mixtral.
- **Feedback**: Plays a click sound and shows a "Text Updated!" notification when text is replaced.

## Usage
- **Shortcuts**: Type `This is good /xreword` in a text area (or `#xreword` if prefix changed). Text is replaced, with click sound and "Text Updated!" notification.
- **Context Menu**: Right-click selected text, choose Edit, Reword, Explain, or Summarize.
- **Options**: Customize prefix, tone, or prompts.

## Notes
- **API Key**: Get an OpenRouter API key from [openrouter.ai](https://openrouter.ai). Models like Claude and LLaMA are accessible via OpenRouter.
- **Troubleshooting**:
  - Shortcuts fail? Check prefix, API key, console (`F12`).
  - No notification? Verify `click.mp3`, check console for errors.
