# 8. FlowAccount how-to · วิธีทำงานใน FlowAccount

**English** · [ภาษาไทย](08-flowaccount-howto.th.md)

_Last verified 15 Nov 2026. Tags: [V] FlowAccount's own help centre · [S] secondary._

FlowAccount is a widely used Thai cloud accounting package. Menu names below are as they appear in the Thai interface; the English interface uses equivalent labels.

## AI connector (Claude and other MCP clients)

- Custom connector URL: `https://mcp.flowaccount.com/mcp`, signed in with OAuth. One company per connection; to switch company, disconnect and reconnect [V FlowAccount help].
- Can **read** documents and reports and **create** quotations, billing notes/invoices, tax invoices, cash-sale tax invoices/receipts, receipts, purchase orders, goods receipts, expenses and journal entries. Every create is a two-step preview then confirm [V FlowAccount help].
- Cannot (at the time of checking) edit, delete or void documents, create credit/debit notes, record partial payments, reconcile banks, run payroll or adjust stock [V FlowAccount help]. Do those on the website.

## Recording a sale or expense with evidence

- Create the document (sales or expense), pick the existing contact rather than retyping it, and choose the right category.
- Attach the supporting files to the document: the invoice or receipt under general documents, and the bank slip or payment advice under payment evidence. Payment evidence also helps automatic bank matching.
- If the money has already moved, record the payment with its real date and bank account so the bank ledger matches the statement.

## Bank reconcile · กระทบยอดธนาคาร (website only)

[V FlowAccount help]

1. Go to Finance (การเงิน), open the bank account card's "···" menu, choose **กระทบยอด** (or เริ่มกระทบยอด).
2. Upload the bank statement file.
3. Check that *bank balance − FlowAccount balance = difference*.
4. Match in either view: **แสดงแบบรายการ** (one statement line ↔ one document) or **แสดงแบบเปรียบเทียบ** (many ↔ many).
5. Undo a match with **ยกเลิก / ยกเลิกจับคู่**.
6. Transfers between your own accounts: use **โอนเงินระหว่างบัญชี**, not income or expense.

Tip: FlowAccount offers a "+ JV" difference journal. Prefer fixing the underlying document (wrong amount, date or account) over posting a difference entry, and only match at a difference of zero.

## Withholding-tax filing file · ไฟล์ยื่นภาษีหัก ณ ที่จ่าย

[V FlowAccount help]

1. **ยื่นแบบภาษีออนไลน์** (or บริหารบัญชี → บริหารภาษีมูลค่าเพิ่ม → ยื่นหัก ณ ที่จ่ายออนไลน์).
2. Choose the form (ภ.ง.ด.3 / 53) and the tax month (เดือนภาษี) → **แสดงผลรายงาน**.
3. **ดาวน์โหลดไฟล์เพื่อยื่นออนไลน์** (.txt).
4. Convert it in the RD's **RD Prep** program to .rdx, then upload on RD e-Filing.
5. Payee names need a title followed by a space (e.g. "น.ส. สมหญิง ...").

## Paying tax, social security or loans · ชำระหนี้

[V FlowAccount help]

- **ค่าใช้จ่าย → สร้างใหม่ → ชำระหนี้/จ่ายเงินทุน.**
- FlowAccount's default liability accounts: **27123** ภาษีหัก ณ ที่จ่าย – ภ.ง.ด.3 and **27124** ภาษีหัก ณ ที่จ่าย – ภ.ง.ด.53. Codes may differ if your chart of accounts was customised.
- Status goes from รอดำเนินการ (awaiting) to ชำระเงิน (paid) once you record the payment.

## Period lock · ล็อกงวดบัญชี

[V FlowAccount help]

- **ตั้งค่า → ตั้งค่าด้านบัญชี → ล็อกงวดบัญชี.** Needs the Standard package or higher. Not available for companies connected through the Open API.
- Lock each month after it has been reconciled and filed, so nobody changes a closed period by accident.

## Chart of accounts and opening balances

- Chart of accounts: **บริหารบัญชี → ผังบัญชี → บริหารผังบัญชี** [S].
- Opening balances for a new file (or a converted entity) need a trial balance, AR/AP lists, a fixed-asset register and bank balances as at the start date [S FlowAccount]. Ask FlowAccount support or your accountant for the entry method.
