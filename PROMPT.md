Help me with the TPG Atlas pre-work. TPG Atlas is a shared brain for how TPG works: strategy, OKRs, what already exists, research, the design system, metric definitions, and past learnings. The pre-work collects real tasks from people's work so Atlas can be built and tested against them. It takes about 10 minutes. My submission is anonymous: no name, email, title, or dates are sent, and nothing is sent until I approve the exact rows and click Send myself.

Work from my own history. Read it here; never send, quote, or save a transcript.

First, work out which of these you are, from what you can do here, and follow the steps marked for it:
- CODE: you can run shell commands on my computer (Claude Code in a terminal or Claude Desktop's Code tab, or Codex in the ChatGPT desktop app).
- CLOUD: you are a claude.ai/code session with list_sessions but no access to my computer.
- CHAT: you are Claude in a chat (the Claude app or claude.ai) and cannot run shell commands.

1. Ask me one question: which group am I in? PM, Design, Research, Engineering, or Other. Remember the answer as my function.

2. Read my AI history from the last 45 days.
   - CODE: Claude Code transcripts in ~/.claude/projects, Cowork sessions in Claude Desktop's local-agent-mode-sessions folder, Codex sessions in ~/.codex. Skip any you cannot reach; do not ask.
   - CLOUD: list_sessions, then read the relevant sessions.
   - CHAT: use your chat history tools (recent_chats, conversation search) to list my chats from the last 45 days and read the relevant ones. If you have none, say so in one line and go straight to step 4.
   Keep only TPG work: specs, PRDs, designs, research plans, analyses, decks, tickets, launch or experiment work. Skip personal chats and pure coding chores. Read each kept session or chat whole, not just its first message.

3. Draft 5 to 8 task records, picking the tasks where TPG business context mattered most. Each record has these fields:
   - task: one or two sentences describing the work in general terms, as someone else could repeat it. Name TPG products (AskTPG, CardMatch, the homepage) where they matter; name no people.
   - work_type: one of spec, design, research, analysis, deck, ticket, other.
   - context_needed: every category the task depended on, from this list: Strategy and priorities; OKRs and KRs; Metric definitions and data; User research; Design system and brand; What already exists; Who owns what; Past tests and decisions; How TPG makes money; Compliance and partner rules; Platform and technical limits; Other (say what).
   - context_found: all, some, or none.
   - where_found: any of doc, Slack, a person, a dashboard, my memory, not found.
   - missing: one line on what was missing or hard to find. Empty if nothing.
   - good_result: three to five short bullets on what a good result for this task contains.
   - must_not: optional, one line on what a good result must not do.
   - ai_helped: yes, partly, no, or not used.
   - origin: mined.

4. Interview me, one question at a time, and turn each answer into a record with origin: interview. Ask:
   a. A task from the last month where AI did not help, or made it worse. What was it, and what was missing?
   b. A task you did without AI at all. What did it need from TPG?
   c. Something you had to ask a person for because it was not written down anywhere.
   Fill the same fields from my answers; ask a short follow-up only when a field would otherwise be empty.

5. Check every record before showing it to me, and fix anything that fails:
   - No people's names, emails, Slack handles, or anything that identifies me, my team, or my manager.
   - No partner or issuer deal terms, revenue or P&L figures, salaries, performance or HR details, customer data, or content from private channels or DMs.
   - No quotes from my sessions.
   Product names and public TPG facts are fine.

6. Show me every record in one table, numbered. Tell me I can edit any field, drop any record, or add one. Apply my changes, then show the final table and ask: ready to send these N records? Wait for a clear yes. If I decline, stop and delete any working files.

7. On yes, make a random 12-character lowercase hex submission id (0-9, a-f only) and build this JSON, with good_result, context_needed, and where_found as arrays of strings:
   {"key":"f2ec6d2c268baa80708eee5b7a7c39ee","schema_version":1,"submission_id":"<id>","function":"<my function>","records":[<the records>]}
   - CODE and CLOUD: encode it as UTF-8, then base64url without padding (replace + with -, / with _, strip =). The send link is https://script.google.com/a/macros/redventures.com/s/AKfycbzHckYTwaeDFYck6qBRACFxmpzqUquhOR0SXkFQUEh-g5fBk0ykep952olnZ_UMy0_OLg/exec#<encoded JSON>. Open it in my browser with `open` on macOS, `start ""` on Windows, or `xdg-open` on Linux; if you cannot open a browser from here, print the link and tell me to open it. Then delete your working files.
   - CHAT: print the JSON as one code block. Tell me to copy it, open https://script.google.com/a/macros/redventures.com/s/AKfycbzHckYTwaeDFYck6qBRACFxmpzqUquhOR0SXkFQUEh-g5fBk0ykep952olnZ_UMy0_OLg/exec#paste and paste it into the box there.
   Then tell me: the page shows my tasks, I can untick any, and nothing is sent until I click Send there. It asks me to be signed in to my Red Ventures Google account; it does not record who I am. If none of this works, show me the final table as plain text and send me to the form instead: https://docs.google.com/forms/d/e/1FAIpQLSfs6SsFqalXUld2bTiuxVdE8XPv4hoOpuArCydnvkyQEKwlhw/viewform
