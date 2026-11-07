# Badland Line for Grok Bot

Text your Grok Bot from any phone. Badland Line gives your Bot a number: you text it over SMS and it texts back.

- Works from any phone over SMS. iMessage and group chats are next.
- Send your Bot pictures: it can see them. On Friends & Family and Pro it texts pictures back too.
- Invite family or an assistant to text your Bot (Friends & Family and Pro plans).
- Your Bot sees a masked version of a sender's number, never the number itself.

## Install

Send your Grok Bot this message:

> Install this plugin https://github.com/Badland-AI/grokbot then set up Badland Line

It installs the plugin from this repository and asks you to sign in to Badland. The marketplace listing is still in
review; once it is live you can also add Badland from **Connect apps**.

## Set up (about two minutes)

1. Your Bot creates one routine, "Badland Line", with a webhook trigger.
2. It sends you a private Badland link, good for 6 hours. In Grok Bot, open **Routines**, then **Badland Line**. Under
   **Webhook**, copy **POST to** and **key**, and paste them on the page. The key never passes through the chat.
3. Your Bot gives you a 6-character code. Text it to the Line number from your phone.

From then on, text your Bot like anyone else. Each text starts a run of the routine, which uses your Grok Bot usage.

## If something goes wrong

| What you see | What to do |
| --- | --- |
| The Bot says it cannot find or install the plugin | Send the install message above exactly, including the GitHub link. |
| The Badland link says it expired | Ask your Bot for a new link ("send me a new Badland Line link"). Each one works for 6 hours. |
| The page will not accept the key | Paste the **key** value from the routine's Webhook section, not the URL. `Bearer crsr_…` and the whole `Authorization: Bearer …` line work too. |
| Your texts get no answer | In Grok Bot, open **Routines** and make sure **Badland Line** is turned on, then ask your Bot to check `line_status`. |
| You texted the pairing code too late | Ask your Bot for a new code. A code works for 15 minutes. |
| You want to stop | Text STOP to the Line number, or ask your Bot to disconnect Badland Line. |

Still stuck? Email support@badland.ai.

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

Messages and their pictures are kept for 30 days so your Bot can read recent context, then deleted. They are never sold or used to train AI
models. Only phones that text a pairing code get messages. Reply STOP to opt out, START to opt back in, and HELP for help.
Message and data rates may apply. Details: https://badland.ai/line.

## Support

support@badland.ai

## License

MIT. Badland Line is an independent plugin by Badland. Grok Bot is a product of SpaceXAI and Cursor.
