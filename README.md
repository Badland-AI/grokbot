# Badland Line for Grok Bot

Text your Grok Bot from any phone. Badland Line gives your Bot a number: you text it over SMS and it texts back.

- Works from any phone over SMS. iMessage and group chats are next.
- Send your Bot pictures.
- Invite family or an assistant to text your Bot (Friends & Family and Pro plans).
- Your Bot sees a masked version of a sender's number, never the number itself.

## Install

In Grok Bot, open **Connect apps**, search **Badland**, choose **Add**, and sign in to Badland.
Before the marketplace listing is live you can also say:

> Install this plugin https://github.com/Badland-AI/grokbot then set up Badland Line

## Set up (about two minutes)

1. Your Bot creates one routine, "Badland Line", with a webhook trigger.
2. It sends you a private Badland link. On the Grok Bot desktop app, open that routine's details, copy its webhook URL and
   key, and paste them on the page. The key never passes through the chat.
3. Your Bot gives you a 6-character code. Text it to the Line number from your phone.

From then on, text your Bot like anyone else. Each text starts a run of the routine, which uses your Grok Bot usage.

## What is in this plugin

| Path | Purpose |
| --- | --- |
| `.cursor-plugin/plugin.json`, `mcp.json` | Grok Bot and Cursor: the hosted MCP server at `https://api.badland.ai/api/line/mcp` (OAuth sign-in) |
| `.grok-plugin/plugin.json`, `.mcp.json` | Grok Build catalog manifest |
| `skills/badland-line/SKILL.md` | Setup steps and how to answer texts |

No code runs on your computer or your Bot's computer; everything goes through the hosted server.

## Plans

The plugin is free. Limits come with your Badland plan: see https://badland.ai/line.

## Privacy and SMS terms

Messages are kept for 30 days so your Bot can read recent context, then deleted. They are never sold or used to train AI
models. Only phones that text a pairing code get messages. Reply STOP to opt out, START to opt back in, and HELP for help.
Message and data rates may apply. Details: https://badland.ai/line.

## Support

support@badland.ai

## License

MIT. Badland Line is an independent plugin by Badland. Grok Bot is a product of SpaceXAI and Cursor.
