# How to use this handbook

**English** · [ภาษาไทย](how-to-use.th.md)

This guide explains, step by step, how to read the handbook, how to plug it into an AI assistant, and how to check that an answer is safe to act on.

---

## 1. Who this is for

- **Founders and SME owners** running a Thai partnership (หจก.) or company (บจก.) who want to understand what their accountant is asking for.
- **Bookkeepers and admin staff** who record invoices, pay suppliers and prepare monthly tax filings.
- **Freelancers moving to a company**, who need to know what changes.
- **Developers and AI builders** who want an agent that answers Thai tax questions with sources instead of guesses.
- **Accountants and lawyers** who want a shared, open reference they can correct and improve.

It is **not** a replacement for a licensed accountant or lawyer. It helps you ask better questions and catch mistakes early.

---

## 2. Three ways to use it

| Way | Best for | Effort |
|---|---|---|
| **A. Read it on GitHub** | Looking something up quickly | None: open the link |
| **B. Download a copy** | Offline use, sharing with your team, printing | 1 minute |
| **C. Plug it into an AI assistant** | Asking questions in plain Thai or English and getting cited answers | 2–5 minutes |

### A. Read it on GitHub

1. Open the repository page: https://github.com/KunanonJ/thai-accounting-tax-law
2. Start with the **at-a-glance table** in the README. It holds the numbers people ask about most.
3. Open the chapter you need from the chapter table. Every chapter has an English and a Thai version.
4. Use the **Glossary** (chapter 0) whenever you meet a Thai form name or term you don't know.

### B. Download a copy

- **No Git needed:** on the repository page click the green **Code** button → **Download ZIP**, then unzip it.
- **With Git:**
  ```bash
  git clone https://github.com/KunanonJ/thai-accounting-tax-law.git
  ```
  Later, run `git pull` inside the folder to get updates.

The files are plain Markdown (`.md`). They open in any text editor, in VS Code, Obsidian or Notion (import), or in a browser on GitHub.

### C. Plug it into an AI assistant

The folder `skills/thai-accounting-tax-law/` is an **agent skill**: a `SKILL.md` file with working rules, plus a `references/` folder holding the handbook. Pick the option that matches the tool you use.

#### C1. Claude Code (terminal or IDE)

1. Clone the repository (see B).
2. Copy the skill folder into your personal skills folder:
   ```bash
   mkdir -p ~/.claude/skills
   cp -r thai-accounting-tax-law/skills/thai-accounting-tax-law ~/.claude/skills/
   ```
   To use it in one project only, copy it to `.claude/skills/` inside that project instead.
3. Start a new Claude Code session. Claude loads the skill automatically when a question is about Thai accounting or tax. You can also ask for it by name: "use the thai-accounting-tax-law skill".
4. To update later: `git pull` in the cloned folder and copy the folder again.

#### C2. Claude apps (web, desktop, mobile)

1. Download the repository as a ZIP (see B) and unzip it.
2. Zip **only** the `skills/thai-accounting-tax-law` folder, so that `SKILL.md` sits at the top level of that folder inside the zip.
3. Open Claude's settings, find the section for skills, and upload the zip as a custom skill. Turn it on.
4. Ask a question in a new chat. Claude uses the skill when it is relevant.

Alternative: in a Claude **Project**, upload the files from `references/` as project knowledge, and paste the "Working rules" section of `SKILL.md` into the project's instructions.

#### C3. Other chat assistants (ChatGPT, Gemini and similar)

Most assistants let you add knowledge files and custom instructions to a project, custom GPT or Gem:

1. Upload the files in `skills/thai-accounting-tax-law/references/` as knowledge.
2. Paste the **Working rules** and **Answer format** sections from `SKILL.md` into the custom instructions.
3. Test with one of the example prompts below and check that the answer cites a source.

#### C4. Coding agents (Codex, Cursor, others)

1. Copy `skills/thai-accounting-tax-law/` into your repository.
2. Point the agent at it from its instruction file, for example in `AGENTS.md`:
   ```markdown
   For any question about Thai accounting, tax or business law, follow
   skills/thai-accounting-tax-law/SKILL.md and read only the reference
   chapters it points to.
   ```
3. In editors that use rule files, add a rule with the same sentence.

---

## 3. Example prompts

You can ask in English or Thai. The skill answers in the language you use.

**Withholding tax**
- "I'm paying a Thai freelancer 25,000 THB for logo design. How much withholding tax, which form, and when is it due?"
- "จ้างฟรีแลนซ์ออกแบบโลโก้ 25,000 บาท ต้องหัก ณ ที่จ่ายเท่าไหร่ ยื่นแบบไหน ภายในวันไหน"

**VAT**
- "Our sales are about 160,000 THB a month. When do we have to register for VAT?"
- "ยอดขายเดือนละประมาณ 160,000 บาท ต้องจด VAT เมื่อไหร่"

**Paying abroad**
- "We're a non-VAT บจก. paying 20 USD a month for a US software tool. What Thai taxes might apply?"
- "บริษัทไม่ได้จด VAT จ่ายค่าโปรแกรมจากอเมริกาเดือนละ 20 ดอลลาร์ มีภาษีอะไรต้องระวังบ้าง"

**Deadlines**
- "Build our 2027 filing calendar. We are a company with a 31 December year end, two employees, not VAT-registered."
- "ทำปฏิทินยื่นภาษีปี 2570 ให้หน่อย บริษัทปิดบัญชี 31 ธันวาคม มีพนักงาน 2 คน ไม่ได้จด VAT"

**Corporate income tax**
- "Our net profit is 1,000,000 THB and paid-up capital is 1M THB. How much CIT?"
- "กำไรสุทธิ 1 ล้านบาท ทุนชำระแล้ว 1 ล้าน เสียภาษีเงินได้นิติบุคคลเท่าไหร่"

**Changing entity**
- "We are converting our หจก. into a บจก. What do we need to do and what is still unclear?"
- "กำลังแปรสภาพ หจก. เป็น บจก. ต้องทำอะไรบ้าง มีเรื่องไหนที่ยังไม่ชัด"

**FlowAccount**
- "How do I export the ภ.ง.ด.53 file from FlowAccount and file it online?"
- "ส่งออกไฟล์ ภ.ง.ด.53 จาก FlowAccount แล้วยื่นออนไลน์ยังไง"

---

## 4. What a good answer looks like

A good answer from the skill has four parts:

1. **The answer first:** the amount, the form, the deadline.
2. **The working:** the base, the rate and the result, line by line.
3. **Tags and sources:** each rule marked [V], [S] or [U], with the link available in `sources.md`.
4. **What to check:** anything time-limited or unconfirmed, plus a reminder to have an accountant confirm before filing.

Example (shortened):

> **Withhold 750 THB and pay the freelancer 24,250 THB.** File ภ.ง.ด.3 by the 7th of next month on paper, or the 15th online.
>
> - Base: 25,000 THB (the freelancer isn't VAT-registered, so there is no VAT)
> - Rate: 3% for hire of work [V]
> - WHT: 25,000 × 3% = 750
> - Give the freelancer a 50 ทวิ certificate [S]
> - If you pay through e-Withholding Tax, the rate is 1% (250 THB) until 31 Dec 2027 [V]
>
> Check: the online +8 days applies to returns due up to 31 Jan 2027. Have your accountant confirm before filing.

If an answer has **no source**, or states a rate without saying where it comes from, treat it as unverified.

---

## 5. How to judge whether you can rely on something

| You see | It means | What to do |
|---|---|---|
| **[V]** | Checked on an official source or an authoritative reference | Generally safe; still confirm for filings |
| **[S]** | From a reputable secondary source (software blog, news, practitioner) | Fine for understanding; confirm before acting |
| **[U]** | Unconfirmed or disputed | Ask your accountant; don't act on it alone |
| **UNKNOWN** | No reliable source found | Ask a professional, or request an RD ruling |
| **Last verified** date | When the facts were last checked | If it's months old, re-check time-limited items |

Watch the **time-limited measures** table in [chapter 6](../skills/thai-accounting-tax-law/references/06-filing-calendar.md): VAT 7%, e-WHT 1%, online +8 days and the social security ceiling all have end dates.

---

## 6. Staying up to date

- On GitHub click **Watch → Custom → Releases** to get an email whenever a new version is published.
- Read [CHANGELOG.md](../CHANGELOG.md) to see what changed in each version.
- If you use the skill with an AI assistant, re-copy or re-upload the skill folder after each release.

---

## 7. FAQ

**Is it free?** Yes. It is MIT-licensed: you can use, copy, change and share it, including commercially, as long as you keep the licence notice.

**Is this legal or tax advice?** No. It is a reference built from public sources. A licensed Thai accountant, CPA or lawyer should confirm anything you file, pay or sign.

**Why English with Thai terms?** So both Thai and international readers can use it, while keeping the exact form names (ภ.ง.ด.53, ภ.พ.30) you see on Revenue Department systems. Every chapter also has a full Thai version.

**What does B.E. mean?** Buddhist Era. Thai documents use it. B.E. = C.E. + 543, so 2026 = 2569.

**Does it cover personal income tax?** Not yet. It focuses on businesses: partnerships and companies. Contributions are welcome.

**I found a mistake. What do I do?** Open an issue on GitHub with the source that shows the correct rule, or send a pull request. See [CONTRIBUTING.md](../CONTRIBUTING.md).

**Can I use it inside my company's internal tools?** Yes. Keep the licence notice and the disclaimer, and add your own house rules on top.
