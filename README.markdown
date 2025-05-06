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

## Installation
1. **Create the Folder**:
   - Create a folder named `text-tickler`.
   - Save files: `manifest.json`, `background.js`, `content.js`, `options.html`, `options.js`, `options.css`, `click.mp3`.
   - Add icons: `icon48.png` (48x48), `icon128.png` (128x128) from [Flaticon](https://www.flaticon.com) or create with [Canva](https://www.canva.com).

2. **Add Click Sound**:
   - Download a royalty-free click sound (MP3, <100KB) from [Freesound](https://freesound.org) or [Mixkit](https://mixkit.co/free-sound-effects/click/).
   - Save as `click.mp3` in `text-tickler`.

3. **Load Extension**:
   - Open Chrome, go to `chrome://extensions/`.
   - Enable "Developer mode".
   - Click "Load unpacked", select `text-tickler`.

4. **Configure Settings**:
   - Open options page (right-click extension icon > "Options").
   - Select an OpenRouter model (e.g., OpenAI GPT-4o, Claude 3.5 Sonnet).
   - Enter your OpenRouter API key from [openrouter.ai](https://openrouter.ai).
   - Set shortcut prefix (e.g., `/`, `#`).
   - Save settings.

## Usage
- **Shortcuts**: Type `This is good /xreword` in a text area (or `#xreword` if prefix changed). Text is replaced, with click sound and "Text Updated!" notification.
- **Context Menu**: Right-click selected text, choose Edit, Reword, Explain, or Summarize.
- **Options**: Customize prefix, tone, or prompts.

## Notes
- **API Key**: Get an OpenRouter API key from [openrouter.ai](https://openrouter.ai). Models like Claude and LLaMA are accessible via OpenRouter.
- **Troubleshooting**:
  - Shortcuts fail? Check prefix, API key, console (`F12`).
  - No notification? Verify `click.mp3`, check console for errors.