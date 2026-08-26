# คู่มือ: Obsidian + Claude Code

**Guide: Obsidian + Claude Code**

วิธีเอาสมองของทีม (โฟลเดอร์นี้) ไปตั้งใช้เองที่ร้าน — โหลดสองแอป แล้วชี้ที่โฟลเดอร์เดียวกัน
_How to run the team brain (this folder) yourself — install two apps and point them at the same folder._

---

## หัวใจของเรื่องนี้ / The big idea

สองแอป ทำงานคนละหน้าที่ แต่เปิด **โฟลเดอร์เดียวกัน**
_Two apps, two jobs, one shared folder._

| แอป / App | คือ / What it is | หน้าที่ / Its job |
|---|---|---|
| **Obsidian** | หน้าต่างของคน · the human's window | เปิดดู/แก้โน้ต เห็นกราฟ เห็นลิงก์ `[[...]]` · read, edit, browse, see the graph |
| **Claude Code** | บรรณารักษ์ AI · the AI librarian | สัมภาษณ์ จด จัดเข้าชั้น ตอบคำถาม · interview, write, file, answer |

> คนอ่านผ่าน Obsidian · AI เขียนผ่าน Claude Code · ทั้งคู่ชี้ไฟล์ชุดเดียวกัน
> _People read through Obsidian. The AI writes through Claude Code. Both see the same files._

---

## เตรียมก่อน / Before you start

- โฟลเดอร์ skeleton (ได้จาก QR / repo / ไฟล์ zip ในงาน) — _the skeleton folder (from the QR / repo / zip)_
- คอมพิวเตอร์ Windows หรือ Mac — _a Windows or Mac computer_
- อินเทอร์เน็ต + บัญชี Claude — _internet + a Claude account_

---

## ขั้นที่ 1 — ติดตั้ง Obsidian / Step 1 — Install Obsidian

1. ไปที่ **obsidian.md** → กด **Download** → ติดตั้งตามปกติ
   _Go to obsidian.md → Download → install._
2. เปิด Obsidian → เลือก **"Open folder as vault"** → เลือกโฟลเดอร์ skeleton
   _Open Obsidian → "Open folder as vault" → pick the skeleton folder._
3. ถ้ามีหน้าต่างถาม **"Trust author and enable plugins"** ให้กด **Trust** (เป็นโฟลเดอร์ของเราเอง)
   _If it asks "Trust author and enable plugins", click Trust — it's your own folder._

**จะเห็นอะไร / What you'll see:** ไฟล์ `HOME.md`, โฟลเดอร์ `raw/` `knowledge/` `wiki/`, และปุ่ม **Graph** ทางซ้าย (ภาพเส้นเชื่อมโน้ต)
_The `HOME.md` file, the `raw/` `knowledge/` `wiki/` folders, and the Graph button on the left (the web of linked notes)._

---

## ขั้นที่ 2 — ติดตั้ง Claude Code / Step 2 — Install Claude Code

1. โหลด **Claude Code** จาก Anthropic — มีทั้งแอปเดสก์ท็อป (Mac/Windows) และแบบใช้ผ่าน terminal
   _Get Claude Code from Anthropic — desktop app (Mac/Windows) or the terminal CLI._
2. ล็อกอินด้วยบัญชี Claude — _Sign in with your Claude account._
3. เปิด **โฟลเดอร์เดียวกัน** กับที่เปิดใน Obsidian
   _Open the **same folder** you opened in Obsidian._
   - แอปเดสก์ท็อป: "Open folder / project" แล้วเลือกโฟลเดอร์ skeleton
     _Desktop app: "Open folder / project" → the skeleton folder._
   - แบบ terminal: `cd` เข้าไปในโฟลเดอร์ แล้วสั่ง `claude`
     _CLI: `cd` into the folder, then run `claude`._
4. พิมพ์ประโยคแรก: **"อ่าน CLAUDE.md ก่อน แล้วรอผม"**
   _First message: "Read CLAUDE.md first, then wait for me."_

> `CLAUDE.md` คือกติกาของบรรณารักษ์ — พอ Claude อ่านแล้ว มันจะรู้ 3 ชั้น (raw/knowledge/wiki) และ 3 กฎเอง
> _`CLAUDE.md` is the librarian's rulebook — once Claude reads it, it knows the three layers and the three rules on its own._

---

## ขั้นที่ 3 — ทำ doc แรก / Step 3 — Make your first doc (grill)

1. พิมพ์: **"ช่วยสัมภาษณ์ผมเรื่อง … หน่อย"** (เติมเรื่องของคุณ เช่น "การนับสต๊อกสิ้นเดือน")
   _Type: "Help me interview about … " (fill in your topic, e.g. "month-end stock count")._
2. ตอบทีละคำถาม ด้วยคำพูดของคุณเอง — ไม่รู้ก็บอกว่าไม่รู้ได้
   _Answer one question at a time, in your own words. "I don't know" is a fine answer._
3. Claude บันทึกร่างไว้ที่ `knowledge/` (confidence: **MEDIUM**)
   _Claude saves a draft in `knowledge/` (confidence: MEDIUM)._
4. สลับไปที่ Obsidian → เห็นไฟล์ใหม่โผล่มาเลย
   _Switch to Obsidian → the new file appears._

---

## ขั้นที่ 4 — ตรวจให้เชื่อได้ / Step 4 — Check to make it trusted

1. ให้คนที่ 2 (หัวหน้า หรือคนที่รู้งานนั้น) อ่านทวน
   _Have a second person (a lead, or someone who knows the job) read it back._
2. บอก Claude: **"ตรวจ draft นี้กับ [ชื่อคนตรวจ]"**
   _Tell Claude: "Check this draft with [name]."_
3. Claude ทำตาม `skills/check.md` → ใส่ `checked_by` → เลื่อนไฟล์ขึ้น `wiki/` (confidence: **HIGH**)
   _Claude follows `skills/check.md` → fills `checked_by` → moves the file to `wiki/` (HIGH)._

---

## ใช้ประจำวัน / Everyday use

- ถามอะไรก็ได้: **"เราทำ X ยังไง?"** → Claude ตอบจาก `wiki/` ก่อน แล้วบอกที่มาเสมอ
  _Ask anything: "How do we do X?" → Claude answers from `wiki/` first and always says where it came from._
- เจออะไรใหม่: บอก Claude ให้จดลง `raw/` ไว้ก่อน แล้วค่อย grill ทีหลัง
  _Found something new: tell Claude to drop it in `raw/`, then grill it later._

---

## กฎเดียวที่ต้องจำ / The one rule (privacy)

**อย่าพิมพ์ ชื่อลูกค้า · เลขบัตร · เบอร์โทร · รหัสผ่าน**
_Don't type customer names, ID/card numbers, phone numbers, or passwords._

---

## 3 สกิล ขยับโน้ตข้าม 3 ชั้น / How the 3 skills move notes across the 3 layers

นี่คือสิ่งเดียวกับที่เดินให้ดูในสไลด์ S14 — _This mirrors the S14 walkthrough:_

| สกิล / Skill | ทำอะไร / What it does | ชั้น / Layers |
|---|---|---|
| **grill** | สัมภาษณ์ทีละคำถาม → เขียนร่าง · interview → draft | `raw/` → `knowledge/` (MEDIUM) |
| **check** | คนที่ 2 อ่านทวน → เลื่อนขึ้นชั้น · 2nd person verifies → promote | `knowledge/` → `wiki/` (HIGH) |
| **answer** | อ่าน `wiki/` ก่อน → `knowledge/` → `raw/` บอกที่มาเสมอ · reads trusted-first, always cites | อ่านทุกชั้น · reads all layers |

> ทางเดินไปทางเดียว: `raw/` → `knowledge/` → `wiki/` — ไม่มีอะไรขึ้นชั้น "เชื่อได้" โดยไม่มีคนตรวจ
> _One-way flow: `raw/` → `knowledge/` → `wiki/`. Nothing reaches the trusted shelf without a human vouching._

---

## ถ้าติดปัญหา / Troubleshooting

| อาการ / Symptom | ทำยังไง / Fix |
|---|---|
| Obsidian ไม่เห็นไฟล์ที่ Claude เขียน · Obsidian doesn't show the new file | รอสักครู่ / กดที่ไฟล์อื่นแล้วกลับมา — Obsidian อัปเดตเอง · wait a moment or click another file; it auto-refreshes |
| Claude เขียนแล้วไม่เห็นใน Obsidian · edits not showing | เช็กว่าเปิด **โฟลเดอร์เดียวกัน** จริง · confirm both apps opened the *same* folder |
| Claude ตอบมั่ว / ไม่ทำตามกติกา · Claude ignores the rules | บอกให้ **"อ่าน CLAUDE.md อีกครั้ง"** · tell it to "read CLAUDE.md again" |

---

ดูเพิ่ม / See also: `HOME.md` (เริ่มที่นี่) · `SETUP.md` (การเชื่อมต่อ) · `CLAUDE.md` (กติกา) · `skills/` (grill · check · answer)
