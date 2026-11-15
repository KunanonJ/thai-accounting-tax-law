# Thai Accounting, Tax & Business Law — open handbook + AI skill

**คู่มือบัญชี ภาษี และกฎหมายธุรกิจไทย สำหรับ SMEs (ภาษาอังกฤษ พร้อมศัพท์ภาษาไทย)**

A practical, source-cited reference for running the books of a small Thai business: company types, corporate income tax, withholding tax, VAT, accounting and audit law, filing deadlines, and the other laws that touch day-to-day operations. It is written in English, with the Thai term placed beside each concept (ภ.ง.ด.53, หจก./บจก., 50 ทวิ, …) so it maps directly onto Revenue Department forms.

The same content ships as an **AI agent skill** (`skills/thai-accounting-tax-law/`), so Claude, Codex or any agent that reads `SKILL.md` files can answer Thai accounting questions with the same rules and citations.

> **Not legal or tax advice.** This is a working reference compiled from public sources. Rates and deadlines change. Re-check the cited source before you file, pay or sign anything, and have a licensed Thai accountant or CPA confirm it.
>
> **Last verified:** 15 November 2026 (B.E. 2569).

---

## At a glance (as of 15 Nov 2026)

| Topic | Key number | Notes |
|---|---|---|
| Corporate income tax (ภาษีเงินได้นิติบุคคล) | **20%** standard | [CIT](skills/thai-accounting-tax-law/references/02-corporate-income-tax.md) |
| SME CIT rates | **0%** on the first 300,000 THB of net profit · **15%** up to 3M · **20%** above | Only if paid-up capital ≤ 5M THB **and** revenue ≤ 30M THB |
| VAT (ภาษีมูลค่าเพิ่ม) | **7%** until **30 Sep 2027** | Royal Decree No. 807 (B.E. 2569); statutory rate is 10% |
| VAT registration | Compulsory once turnover exceeds **1.8M THB / year** | Register within 30 days |
| WHT on services (ค่าบริการ/ค่าจ้างทำของ) | **3%** | **1%** if paid through e-Withholding Tax, 1 Jan 2026 – 31 Dec 2027 |
| WHT on rent / advertising / transport | **5% / 2% / 1%** | Rent and advertising also drop to 1% via e-WHT |
| Payments abroad (ภ.ง.ด.54) | **15%** (dividends 10%) | A tax treaty may reduce it |
| Monthly WHT filing (ภ.ง.ด.1/3/53) | **7th** of next month on paper · **15th** online | Online +8 days applies to returns due up to 31 Jan 2027 |
| Annual CIT return (ภ.ง.ด.50) | Within **150 days** after year end | Half-year ภ.ง.ด.51 within 2 months after month 6 |
| Social security (ประกันสังคม) | Employer **5%** + employee **5%**, wage ceiling **17,500 THB** | 2026–2028; max 875 THB/month each |
| Keeping books and records | At least **5 years** | Accounting Act B.E. 2543 s. 14 |

---

## Handbook (คู่มือ)

| # | Chapter | What it covers |
|---|---|---|
| 0 | [Glossary · อภิธานศัพท์](skills/thai-accounting-tax-law/references/00-glossary.md) | Thai ↔ English terms, form names, document names |
| 1 | [Business entities](skills/thai-accounting-tax-law/references/01-business-entities.md) | Sole trader, หจก., บจก.; audit rules; converting a หจก. into a บจก. |
| 2 | [Corporate income tax](skills/thai-accounting-tax-law/references/02-corporate-income-tax.md) | Rates, SME bands, ภ.ง.ด.50/51, penalties, worked examples |
| 3 | [Withholding tax](skills/thai-accounting-tax-law/references/03-withholding-tax.md) | Forms, rates, e-WHT 1%, payments abroad, 50 ทวิ, worked example |
| 4 | [VAT](skills/thai-accounting-tax-law/references/04-vat.md) | Rate, registration, tax invoices, ภ.พ.30, ภ.พ.36, non-registered businesses |
| 5 | [Accounting, audit & DBD](skills/thai-accounting-tax-law/references/05-accounting-audit-dbd.md) | Accounting Act, TFRS for NPAEs, CPA vs TA, AGM and DBD filings |
| 6 | [Filing calendar](skills/thai-accounting-tax-law/references/06-filing-calendar.md) | Monthly and annual deadlines in one place |
| 7 | [Other laws](skills/thai-accounting-tax-law/references/07-other-laws.md) | PDPA, Payment Systems Act, stamp duty, social security |
| 8 | [FlowAccount how-to](skills/thai-accounting-tax-law/references/08-flowaccount-howto.md) | Bank reconcile, WHT filing file, paying tax, period lock, AI connector |
| — | [Sources](skills/thai-accounting-tax-law/references/sources.md) | Every source cited, with links |

### Evidence tags

Every rate, deadline and rule carries a tag so you know how much to trust it:

- **[V]** verified on an official source (rd.go.th, ratchakitcha, bot.or.th, dbd.go.th) or an authoritative reference (e.g. PwC Tax Summaries)
- **[S]** secondary source (accounting-software blogs, news, practitioner guides)
- **[U]** unconfirmed or disputed; ask an accountant before relying on it

---

## Use it with an AI agent

The folder `skills/thai-accounting-tax-law/` is a self-contained agent skill: `SKILL.md` holds the working rules and the `references/` folder holds the handbook.

**Claude Code**

```bash
git clone https://github.com/KunanonJ/thai-accounting-tax-law.git
mkdir -p ~/.claude/skills
cp -r thai-accounting-tax-law/skills/thai-accounting-tax-law ~/.claude/skills/
```

**Claude apps:** zip the `skills/thai-accounting-tax-law` folder and upload it as a custom skill in Claude's settings.

**Other agents (Codex, Cursor, etc.):** point the agent at `skills/thai-accounting-tax-law/SKILL.md`, or paste it into your project's agent instructions.

Then ask questions such as:

- “I'm paying a Thai freelancer 25,000 THB for design work. How much WHT, which form, and when is it due?”
- “We're a non-VAT บจก. paying for a US SaaS tool. What Thai taxes might apply?”
- “Build our 2027 filing calendar for a company with a 31 December year end.”

---

## Contributing

Corrections and additions are welcome, especially from Thai accountants and lawyers. Please read [CONTRIBUTING.md](CONTRIBUTING.md): every change needs a source, an evidence tag, and an updated *last verified* date.

Wanted next: personal income tax (ภ.ง.ด.90/91/94) for freelancers, specific business tax (ภาษีธุรกิจเฉพาะ), BOI incentives, transfer pricing for SMEs, and Thai-language translations of each chapter.

## License

[MIT](LICENSE) © Kunanon Jarat. You may copy, adapt and redistribute it. Keep the notice, and remember that the content is a reference, not advice.
