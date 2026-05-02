# Agent Trace

A lightweight, client-side viewer for coding-agent session transcripts. Paste or drop a JSONL file from  one of your coding agent sessions, e.g., [Codex](https://github.com/openai/codex) or [Claude Code](https://claude.com/claude-code) and read the run as a conversation.                  
  **Live:** https://shekkizh.github.io/jsonl-viewer/ *(or wherever you host it)*                                                                                                                                               

## Features              
- **Auto-detects** the Codex (`type: session_meta` / `response_item`) vs. Claude Code (`uuid` + `sessionId`) JSONL layout.                                                                                                                        
- **Readable conversation** rendering: user, assistant, tool / shell, thinking, and system events each get their own accent.
- **Tool call pairing** — shell commands, file edits, sub-agents, and patch applies are grouped with their outputs.                                                                                                                               
- **Smart collapsing** — long outputs (>500 chars or >8 lines) fold behind a disclosure so the timeline stays scannable.                                                                                                                          
- **Noise controls** — header toggles to hide thinking, system prompts, or meta events.                                                                                                                                                           
- **Upload or paste** — drag a `.jsonl` file anywhere on the page, click *Upload file…*, or paste into the textarea.                                                                                                                             
- **Client-side only** — no server, no analytics, nothing leaves your browser. Save the page and it works offline.
----                                                                                                              
## Privacy                                                                                                                                                                                                                      
The transcript never leaves your browser. There's no server and no analytics. The only external request is to fonts.googleapis.com for the two webfonts on first load — if you want to remove even that, vendor the fonts or strip the <link> and the font-family fallbacks will take over.                                                                                                                                                                                                      
## License                                                                                                                                                                                                                      
MIT.
                        
