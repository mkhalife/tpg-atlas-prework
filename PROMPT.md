Help me with the TPG Atlas pre-work. TPG Atlas is a shared brain for how TPG works: strategy, OKRs, what already exists, research, the design system, metric definitions, and past learnings. The pre-work collects real tasks and the specific questions behind them, so Atlas can be built from what people actually needed and tested against it. It takes about 10 minutes. No name, email, title, or dates are sent, though the tasks themselves may make it clear whose they are. Nothing is sent until I approve the exact rows and click Send myself.

Work from my own history. Read it here; never send, quote, or save a transcript.

First, work out which of these you are, from what you can do here, and follow the steps marked for it:
- CODE: you can run shell commands on my computer (Claude Code in a terminal or Claude Desktop's Code tab, or Codex in the ChatGPT desktop app).
- CLOUD: you are a claude.ai/code session with list_sessions but no access to my computer.
- CHAT: you are Claude in a chat (the Claude app or claude.ai) and cannot run shell commands.

How to ask me things: whenever you need an answer from me (steps 1, 4 and 6), use your tool for asking the user a question, such as AskUserQuestion, so it shows as a card I answer. Give two to four short example answers as options; I can always type my own. If you have no such tool, ask one question per message, put the question in bold on its own line, and write nothing after it. Never bury a question in the middle of an update.

1. Ask me which group I am in: PM, Design, Research, Engineering, or Other. Remember the answer as my function.

2. Read my AI history from the last 45 days.
   - CODE: Claude Code transcripts in ~/.claude/projects, Cowork sessions in Claude Desktop's local-agent-mode-sessions folder, Codex sessions in ~/.codex. Skip any you cannot reach; do not ask.
   - CLOUD: list_sessions, then read the relevant sessions.
   - CHAT: use your chat history tools (recent_chats, conversation search) to list my chats from the last 45 days and read the relevant ones. If you have none, say so in one line and go straight to step 4.
   Keep only TPG work: specs, PRDs, designs, research plans, analyses, decks, tickets, launch or experiment work. Skip personal chats and pure coding chores. Read each kept session or chat whole, not just its first message. While you read, you may start step 4 so I am not waiting.

3. Draft task records. Size each task to one deliverable or one decision: split a long project into the step where TPG context mattered most. Keep up to 10, chosen for variety of work type and for how much TPG context they needed, and list any others you found by title only, so I can pull one in. Each record has these fields:
   - task: one or two sentences describing the work in general terms, as someone else could repeat it. Name TPG products (AskTPG, CardMatch, the homepage) where they matter; name no people.
   - work_type: one of spec, design, research, analysis, deck, ticket, other.
   - questions: two to four specific questions about TPG that the task needed answered, worded the way I would actually type them to an AI. Each is later asked of an AI and the reply scored against the answer, so keep both concrete. For each: question; answer, if I know it: the one to three facts a correct reply must include, specific enough to check (a definition, a number, a rule, a named doc or dashboard), else empty, and only facts any TPG employee may see; answer_lives_in, the doc, Slack channel, dashboard, or role or team that has the answer or should have had it, else empty, never a person's name. Example: {"question":"What counts as an active newsletter subscriber?","answer":"","answer_lives_in":"Data team; newsletter dashboard"}.
   - context_needed: the one or two categories that mattered most, from: Strategy and priorities; OKRs and KRs; Metric definitions and data; User research; Design system and brand; What already exists; Who owns what; Past tests and decisions; How TPG makes money; Compliance and partner rules; Platform and technical limits; Other (say what).
   - context_found: all, some, or none.
   - where_found: any of doc, Slack, a person, a dashboard, my memory, not found.
   - missing: one line on what was missing or hard to find. Empty if nothing.
   - good_result: three to five short bullets on the TPG facts, constraints, and decisions a good result has to get right, each concrete enough that a reviewer could mark it present or missing. Leave out how I like things written or formatted and how I like to work.
   - must_not: optional, one line on what a good result must not get wrong.
   - ai_helped: yes, partly, no, or not used.
   - origin: mined.

4. Interview me, one question at a time, and turn each answer into a record with origin: interview. Ask:
   a. A task from the last month where AI did not help, or made it worse. What was it, and what was missing?
   b. A task you did without AI at all. What did it need from TPG?
   c. Something you had to ask a person for because it was not written down anywhere.
   Fill the same fields from my answers, including two to four questions. If I have not said which doc, channel, or role should have had an answer, ask that as one short follow-up (optional; a role or channel, not a person). Otherwise ask a follow-up only when a field would otherwise be empty. If I share a link (a doc, a Slack thread), you may read it to understand my answer; summarize what it tells you in your own words, and never copy content from a private channel, DM, or restricted doc into a record.

5. Check every record before showing it to me, and fix anything that fails:
   - No people's names, emails, Slack handles, or anything that identifies a person.
   - No partner or issuer deal terms, revenue or P&L figures, salaries, performance or HR details, customer data, or content from private channels, DMs, or restricted docs.
   - No quotes from my sessions.
   - Answers in questions are facts any TPG employee may see.
   Product names, public TPG facts, team names, and public channel names are fine.

6. Show me every record, numbered, as a compact table followed by each record's questions. Then ask me, as a card: send these, or change something first? I can edit any field, drop or add a record, or pull in one of the titles you listed. Apply my changes and ask again until I choose send. If I decline, stop and delete any working files.

7. On send, make a random 12-character lowercase hex submission id (0-9, a-f only) and build this JSON, with good_result, context_needed, and where_found as arrays of strings and questions as an array of objects:
   {"key":"f2ec6d2c268baa80708eee5b7a7c39ee","schema_version":2,"submission_id":"<id>","function":"<my function>","records":[<the records>]}
   - CODE and CLOUD: encode it as UTF-8, then base64url without padding (replace + with -, / with _, strip =). The send link is https://script.google.com/a/macros/redventures.com/s/AKfycbzHckYTwaeDFYck6qBRACFxmpzqUquhOR0SXkFQUEh-g5fBk0ykep952olnZ_UMy0_OLg/exec#<encoded JSON>. Open it in my browser with `open` on macOS, `start ""` on Windows, or `xdg-open` on Linux; if you cannot open a browser from here, print the link and tell me to open it. Then delete your working files.
   - CHAT: print the JSON as one code block. Tell me to copy it, open https://script.google.com/a/macros/redventures.com/s/AKfycbzHckYTwaeDFYck6qBRACFxmpzqUquhOR0SXkFQUEh-g5fBk0ykep952olnZ_UMy0_OLg/exec#paste and paste it into the box there.
   Then tell me: the page shows my tasks, I can untick any, and nothing is sent until I click Send there. It asks me to be signed in to my Red Ventures Google account; it does not record who I am. If none of this works, show me the final records as plain text and send me to the form instead: https://docs.google.com/forms/d/e/1FAIpQLSfs6SsFqalXUld2bTiuxVdE8XPv4hoOpuArCydnvkyQEKwlhw/viewform
