# 🇹🇭 Thai Accounting, Tax & Business Law

**English** · [ภาษาไทย](README.th.md)

**Thai SME taxes, explained without the headache. Every number has receipts.** 🧾

You run a หจก. or บจก., or you're about to. You've heard "ภ.ง.ด.53", "50 ทวิ" and "VAT 7%… for now?" and nodded along. This repo is the open, free cheat sheet we wish we'd had: what to pay, which form, by when, and *where that rule actually comes from*.

It's a handbook you can read **and** an AI skill you can plug into Claude, ChatGPT or your own agent, so you get cited answers instead of confident guesses.

> ⚠️ **Real talk first:** this is a reference, not legal or tax advice. Thai rules change, sometimes every year. Before you file, pay or sign anything, check the linked source and have a licensed accountant or CPA confirm it.
>
> 🗓️ **Facts last verified:** 15 Nov 2026 (B.E. 2569) · 📦 **Version:** [v1.0.0](CHANGELOG.md)

---

## ✅ Why you can trust this (and when you shouldn't)

We'd rather be useful than sound smart, so here's how it works:

- **Receipts on every line.** Every rate, deadline and rule links to where it came from: Revenue Department, Royal Gazette, DBD, BOT, PwC, and so on. See [sources](skills/thai-accounting-tax-law/references/sources.md).
- **We tag how sure we are.** **[V]** checked on an official source · **[S]** reputable secondary source · **[U]** not confirmed, ask an accountant.
- **We say "UNKNOWN" out loud.** If we couldn't find a solid answer (hi, ภ.พ.36 for non-VAT companies 👋), we say so instead of making something up.
- **We show the maths.** Worked examples, line by line, so you can check them yourself.
- **We flag expiry dates.** VAT 7%, e-WHT 1% and online +8 days are all temporary. They're tracked in one [table](skills/thai-accounting-tax-law/references/06-filing-calendar.md#time-limited-measures-to-watch).
- **No private data.** No real tax IDs, bank accounts or client details. Ever.
- **Open and fixable.** MIT-licensed. Spot a mistake? Open an issue with a source and it gets fixed, with the change logged in the [changelog](CHANGELOG.md).

---

## ⚡ The numbers people ask about most (as of 15 Nov 2026)

| What | Number | The catch |
|---|---|---|
| Corporate income tax | **20%** | SMEs pay less (next row) |
| SME CIT | **0%** on the first 300k profit · **15%** to 3M · **20%** above | Only if paid-up capital ≤ 5M **and** revenue ≤ 30M THB |
| VAT | **7%** | Until **30 Sep 2027** (Royal Decree 807). The legal rate is 10% |
| Register for VAT | Turnover **> 1.8M THB/year** | Within 30 days of crossing it |
| WHT: services | **3%** | **1%** via e-Withholding Tax until 31 Dec 2027 |
| WHT: rent / ads / transport | **5% / 2% / 1%** | Rent and ads also drop to 1% via e-WHT |
| Paying abroad (ภ.ง.ด.54) | **15%** | A tax treaty may cut it; SaaS is a grey area [U] |
| Monthly WHT filing | **7th** (paper) · **15th** (online) | Online +8 days covers returns due up to 31 Jan 2027 |
| Annual CIT (ภ.ง.ด.50) | **150 days** after year end | Half-year ภ.ง.ด.51 within 2 months after month 6 |
| Social security | **5% + 5%**, wage cap **17,500** | Max 875 THB/month each, 2026–2028 |
| Keep your books | **5 years** | Accounting Act s. 14 |

---

## 📚 The handbook

Every chapter comes in English and Thai.

| # | Chapter | English | ภาษาไทย |
|---|---|---|---|
| 🚀 | **How to use this repo** (start here) | [Guide](docs/how-to-use.md) | [คู่มือการใช้งาน](docs/how-to-use.th.md) |
| 0 | Glossary: Thai ↔ English terms and forms | [Glossary](skills/thai-accounting-tax-law/references/00-glossary.md) | (bilingual) |
| 1 | Business entities, CPA vs TA, หจก. → บจก. | [EN](skills/thai-accounting-tax-law/references/01-business-entities.md) | [TH](skills/thai-accounting-tax-law/references/01-business-entities.th.md) |
| 2 | Corporate income tax | [EN](skills/thai-accounting-tax-law/references/02-corporate-income-tax.md) | [TH](skills/thai-accounting-tax-law/references/02-corporate-income-tax.th.md) |
| 3 | Withholding tax, e-WHT, paying abroad | [EN](skills/thai-accounting-tax-law/references/03-withholding-tax.md) | [TH](skills/thai-accounting-tax-law/references/03-withholding-tax.th.md) |
| 4 | VAT, ภ.พ.30, ภ.พ.36 | [EN](skills/thai-accounting-tax-law/references/04-vat.md) | [TH](skills/thai-accounting-tax-law/references/04-vat.th.md) |
| 5 | Accounting law, audit, DBD filings | [EN](skills/thai-accounting-tax-law/references/05-accounting-audit-dbd.md) | [TH](skills/thai-accounting-tax-law/references/05-accounting-audit-dbd.th.md) |
| 6 | Filing calendar | [EN](skills/thai-accounting-tax-law/references/06-filing-calendar.md) | [TH](skills/thai-accounting-tax-law/references/06-filing-calendar.th.md) |
| 7 | PDPA, payments law, stamp duty, social security | [EN](skills/thai-accounting-tax-law/references/07-other-laws.md) | [TH](skills/thai-accounting-tax-law/references/07-other-laws.th.md) |
| 8 | FlowAccount how-to | [EN](skills/thai-accounting-tax-law/references/08-flowaccount-howto.md) | [TH](skills/thai-accounting-tax-law/references/08-flowaccount-howto.th.md) |
| 9 | **Real-life scenarios**: freelancer, rent, SaaS, VAT threshold, first hire, month end, year end | [EN](skills/thai-accounting-tax-law/references/09-scenarios.md) | [TH](skills/thai-accounting-tax-law/references/09-scenarios.th.md) |
| — | Sources | [All links](skills/thai-accounting-tax-law/references/sources.md) | |

---

## 🤖 Use it with AI (2-minute setup)

The folder `skills/thai-accounting-tax-law/` is a ready-made **agent skill**. It tells the AI to cite sources, show its maths, flag what's unconfirmed and check expiry dates.

**Claude Code**

```bash
git clone https://github.com/KunanonJ/thai-accounting-tax-law.git
mkdir -p ~/.claude/skills
cp -r thai-accounting-tax-law/skills/thai-accounting-tax-law ~/.claude/skills/
```

**Claude apps, ChatGPT, Gemini, Codex, Cursor:** step-by-step instructions for each are in the [how-to-use guide](docs/how-to-use.md#c-plug-it-into-an-ai-assistant).

Then just ask, in Thai or English:

> "Paying a Thai freelancer 25,000 THB for design work. How much WHT, which form, and when?"
>
> "จ้างฟรีแลนซ์ 25,000 บาท ต้องหัก ณ ที่จ่ายเท่าไหร่ ยื่นแบบไหน ภายในวันไหน"

You should get the answer first, then the maths, then the tags and what to double-check. If an answer doesn't cite anything, don't trust it.

---

## 🛠️ Contribute

Accountants, lawyers, bookkeepers, founders who've been through it: your corrections make this better for everyone. Read [CONTRIBUTING.md](CONTRIBUTING.md) ([ภาษาไทย](CONTRIBUTING.th.md)). The rules are short: cite a source, tag it, update the date.

**On the wishlist:** personal income tax for freelancers (ภ.ง.ด.90/91/94), specific business tax, BOI incentives, transfer pricing for SMEs.

---

## 📄 License

[MIT](LICENSE) © Kunanon Jarat. Use it, fork it, ship it in your product. Just keep the notice, and remember it's a reference, not advice.

If this saved you a confused afternoon, a ⭐ helps other people find it.
