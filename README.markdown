# TextTickler Chrome Extension

A fun, AI-powered writing buddy that tickles your text into shape live in the browser using OpenRouter's API. Requires an OpenRouter API key.

## Features
- **Shortcuts**: Type `[prefix]xedit`, `[prefix]xreword`, `[prefix]xexplain`, or `[prefix]xsummarize` in any text area to process the preceding text inline (default prefix: `/`, customizable in options).
- **Context Menu**: Right-click selected text to edit, reword, explain, or summarize, replacing the text directly.
- **Tone Adjustment**: Choose from Neutral, Formal, Casual, or Friendly tones to modify AI output.
- **Custom Prompts**: Tailor instructions for each command (e.g., academic edits, concise rephrasing, kid-friendly explanations, bullet-point summaries).
- **Custom Shortcut Prefix**: Set your preferred shortcut prefix (e.g., `/`, `#`) in the options page.
- **Flexible Model Selection**: Choose from predefined OpenRouter models (GPT-4o, Claude 3.5 Sonnet, LLaMA 3.1 70B, Mixtral 8x7B) or specify a custom model ID from OpenRouter’s model list.
- **API-Only**: Uses OpenRouter API to access a wide range of AI models.
- **Feedback**: Plays a click sound and shows a "Text Updated!" notification when text is replaced.

## Usage
- **Shortcuts**: Type `This is good /xreword` in a text area (or `#xreword` if prefix changed). Text is replaced (e.g., academic edit, concise rephrase), with click sound and "Text Updated!" notification.
- **Context Menu**: Right-click selected text, choose Edit, Reword, Explain, or Summarize.
- **Custom Model**: In options, enter a custom model ID (e.g., `mistralai/mixtral-8x22b-instruct`) to use any OpenRouter model, overriding the dropdown.
- **Options**: Customize prefix, tone, prompts, or model.

## Notes
- **API Key**: Get an OpenRouter API key from [openrouter.ai](https://openrouter.ai). Models like Claude and LLaMA are accessible via OpenRouter.
- **Custom Model**: Ensure the custom model ID matches OpenRouter’s format exactly (see [openrouter.ai/models](https://openrouter.ai/models)). Invalid IDs may cause API errors.
- **Troubleshooting**:
  - Shortcuts fail? Check prefix, API key, model ID, console (`F12`).
