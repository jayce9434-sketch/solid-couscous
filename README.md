# Roblox Brain

A lightweight, GitHub/Vercel-ready personal AI chatbot focused on Roblox + Luau coding, memory, image uploads, and code-file export.

## What is included

- Chat mode + Code mode
- Roblox/Luau-focused system behavior
- Editable long-term memory stored locally in the browser
- Automatic local style examples so the assistant can gradually match your energy
- Image attachments for screenshots, Roblox Studio views, errors, etc.
- Streaming responses
- Model selector and reasoning setting
- Dark/light/system themes and compact/comfortable density
- Code block Copy + Save buttons
- Multiple persistent chats
- iPad/mobile-friendly responsive UI
- No API key in frontend source code

## AI setup

This app uses Vercel AI Gateway. Create an AI Gateway API key, then set `AI_GATEWAY_API_KEY` as a Vercel environment variable for Production/Preview/Development. Do not commit the key to GitHub.

The default model is `openai/gpt-6.1-sol`, selected for strong coding and multimodal work. The app also exposes GPT-5.6 Luna, DeepSeek V4.1 Flash, and Claude Sonnet 5.5 in Settings.

## Deploy to Vercel

1. Put this folder in a GitHub repository.
2. Import the repository into Vercel.
3. Add `AI_GATEWAY_API_KEY` in the project environment variables.
4. Deploy.

## Run locally

Node 18+ is enough because the project uses the built-in `fetch`.

```bash
AI_GATEWAY_API_KEY="your-key" npm run dev
```

Then open `http://localhost:3000`.

## GitHub

The project is intentionally dependency-light. You can upload this folder directly to a new GitHub repository. Keep `.env` and credentials out of the repository.

## Personalization

Use the Memory panel for facts you want the bot to remember. The app starts with broad Roblox preferences and can learn communication-style examples locally when Auto-style memory is enabled. Nothing is silently written to the model provider as permanent training data.
