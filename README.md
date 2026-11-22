# b2b-sales-skills

Nine Agent Skills for Claude and Codex, written for B2B sales teams that qualify deals with MEDDPICC: sellers, sales engineers, sales leaders and customer success. They prepare meetings, write debriefs and recaps, review deals, suggest forecast categories, test champions, prepare QBRs and keep the value map current.

They all work the same way: AI drafts and people decide. The seller writes first and the AI challenges. "Confirmed" means the right person at the customer agreed to a playback or recap, or acted, with the moment to show for it. The AI never moves a deal's stage or forecast category, and anything not discussed stays empty.

The skills use the SKILL.md format read by Claude Code, Claude.ai and Codex: one folder per skill, with YAML frontmatter (`name`, `description`) followed by instructions. For other assistants, use the [prompt pack](PROMPTS.md).

## When to use which

| When | Skill | What it does |
|---|---|---|
| Before a customer meeting | [meeting-prep](skills/meeting-prep/SKILL.md) | You write your 3 whys first; it challenges them, shows what you know per letter and proposes three questions and the ask. |
| The same day | [call-debrief](skills/call-debrief/SKILL.md) | Drafts the evidence per letter in the customer's words, what both sides promised and the next step, for your sign-off. |
| The same day | [what-we-heard](skills/what-we-heard/SKILL.md) | Drafts the recap mail the customer can correct. You send it. |
| The weekly 1:1 | [deal-review](skills/deal-review/SKILL.md) | Scores each letter with the moment behind it, finds the two weakest and asks the questions that test them. |
| Friday forecast | [forecast-category](skills/forecast-category/SKILL.md) | Suggests commit, upside, future or black hole from the evidence, and what would move it. |
| Before a proof of value or a forecast call | [champion-check](skills/champion-check/SKILL.md) | Separates actions from promises and proposes the next small ask with a date. |
| Before practice or a big call | [buyer-roleplay](skills/buyer-roleplay/SKILL.md) | Plays the buyer, then gives feedback on eight points. |
| Before a QBR | [qbr-prep](skills/qbr-prep/SKILL.md) | Opens with the customer's value pyramid and ends with goals that state what missing them would cost. |
| Each quarter | [value-map-refresh](skills/value-map-refresh/SKILL.md) | Brings the customers' own words and results into the value map for the leadership team to decide on. |

The method behind them fits on one page: [METHOD.md](METHOD.md). It covers the evidence ladder (not asked, assumed, relayed, confirmed), the eight MEDDPICC letters, the stages and their exits, and the forecast categories.

## Install

Get the files first: `git clone https://github.com/jacobtop-tcg/b2b-sales-skills.git`, or Code > Download ZIP on GitHub. Run the commands below from inside that folder.

Claude Code: copy the skill folders into `~/.claude/skills/` to use them everywhere, or into `.claude/skills/` inside a project to use them there.

```sh
mkdir -p ~/.claude/skills
cp -r skills/* ~/.claude/skills/
```

Claude.ai: turn on code execution in Settings > Capabilities. Zip one skill folder, then upload it in Customize > Skills: choose +, Create skill, Upload a skill. Repeat for each skill.

```sh
cd skills && zip -r deal-review.zip deal-review
```

Codex: run `mkdir -p ~/.codex/skills && cp -r skills/* ~/.codex/skills/`, then open a new Codex session. Other agents that read SKILL.md: copy the folders into that agent's skills folder.

ChatGPT, Gemini, Copilot: paste a prompt from [PROMPTS.md](PROMPTS.md), or the body of a `SKILL.md`, as your first message.

## Before you use them on real deals

- Agree with your team which tool customer data may go into, and use only that one.
- Ask before you record a call, offer to stop, and keep recordings only as long as you need them.
- Start with two skills, meeting-prep and call-debrief, on live deals, with the sales leader going first.

## Related

- Every skill as a web page with a copy button: [AI sales skills and prompts](https://topmoller.com/tools/ai-sales-skills/). Practise the forecast categories in the [sales forecast game](https://topmoller.com/tools/sales-forecast-game/).
- [sales-engineering-skills](https://github.com/jacobtop-tcg/sales-engineering-skills): skills for sales engineers, including proof of value plans, business value assessment interviews and mutual action plans.
- Free tools in the browser: the [champion test](https://topmoller.com/tools/champion-test/), the [sales follow-up email](https://topmoller.com/tools/sales-follow-up-email/) and the [sales pipeline calculator](https://topmoller.com/tools/sales-pipeline-calculator/).
- Articles: https://topmoller.com/articles/

## About

Written by Jacob Top Møller, who advises and trains B2B sales teams on go-to-market and AI. More at https://topmoller.com/.

Two techniques in meeting-prep come from the presales trainer Steve Capper: agreeing who asks, writes, keeps time and closes when an SE joins, and "play tennis", answering a question with a question. MEDDPICC is a widely used public qualification checklist.

## License

MIT. See [LICENSE](LICENSE).
