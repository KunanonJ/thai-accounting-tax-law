# Changelog · บันทึกการเปลี่ยนแปลง

All notable changes are listed here, newest first. Each release also records the date its facts were last verified.
การเปลี่ยนแปลงสำคัญทั้งหมดบันทึกไว้ที่นี่ เรียงจากใหม่ไปเก่า แต่ละเวอร์ชันระบุวันที่ตรวจสอบข้อมูลล่าสุดด้วย

Format based on [Keep a Changelog](https://keepachangelog.com/). Versions follow [Semantic Versioning](https://semver.org/): a **major** version for restructures, a **minor** version for new chapters or new rules, a **patch** for corrections and updated rates.

---

## [1.0.0] — 2026-11-15

**Facts last verified · ตรวจสอบข้อมูลล่าสุด:** 15 Nov 2026 (15 พ.ย. 2569)

### English

First public release.

**Added**
- A handbook of ten chapters for Thai SMEs: glossary, business entities and หจก. → บจก. conversion, corporate income tax, withholding tax, VAT, accounting/audit/DBD filings, filing calendar, other laws (PDPA, Payment Systems Act, stamp duty, social security), a FlowAccount how-to, and real-life scenarios.
- Full Thai versions of every chapter (`*.th.md`), a Thai README and a Thai contributing guide.
- A step-by-step how-to-use guide in English and Thai, covering reading, Claude Code, Claude apps, other chat assistants and coding agents, with example prompts in both languages.
- An AI agent skill (`skills/thai-accounting-tax-law/SKILL.md`) with working rules: cite or say UNKNOWN, show the maths, check time-limited measures, draft rather than decide.
- Evidence tags on every rule ([V] official · [S] secondary · [U] unconfirmed) and a sources page.

**Verified in this release**
- VAT stays at 7% until 30 Sep 2027 under Royal Decree No. 807 (B.E. 2569), published 23 Aug 2026.
- e-Withholding Tax at 1% from 1 Jan 2026 to 31 Dec 2027 under Ministerial Regulation No. 402 (B.E. 2569), published in October 2026.
- Online filing +8 days applies to returns due 1 Feb 2024 – 31 Jan 2027.
- Social security wage ceiling of 17,500 THB (maximum 875 THB a month each) for 2026–2028.

**Known gaps**
- ภ.พ.36 for non-VAT-registered buyers of foreign services: [U].
- ภ.ง.ด.54 treatment of foreign SaaS subscriptions: [U].
- Whether a stub-period ภ.ง.ด.50 is due when a หจก. converts into a บจก.: [U].
- Personal income tax is not covered yet.

### ภาษาไทย

เวอร์ชันแรกที่เผยแพร่สู่สาธารณะ

**เพิ่มเข้ามา**
- คู่มือ 10 บทสำหรับ SMEs ไทย: อภิธานศัพท์, รูปแบบธุรกิจและการแปรสภาพ หจก. เป็น บจก., ภาษีเงินได้นิติบุคคล, ภาษีหัก ณ ที่จ่าย, ภาษีมูลค่าเพิ่ม, การบัญชี/การสอบบัญชี/การส่งงบ, ปฏิทินยื่นภาษี, กฎหมายอื่น (PDPA, พ.ร.บ.ระบบการชำระเงิน, อากรแสตมป์, ประกันสังคม), วิธีใช้ FlowAccount และสถานการณ์ตัวอย่าง
- ฉบับภาษาไทยครบทุกบท (`*.th.md`) พร้อม README และคู่มือการร่วมพัฒนาภาษาไทย
- คู่มือการใช้งานแบบทีละขั้นตอน ทั้งภาษาไทยและอังกฤษ ครอบคลุมการอ่าน, Claude Code, แอป Claude, ผู้ช่วย AI อื่น ๆ และ coding agent พร้อมตัวอย่างคำถามสองภาษา
- AI agent skill (`skills/thai-accounting-tax-law/SKILL.md`) พร้อมกฎการทำงาน: ต้องอ้างอิงที่มาหรือบอกว่าไม่ทราบ, แสดงวิธีคำนวณ, ตรวจมาตรการที่มีวันหมดอายุ, ร่างให้แต่ไม่ตัดสินใจแทน
- ป้ายระดับความน่าเชื่อถือทุกกฎ ([V] แหล่งทางการ · [S] แหล่งรอง · [U] ยังไม่ยืนยัน) และหน้ารวมแหล่งอ้างอิง

**ตรวจสอบแล้วในเวอร์ชันนี้**
- VAT 7% ถึง 30 ก.ย. 2570 ตามพระราชกฤษฎีกา ฉบับที่ 807 (พ.ศ. 2569) ประกาศ 23 ส.ค. 2569
- ภาษีหัก ณ ที่จ่ายผ่านระบบ e-Withholding Tax 1% ตั้งแต่ 1 ม.ค. 2569 ถึง 31 ธ.ค. 2570 ตามกฎกระทรวง ฉบับที่ 402 (พ.ศ. 2569) ประกาศเดือนตุลาคม 2569
- ยื่นแบบออนไลน์ได้เพิ่ม 8 วัน สำหรับแบบที่ครบกำหนด 1 ก.พ. 2567 – 31 ม.ค. 2570
- เพดานค่าจ้างประกันสังคม 17,500 บาท (สมทบสูงสุดฝ่ายละ 875 บาทต่อเดือน) ปี 2569–2571

**เรื่องที่ยังไม่ชัด**
- ภ.พ.36 สำหรับผู้ซื้อบริการต่างประเทศที่ไม่ได้จด VAT: [U]
- การหักภาษี ภ.ง.ด.54 สำหรับค่าบริการ SaaS ต่างประเทศ: [U]
- ต้องยื่น ภ.ง.ด.50 ช่วงก่อนแปรสภาพ หจก. เป็น บจก. หรือไม่: [U]
- ยังไม่ครอบคลุมภาษีเงินได้บุคคลธรรมดา
