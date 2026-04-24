# Gemini Remediation Skills

Self-contained skill prompts for deployment on `gemini.genai.mil` via SharePoint launcher buttons.

## Deployment model

- Each skill is a single Markdown file containing one complete, locked-in prompt.
- The prompt is pasted as the first message in a Gemini conversation.
- A SharePoint page exposes one button per skill. Each button opens a pre-loaded conversation.
- Users never route themselves between skills. The button they click *is* the routing.

## Design principles

1. **Each skill is fully self-contained.** All baseline knowledge, tone rules, scoping rules, walkthrough protocol, training URLs, wrap-up, and disclaimer are inlined. No external file references.
2. **No mention of `.md` files, reference documents, or external knowledge bases.** The skill presents its knowledge as its own internal knowledge.
3. **No cross-skill references.** A Word skill conversation never says "go use the PDF button instead." Each skill works with whatever the user brings.
4. **Plain Markdown, copy-paste-ready.** No dependencies on features the target system may or may not render.
5. **Shared sections are identical across skills for maintainability.** Tone rules, walkthrough protocol, wrap-up message, and disclaimer are copy-paste identical.

## Inventory

| File | Button label | Status |
|------|--------------|--------|
| `skill-word.md` | Remediate Word Document | ✅ Ready |
| `skill-excel.md` | Remediate Excel Spreadsheet | ⏳ Pending approval of Word pattern |
| `skill-powerpoint.md` | Remediate PowerPoint Presentation | ⏳ Pending approval of Word pattern |
| `skill-pdf.md` | Remediate PDF | ⏳ Pending approval of Word pattern |
| `skill-web.md` | Remediate Web Page | ⏳ Pending approval of Word pattern |

## Updating a skill

When standards change or feedback comes in:

1. Edit the relevant `skill-*.md` file.
2. If the change is to a shared section (tone, walkthrough protocol, wrap-up, disclaimer), apply it to all five files.
3. Replace the pinned prompt in the corresponding SharePoint launcher.

## Disclaimer posture

Every skill ends a completed session with the same AI disclaimer. The SharePoint launcher page should also carry high-level context (what this is, what it is not, when to consult your accessibility program office).
