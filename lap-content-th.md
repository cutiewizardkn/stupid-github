# LAP ลีออโต้เพ้นท์: Website Content Brief (for dev)

Site: https://lap-frontend-hazel.vercel.app

**How to read this file**
- Instructions are in English. **Text in 「 」 goes on the website exactly as written (Thai).** Don't translate or rephrase it. Don't include the 「 」 brackets themselves.
- New photos: small previews are inside this doc (section 3). Full-size files are in the GitHub repo cutiewizardkn/stupid-github, folder `photos/` (branch claude/zealous-ptolemy-l1xh1v). Copy them to `public/images/garage/`.
- `[ ]` = info still missing. If it isn't filled in before launch, **delete that whole line**. Don't put placeholder text on the live site.
- Tone: the shop talks about itself as 「ทางอู่」 or 「ทางเรา」 and calls customers 「ลูกค้า」. Keep it that way if you add any text.

## 0. Still need from the garage

- New LINE ID (current link uses the old 089 number)
- Warranty length and repair times (fills the [ ] in the FAQ)
- Owner OK on the quote in section 2.6 (name on site is confirmed: 「เสี่ยลี」)
- Is the big EV workshop with BYD banners (team meeting + EV photos) LAP's own shop, a second branch, or a partner centre? If it's not theirs, don't present it as LAP
- Insurer count after removing LMG

---

## 1. Global changes (do these first)

| What | Change |
|---|---|
| Shop name | Replace "L.A.P. ศูนย์ซ่อมสีตัวถังมาตรฐาน" and "ซากุระ การาจ" everywhere with 「LAP ลีออโต้เพ้นท์」: header logo text, `<title>`, meta description, image alt text, footer, © line |
| Main phone | **「081-542-8799」**: use this for every call button, the sticky header button and `tel:0815428799` links. This is the owner's number (เสี่ยลี), so it must be the most visible number |
| Second phone | 「099-396-9187」: show only in the map/contact section and the footer |
| Remove old numbers | Delete 089-500-8567 and 02-120-6629 everywhere, including meta description and alt text |
| LINE button | Current link `line.me/R/ti/p/~0895008567` uses the old number. **Ask for the new LINE ID.** Until we have it, change the LINE buttons to call 081-542-8799 |
| Insurance | Remove LMG (`lmg.png`) from the hero card and the claims section. Update the company count to match the logos left |
| Brands | Remove the "ชำนาญ Benz · Alphard" chip and the whole "ชำนาญรถหรู" section. Replace with the new "All brands" section (2.4) |
| Draft labels | Delete every small pink note ("ฉบับร่าง…", "รอ…", "ตัวอย่าง…") |
| Promotions | Hide the whole promotions section until the owner gives real promos |
| Stock photos | Stop using `found/damaged-front.jpg` and `found/headlight.webp`. Only use the shop's real photos |
| Meta description | 「LAP ลีออโต้เพ้นท์ อู่ซ่อมสีและตัวถังรถยนต์ บางใหญ่ นนทบุรี รับเคลมประกันและงานเงินสด รับซ่อมทุกยี่ห้อ รวมรถไฟฟ้า EV โทร 081-542-8799」 |

---

## 2. Sections (top to bottom)

### 2.1 Hero
- **Background photo:** `photos/paint-booth-porsche-spraying.jpg` (new, replaces `paint-booth-red-side.jpg`). Vertical photo, so use `object-position: center 60%` on desktop.
- Small badge: 「อู่ซ่อมสีและตัวถัง บางใหญ่ นนทบุรี」
- H1 line 1: 「ซ่อมสี เคาะพ่นสี ซ่อมตัวถัง」
- H1 line 2 (orange highlight): 「รับเคลมประกัน และงานเงินสด」
- Subtitle: 「ทางอู่รับซ่อมรถทุกยี่ห้อ ทั้งรถญี่ปุ่น รถยุโรป และรถไฟฟ้า EV พ่นและอบสีในห้องพ่นสีระบบปิด ราคาไม่แพงอย่างที่คิด」
- Subtitle line 2: 「ส่งรูปรถมาทางไลน์ ทางอู่ประเมินราคาเบื้องต้นให้ฟรี」
- Button 1 (primary, big): 「โทร 081-542-8799」 → `tel:0815428799`
- Button 2: 「ส่งรูปประเมินราคาทางไลน์」 → LINE (see LINE note above)
- Chips: 「เปิดจันทร์–เสาร์ 08:00–17:00 น.」 · 「ต.บางแม่นาง อ.บางใหญ่」 · 「รับซ่อมทุกยี่ห้อ รวมรถ EV」

### 2.2 Why us strip (NEW, 4 small cards under hero)
- Section title: 「ทำไมต้องซ่อมกับทางเรา」

| Icon idea | Title | Text |
|---|---|---|
| receipt | 「แจ้งราคาก่อนซ่อมทุกคัน」 | 「ทางอู่ประเมินและแจ้งราคาให้ลูกค้าทราบก่อน ลูกค้าตกลงแล้วจึงเริ่มงาน」 |
| spray | 「ห้องพ่นสีระบบปิด」 | 「พ่นและอบสีในห้องพ่นสีมาตรฐาน ป้องกันฝุ่น ผิวสีเรียบเนียน」 |
| palette | 「ผสมสีตามรหัสสีรถ」 | 「ใช้สี Glasurit และ Axalta ผสมในอู่ตามรหัสสีรถแต่ละคัน ให้สีเข้ากับสีเดิม」 |
| check | 「ตรวจเช็คงานก่อนส่งมอบ」 | 「ทางอู่ตรวจเช็คความเรียบร้อยทุกจุดร่วมกับลูกค้าก่อนส่งมอบรถ」 |

### 2.3 Services (3 cards, keep current layout)
- Section label: 「บริการของเรา」
- H2: 「บริการซ่อมสีและตัวถังครบวงจร」
- Sub: 「ตั้งแต่รอยขีดข่วน รอยบุบเล็กน้อย ไปจนถึงรถที่เกิดอุบัติเหตุหนัก」

| Card | Photo | Title | Text |
|---|---|---|---|
| 1 | `body-shell-rebuild.jpg` (keep) | 「ซ่อมตัวถัง」 | 「เคาะ ดึง แก้ไขตัวถังที่บุบ ยุบ หรือเสียรูปจากอุบัติเหตุ ปรับร่องประตูและฝากระโปรงให้ได้ระยะ ซ่อมหรือเปลี่ยนกันชนที่แตกเสียหาย」 |
| 2 | `photos/fb-paint-booth-sedan-primer.jpg` (new) | 「ทำสีรถยนต์」 | 「รับทำสีเฉพาะจุด ทำสีทั้งชิ้น และทำสีรอบคัน ขัดเคลือบเงาหลังทำสีทุกครั้ง」 |
| 3 | `inspection.jpg` (keep) | 「เคลมประกัน / งานเงินสด」 | 「รับรถเคลมประกัน ทางอู่ประสานงานกับบริษัทประกันให้ทั้งหมด หากไม่ใช้ประกันก็ซ่อมแบบเงินสดได้ แจ้งราคาก่อนซ่อมทุกครั้ง」 |

### 2.4 All brands (NEW, replaces "ชำนาญรถหรู")
- Section label: 「รับซ่อมทุกยี่ห้อ」
- H2: 「รับซ่อมสีและตัวถังรถทุกยี่ห้อ ทุกรุ่น」
- Sub: 「รถเก๋ง รถกระบะ SUV รถตู้ ทั้งรถญี่ปุ่น รถยุโรป และรถไฟฟ้า ทางอู่ดูแลด้วยมาตรฐานเดียวกันทุกคัน」
- **Brand row** (plain text pills, or grey logos if we get them):
  「Toyota · Honda · Isuzu · Mazda · Nissan · Mitsubishi · Mercedes-Benz · BMW · Volvo · Porsche · BYD · Tesla · MG · ORA · และยี่ห้ออื่นๆ」
- **3 cards:**

| Photo | Title | Text |
|---|---|---|
| `benz-repair.jpg` (keep) | 「รถยุโรป」 | 「Mercedes-Benz, BMW, Volvo, Porsche งานสีเงิน สีดำ และสีมุก ทางอู่ผสมและเทียบสีให้ใกล้เคียงสีเดิมมากที่สุด」 |
| `photos/tow-truck-van-arrival-front.jpg` (new) | 「รถตู้ / SUV」 | 「Alphard, Vellfire, Fortuner และรถขนาดใหญ่ ห้องพ่นสีของทางอู่รองรับได้」 |
| `photos/ev-workshop-floor.jpg` (new) | 「รถไฟฟ้า EV」 | 「รับซ่อมสีและตัวถังรถไฟฟ้า BYD, Tesla, MG, ORA และยี่ห้ออื่นๆ รับเคลมประกันเช่นเดียวกับรถทั่วไป」 |

### 2.5 Insurance claims (keep layout, change text)
- Section label: 「เคลมประกัน」
- H2: 「รับเคลมประกัน ทางอู่ดูแลเรื่องเคลมให้」
- Sub: 「ลูกค้าเพียงแจ้งบริษัทประกันว่าต้องการซ่อมที่ LAP ลีออโต้เพ้นท์ ทางอู่จะประสานงานส่วนที่เหลือให้ทั้งหมด」
- Logos: all current ones **minus LMG**. Count text: 「รับเคลมประกัน [count] บริษัท」. Show Roojai as a separate badge: 「อู่ในเครือรู้ใจ」
- Steps title: 「ขั้นตอนการเคลม」 (**cut from 5 steps to 4**)
  1. 「แจ้งเคลม」: 「แจ้งบริษัทประกันและรับเลขเคลม」
  2. 「นำรถเข้าอู่」: 「ทางอู่ตรวจสภาพและถ่ายรูปความเสียหาย」
  3. 「รออนุมัติ」: 「ทางอู่ส่งใบเสนอราคาให้บริษัทประกันพิจารณา」
  4. 「ซ่อมและรับรถ」: 「ซ่อมเสร็จ ลูกค้าตรวจเช็คงานก่อนรับรถ」
- Documents title: 「เอกสารที่ต้องเตรียม」
- Documents list: 「สำเนาบัตรประชาชน · สำเนาใบขับขี่ · สำเนาทะเบียนรถ · กรมธรรม์ประกันภัย · ใบเคลม · ใบแจ้งความ (กรณีบริษัทประกันขอ)」
- Under list: 「หากไม่แน่ใจเรื่องเอกสาร สอบถามทางอู่ได้ที่ 081-542-8799」

### 2.6 Our team (REPLACES "อู่จริง ทีมช่างจริง" / owner quote block)
This section should feel like a family business, not a corporate one. Use the new photos.

- Section label: 「ทีมงานของเรา」
- H2: 「ทีมงานพร้อมให้บริการ」 *(the owner's own phrase from FB)*
- Sub: 「ทีมช่างเคาะ ช่างสี และช่างประกอบ ประชุมวางแผนงานกันทุกเช้า เพื่อให้รถของลูกค้าทุกคันเสร็จตามกำหนด」
- **Big photo (left):** `photos/team-briefing-1.jpg`
- **Owner quote card (right, orange card like now):**
  - Quote: 「ทางเราดูแลรถลูกค้าทุกคันเหมือนรถของเราเอง ซ่อมให้เรียบร้อยก่อนส่งมอบทุกครั้ง」
  - Name: 「เสี่ยลี · เจ้าของอู่」 *(get the owner's OK on the quote before launch)*
- **Gallery row (4 small photos with Thai captions):**

| Photo | Caption |
|---|---|
| `photos/fb-team-briefing-3.jpg` | 「ประชุมงานช่วงเช้า」 |
| `paint-mixing-axalta.jpg` (keep) | 「ห้องผสมสี」 |
| `photos/team-briefing-2.jpg` | 「ทีมช่าง」 |
| `photos/fb-final-check-before-delivery.jpg` | 「ตรวจเช็คงานก่อนส่งมอบ」 |

- **Team trip strip (NEW, small block at bottom of this section):**
  - Photo: `photos/team-trip-group-1.jpg` (wide, rounded corners). Optional: make it a mini carousel with `team-trip-group-2.jpg` and `team-trip-candid.jpg`
  - Title: 「ทริปท่องเที่ยวของทีมงาน」
  - Text: 「ขอบคุณทีมงานทุกคนที่ตั้งใจทำงานกันมาตลอด」
  - ⚠️ The shop sign in these photos still shows the old name and number. That's fine for a team photo, but **don't use these as the location/shopfront photo**

### 2.7 How we paint (keep 3 steps, swap photos + text)
- H2: 「ขั้นตอนการทำสี」

| Step | Photo | Title | Text |
|---|---|---|---|
| 1 | `photos/tow-truck-van-arrival-rear.jpg` (new) | 「รับรถเข้าอู่」 | 「กรณีรถขับมาเองไม่ได้ ทางอู่มีบริการรถสไลด์ไปรับ」 |
| 2 | `jaguar-primer-booth.jpg` (keep) | 「เตรียมพื้นผิว」 | 「ขัดสีเดิม โป๊ว และพ่นสีรองพื้นให้ผิวเรียบก่อนทำสีจริง」 |
| 3 | `photos/paint-booth-porsche-spraying.jpg` (new) | 「พ่นสี อบสี ขัดเงา」 | 「พ่นสีและเคลียร์ในห้องพ่นสี อบให้สีแห้งสนิท แล้วขัดเงาก่อนประกอบชิ้นส่วนกลับ」 |

### 2.8 Our work (before/after)
- **Remove the slider and its instruction text** (stock photos, different cars).
- Replace with a simple photo grid, H2: 「ผลงานของทางอู่」
- Photos: `jaguar-arrival-tow.jpg`, `jaguar-primer-booth.jpg`, `photos/fb-paint-booth-sedan-primer.jpg`, `photos/fb-final-check-before-delivery.jpg`
- Caption under grid: 「ภาพจากงานจริงภายในอู่」

### 2.9 FAQ (all items must have an answer)
- H2: 「คำถามที่พบบ่อย」

| Question | Answer |
|---|---|
| 「ต้องนัดล่วงหน้าหรือไม่」 | 「ลูกค้าสามารถนำรถเข้ามาได้ในเวลาทำการ แนะนำให้โทรแจ้งทางอู่ก่อน เพื่อความสะดวกและไม่ต้องรอนาน」 |
| 「ขอประเมินราคาก่อนได้หรือไม่」 | 「ได้ ลูกค้าส่งรูปความเสียหายทั้งระยะใกล้และระยะไกล พร้อมแจ้งยี่ห้อและรุ่นรถมาทางไลน์ ทางอู่จะประเมินราคาเบื้องต้นให้ฟรี ราคาจริงจะแจ้งอีกครั้งหลังตรวจสภาพรถ」 |
| 「ไม่มีประกัน ซ่อมแบบเงินสดได้หรือไม่」 | 「ได้ ทางอู่รับทั้งงานเคลมประกันและงานเงินสด และแจ้งราคาให้ทราบก่อนเริ่มซ่อมทุกครั้ง」 |
| 「รับซ่อมรถไฟฟ้าหรือไม่」 | 「รับซ่อมสีและตัวถังรถไฟฟ้า เช่น BYD, Tesla, MG, ORA และยี่ห้ออื่นๆ」 |
| 「ใช้เวลาซ่อมกี่วัน」 | 「ขึ้นอยู่กับความเสียหาย งานเล็กประมาณ [ ] วัน งานใหญ่ประมาณ [ ] วัน ทางอู่จะแจ้งวันรับรถให้ทราบตั้งแต่ตอนประเมินราคา」 |
| 「รถขับมาที่อู่ไม่ได้ ทำอย่างไร」 | 「โทรแจ้งทางอู่ได้ที่ 081-542-8799 ทางอู่มีบริการรถสไลด์ไปรับรถ」 |
| 「มีรับประกันงานซ่อมหรือไม่」 | 「ทางอู่รับประกันงานสี [ ] ปี」 |
| 「ระหว่างซ่อมจะทราบความคืบหน้าได้อย่างไร」 | 「ทางอู่จะแจ้งความคืบหน้าให้ลูกค้าทราบเป็นระยะจนกว่าจะซ่อมเสร็จ」 |

### 2.10 Map / Contact
- H2: 「ที่ตั้งอู่」
- Address: 「98/63 หมู่ 4 ต.บางแม่นาง อ.บางใหญ่ จ.นนทบุรี 11140」
- Phones: 「โทร 081-542-8799」 (big) · 「099-396-9187」 (smaller)
- Hours: 「เปิดวันจันทร์–เสาร์ 08:00–17:00 น. · ปิดวันอาทิตย์」
- Remove the "รอยืนยันหมุดแผนที่" note. Keep the Google Maps button: 「นำทางด้วย Google Maps」

### 2.11 Bottom CTA band
- H2: 「รถมีรอยบุบ รอยขีดข่วน ปรึกษาทางอู่ได้」
- Sub: 「เคลมประกันหรือเงินสด ติดต่อสอบถามได้ ราคาไม่แพงอย่างที่คิด」
- Big number: 「081-542-8799」
- Buttons: 「โทรหาทางอู่」 · 「ส่งรูปทางไลน์」

### 2.12 Footer
- 「LAP ลีออโต้เพ้นท์ · ซ่อมสีและตัวถังรถยนต์ · รับเคลมประกัน · รับซ่อมทุกยี่ห้อ」
- 「โทร 081-542-8799 · 099-396-9187」
- 「© 2026 LAP ลีออโต้เพ้นท์」
- Remove "ตัวอย่างเว็บไซต์ ยังไม่เผยแพร่จริง" and the top preview banner before launch.

---

## 3. New photo list (`/photos`)

| File | What it shows | Used in |
|---|---|---|
| `paint-booth-porsche-spraying.jpg` | Painter spraying white Porsche in booth | Hero, Paint step 3 |
| `fb-paint-booth-sedan-primer.jpg` | Sedan in primer inside booth | Services card 2, Work grid |
| `ev-workshop-floor.jpg` | Workshop floor with EVs being repaired | Brands → EV card |
| `tow-truck-van-arrival-front.jpg` | Black luxury van arriving on tow truck | Brands → Van card |
| `tow-truck-van-arrival-rear.jpg` | Same van unloading at shop | Paint step 1 |
| `fb-final-check-before-delivery.jpg` | Staff + customer checking SUV before handover | Team gallery, Work grid |
| `team-briefing-1.jpg` / `-2.jpg` / `fb-team-briefing-3.jpg` | Morning team meeting | Team section |
| `team-trip-group-1.jpg` / `-2.jpg` / `team-trip-candid.jpg` | Staff company trip (orange shirts) | Team trip strip |

Alt text: write it in Thai, short, describing the photo (e.g. 「ช่างพ่นสีรถในห้องพ่นสีของทางอู่」).

---

## 4. Wording references (20 Thai garages checked)

The Thai copy follows how these garages actually write (「ทางอู่」, 「ลูกค้า」, 「ประเมินราคาเบื้องต้นให้ฟรี」, 「งานเงินสด」, 「ห้องพ่นสีมาตรฐาน」, 「รับประกันงานสี」):

- SEC Body & Paint (รามอินทรา) · ขวัญฉัตร การาจ · Car Glossy (ชลบุรี) · วันสไมล์สตาร์ ออโต้สปอร์ต · K Auto Colour (บางกรวย)
- Lee Auto Premium · อู่ไรส์ซิ่ง (risingimex.com) · S.K. Service · U.C.S. Car Service · Refine Plus (วิภาวดี)
- นครพิงค์เวอร์คช็อพ (เชียงใหม่) · ธนาวุฒิออโต้เซอร์วิส (tooncarpaint.online) · สุขสันต์ ออโต้เซอร์วิส (นวมินทร์) · อู่ฉัตรเพชร คาร์เพ้นท์ · Diamond Auto Service
- JK Auto Garage (บางบ่อ) · อู่รุ่งทรัพย์ (ฮ้อการาจ) · NKC Motors ศูนย์ซ่อมสีและตัวถัง · ABLE Body and Paint · BYD Hi-Class ศูนย์ซ่อมสีและตัวถัง
