# DRIFT Check 

This repository contains a prompt designed to run inside an LLM to help you understand an organisational situation more clearly.

You can jump straight in and download it [here](https://raw.githubusercontent.com/stigmergist/DRIFT-Check/refs/heads/main/DRIFT_CHECK_THINKING.md ) (right-click, 'Download as...' - see [instructions](#how-to-use-this-prompt-in-an-llm))

Or there is a [chat bot on the ChatGPT Store](https://chatgpt.com/g/g-69ce433adb988191ba0ef75e8e87204c-drift-check) that uses it.

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/W7W31XXGLZ)

## What this is

- A thinking tool for sense-making in messy organisational contexts.
- A prompt that keeps analysis anchored in observable signals, not assumptions.
- A way to surface misfit between the situation and the action being proposed.
- A way to work through large document sets, long email chains, and board or programme packs to extract key signals and patterns about:
  - what situation you are really in
  - the current state of capabilities
  - what actions are currently happening
  - where those things are in conflict
- A practical language for four questions:
  - Should we act? (context)
  - What kind of action fits? (capability state)
  - What actions are we doing?
  - What are the issues and risks if these are in conflict?

This prompt is built to improve judgment quality, not to automate judgment.

## What this is not

- Not a framework explainer.
- Not a methodology rollout package.
- Not a diagnostic engine.
- Not an answer generator.
- Not a replacement for observation-based judgment.

For a future side-by-side boundary comparison against methods/frameworks, see [METHOD_COMPARISON.md](METHOD_COMPARISON.md).


## How to use this prompt in an LLM

### 1. Start by sharing the prompt

- First, share [DRIFT_CHECK_THINKING.md](DRIFT_CHECK_THINKING.md) with the assistant (see [Security and safety](README.md#security-and-safety) and make sure you are using an appropriate approved AI chat for your information).
  - Option 1: download it and add it to chat as a file attachment.
  - Option 2: if your chat tool does not let you attach files, copy all text from [DRIFT_CHECK_THINKING.md](DRIFT_CHECK_THINKING.md) and paste it as your first message.
  - Better option for repeat use: create a persistent assistant and store this prompt as its main instruction.
    - Microsoft Copilot (Copilot Studio Agents): https://learn.microsoft.com/microsoft-copilot-studio/
    - ChatGPT (Custom GPTs): https://help.openai.com/en/articles/8554397-creating-a-gpt
    - Claude (Projects): https://support.anthropic.com/en/articles/9517075-what-are-projects
    - Gemini (Gems): https://support.google.com/gemini/answer/15235426
    - NotebookLM (notebooks and sources): https://support.google.com/notebooklm
- Check it loaded correctly. Ask: "What is DRIFT?"
- Keep everything in one chat thread so the assistant keeps the same context.

### 2. Discuss a real situation

Discuss what is happening in your organisation right now:

- what is happening now
- share documents, spreadsheets, links, etc. for context (make sure you're not breaking an info security!)
- what decisions are pending
- what outcomes are inconsistent or unclear
- what people are saying versus what they are doing

You can also say: "Before you answer, ask me any clarifying questions you need."

The more detail, the better. Do not worry if it is not coherent - that is kind of the point.

### 3. Ask for an initial analysis

Once you have shared your situation, ask for an initial analysis.

You can copy and paste one of these:

- "Based on what I shared, what do you think is really going on here?"
- "What are the most important factors driving this situation right now?"
- "What might I be missing or assuming without real evidence?"
- "If we do nothing, what is the most likely outcome in the short term?"
- "What is one practical next step we could take this week to learn more before making a bigger decision?"

Depending on the capabilities of your LLM, you might ask it to do large scoped analysis:
- "here's a large board pack. give me drift check and help me understand the difference between the intention and the signalled reality, so that I can focus on the rigth issues"
- "here are N programmes and their bsuiness cases, plans, risk logs, etc. all in the same organisation., give me a drift check of the situation"
- "Look at companies in the XXX sector. find online information about them inclduing recent news articels, features, blog posts, company filings, company documents, audits, analysts findings, employee ratings, customer ratings, and information on the sector they are in. Consider the capabiltities stacks and what underlying capabilities the share - and any systemic risk this might imply. With relevant links and quotes taht can be verified, give my a DRIFT based analysis of what is going on."

### 4. Continue until clarity

Keep discussing the situation until it helps you get clarity.

Do not push for one final answer too quickly. Use the chat to test your thinking, challenge assumptions, and improve your understanding step by step.

### 5. Revisit regularly

Come back to the same situation regularly and re-check your view.

Things change, and new observations appear once you start seeing the situation differently.

- Treat each discussion as a snapshot, not a permanent conclusion.
- Update your understanding as new evidence comes in.
- Re-check decisions after key events or new information.

## Example usage modes

- **Programme pulse-check**: use it periodically to detect misfit early.
- **Board and executive papers review**: run business cases, programme packs, and board packs through the prompt to test assumptions, clarity, risks, and likely consequences.
- **Interview preparation**: ask the LLM to gather public signals (news, product launches, strategy updates, filings, and investor commentary) to build a picture of the company's priorities and likely challenges.
- **Journalism and investigations**: as a journalist trying to understand what is going on in one company or across a group of companies, use it to surface patterns and generate stronger interview questions.
- **Executive checkpoint**: use it before a major decision to test readiness and action fit.
- **Team review**: use it in a working session to align interpretation across functions.

## Security and safety

- The core prompt is delivered as raw text in a markdown file ([DRIFT_CHECK_THINKING.md](DRIFT_CHECK_THINKING.md)) so you can inspect it directly for unsafe directives, jailbreak attempts, or hidden instructions.
- Always use LLM tools within the information security boundary appropriate to the material you are sharing.
- Do not paste sensitive internal programme documents into public or unapproved tools.
- Use only LLM platforms approved by your information security team for the sensitivity level of your data.
- If unsure, treat the information as high risk and check with your security/governance team before uploading content.

## Repository guide

- Prompt source: [DRIFT_CHECK_THINKING.md](DRIFT_CHECK_THINKING.md)
- Principles: [DRIFT_PRINCIPLES.md](DRIFT_PRINCIPLES.md)
- Practical companion docs: [docs/README.md](docs/README.md)
  - Companion guides and checklists for manual use.
  - Layer 1 context checklist: [docs/l1_context_checklist_v2.md](docs/l1_context_checklist_v2.md)
  - Layer 2 action-fit checklist: [docs/l2_sro_checklist_v2.md](docs/l2_sro_checklist_v2.md)
  - One-page alignment matrix: [docs/l2_sro_alignment_matrix_v2.md](docs/l2_sro_alignment_matrix_v2.md)

## License

This work is licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).

Under CC BY 4.0, you are free to:

- Share: copy and redistribute the material in any medium or format.
- Adapt: remix, transform, and build upon the material for any purpose, including commercial use.

Under the following terms:

- Attribution: give appropriate credit, provide a link to the license, and indicate whether changes were made.

No liability / no warranty: this material is provided "as is", without warranties of any kind, express or implied.
Use at your own risk. The author is not liable for any loss, damage, or consequences arising from use of this material.

- License: https://creativecommons.org/licenses/by/4.0/
- Copyright: John S Nolan, TechTalkType
- Contact: john@techtalktype.com
