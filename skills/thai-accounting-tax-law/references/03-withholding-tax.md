# 3. Withholding tax · ภาษีหัก ณ ที่จ่าย

_Last verified 15 Nov 2026. Tags: [V] official · [S] secondary · [U] unconfirmed._

The payer deducts tax from a payment, files a return, remits the tax to the RD, and gives the payee a certificate. The payee claims the withheld amount against their own income tax.

## Which form

| Form | Use for |
|---|---|
| ภ.ง.ด.1 | Salaries and wages to employees |
| ภ.ง.ด.3 | Payments to **individuals** (freelancers, landlords who are individuals) |
| ภ.ง.ด.53 | Payments to **juristic persons** (companies, partnerships) |
| ภ.ง.ด.54 | Payments to recipients **abroad** |

File only in months when tax was actually withheld [S FlowAccount].

## Domestic rates (normal)

| Payment | Rate | Evidence |
|---|---|---|
| Services, hire of work (ค่าบริการ, ค่าจ้างทำของ) | 3% | [V — rates restated in the cabinet's e-WHT decision, 16 Jun 2026] |
| Professional fees to individuals (ค่าวิชาชีพอิสระ) | 3% | [S Krungsri] |
| Rent (ค่าเช่า) | 5% | [V same as above] |
| Advertising (ค่าโฆษณา) | 2% | [V same] |
| Transport (ค่าขนส่ง) | 1% | [V same]; Thailand Post is exempt [S Krungsri] |
| Dividends | 10% (0% if the recipient is a listed company) | [V PwC] |
| Interest to a non-bank company | 1% | [V PwC] |
| Royalties to a company | 3% | [V PwC] |
| Salaries | Progressive personal income tax rates, estimated for the year | [S FlowAccount] |

**The 1,000 THB rule.** Withholding is generally required when a payment to a payee is **1,000 THB or more**. It also applies to smaller amounts under an ongoing contract (e.g. monthly internet), and to a job worth 1,000 THB or more that is paid in instalments below 1,000 [S FlowAccount]. Confirm edge cases with your accountant.

**Base.** WHT is computed on the amount **before VAT** [S].

## e-Withholding Tax: 1%

If you pay through a bank that offers the RD's **e-Withholding Tax** system, the 5%, 3% and 2% rates drop to **1%** [V].

- Legal basis: Ministerial Regulation No. 402 (กฎกระทรวง ฉบับที่ 402, B.E. 2569), published in the Royal Gazette in October 2026 and effective **1 Jan 2026 – 31 Dec 2027** [V rd.go.th].
- The bank deducts the tax, remits it to the RD and issues electronic evidence to both sides, so you don't remit those amounts yourself [S PEAK].
- Payments made outside the system keep the normal rates [S PEAK].
- There was a gap: the previous measure ended on 31 Dec 2025, and the new regulation applies back to 1 Jan 2026 [V].

## Worked example

You buy a 10,000 THB service from a VAT-registered Thai company.

| Line | Normal | Through e-WHT |
|---|---|---|
| Service fee | 10,000.00 | 10,000.00 |
| VAT 7% | 700.00 | 700.00 |
| Invoice total | 10,700.00 | 10,700.00 |
| WHT on the pre-VAT 10,000 | 3% = 300.00 | 1% = 100.00 |
| **You transfer** | **10,400.00** | **10,600.00** |
| Form | ภ.ง.ด.53 | Handled by the bank |

## Payments abroad (ภ.ง.ด.54)

- Final WHT is generally **15%** on interest, royalties, rentals and service fees paid to a foreign company not carrying on business in Thailand; **10%** on dividends [V PwC].
- A **double tax treaty** may reduce or remove it. You need the recipient's certificate of residence to apply a treaty rate [S].
- Software and SaaS subscriptions are a grey area. One accounting-software blog treats Google Workspace fees as royalty-type income at 15% unless a treaty applies [S FlowAccount]. Whether ภ.ง.ด.54 applies to a particular foreign SaaS vendor, and at what treaty rate, is **[U]**. Get your accountant's view before you start or stop withholding.
- Paying abroad can also trigger **ภ.พ.36** (self-assessed VAT); see [chapter 4](04-vat.md).

## Deadlines

| Filing | Due | Evidence |
|---|---|---|
| Paper | Within **7 days** after the end of the month of payment | [V RD; S FlowAccount] |
| Online (e-Filing) | **8 days later**, around the 15th, moved to the next business day if it falls on a holiday | [V] for returns due 1 Feb 2024 – 31 Jan 2027; check renewal after that |

Example: WHT on payments made in September is due 7 October on paper or 15 October online.

## Certificate (50 ทวิ)

The payer gives the payee the original withholding tax certificate (หนังสือรับรองการหักภาษี ณ ที่จ่าย, form 50 ทวิ) and keeps a copy with the payment record [S]. Freelancers need it to file their personal income tax return.

## Common mistakes

- Using ภ.ง.ด.3 for a company (it should be ภ.ง.ด.53) or the reverse; check the payee's tax ID and entity type.
- Computing WHT on the VAT-inclusive amount.
- Forgetting a title on payee names in the e-Filing file; names need a title and a space, e.g. "น.ส. ..." or "บริษัท ... จำกัด" [S FlowAccount].
- Filing late: a 1.5% per month surcharge applies to tax remitted late [S].
