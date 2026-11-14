# LAP ลีออโต้เพ้นท์: Website Content Brief (for dev)

Site: https://lap-frontend-hazel.vercel.app

**How to read this file**
- Instructions are in English. **Text in `「 」` brackets goes on the website exactly as written (Thai).** Don't translate or rephrase it.
- New photos are in `/photos` in this repo. Copy them to `public/images/garage/`.
- `[ ]` = info still missing. If it isn't filled in before launch, **delete that whole line**. Don't put placeholder text on the live site.

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
| Brands | Remove the "ชำนาญ Benz · Alphard" chip and the whole "ชำนาญรถหรู" section. Replace with the new "All brands" section (section 2.4) |
| Draft labels | Delete every small pink note ("ฉบับร่าง…", "รอ…", "ตัวอย่าง…") |
| Promotions | Hide the whole promotions section until the owner gives real promos |
| Stock photos | Stop using `found/damaged-front.jpg` and `found/headlight.webp`. Only use the shop's real photos |

---

## 2. Sections (top to bottom)

### 2.1 Hero
- **Background photo:** `photos/paint-booth-porsche-spraying.jpg` (new, replaces `paint-booth-red-side.jpg`). Vertical photo, so use `object-position: center 60%` on desktop.
- Small badge: 「อู่เคาะพ่นสี · บางใหญ่ นนทบุรี」
- H1 line 1: 「ชนมา เฉี่ยวมา」
- H1 line 2 (orange highlight): 「ซ่อมจบที่ LAP」
- Subtitle: 「เคาะ พ่น อบสี เคลมประกันหรือเงินสด รับทุกยี่ห้อ」
- Subtitle line 2: 「ไม่แพงอย่างที่คิด โทรถามได้เลย」 *(from the owner's own FB posts, so keep this wording)*
- Button 1 (primary, big): 「โทร 081-542-8799」 → `tel:0815428799`
- Button 2: 「ส่งรูปทางไลน์」 → LINE (see LINE note above)
- Chips: 「เปิด จ.–ส. 08:00–17:00」 · 「บางแม่นาง บางใหญ่」 · 「รับทุกยี่ห้อ รวมรถ EV」

### 2.2 Highlights strip (NEW, 4 small cards under hero)
| Icon idea | Title | Text |
|---|---|---|
| receipt | 「บอกราคาก่อนซ่อม」 | 「รู้ราคาก่อน ตกลงแล้วค่อยเริ่มงาน」 |
| spray | 「ห้องอบสีระบบปิด」 | 「ฝุ่นไม่ลง สีเรียบ เงาเนียน」 |
| palette | 「ผสมสีเองในอู่」 | 「Glasurit / Axalta ผสมตามรหัสสีรถ สีไม่ด่าง ไม่เป็นขอบ」 |
| check | 「เช็คทุกจุดก่อนส่งมอบ」 | 「ดูงานกับลูกค้าให้เรียบร้อยก่อนส่งรถทุกคัน」 |

### 2.3 Services (3 cards, keep current layout)
- Section label: 「บริการของเรา」
- H2: 「งานหนัก งานเบา เราทำหมด」
- Sub: 「ตั้งแต่รอยขูดนิดเดียว ไปจนถึงชนหนักต้องดึงแท่น」

| Card | Photo | Title | Text |
|---|---|---|---|
| 1 | `body-shell-rebuild.jpg` (keep) | 「เคาะ ดึง ซ่อมตัวถัง」 | 「บุบ ยุบ บิด ดึงกลับเข้ารูปเดิม ร่องประตู ฝากระโปรง ต้องได้ระยะเท่ากัน กันชนแตกก็ซ่อมหรือเปลี่ยนให้」 |
| 2 | `photos/fb-paint-booth-sedan-primer.jpg` (new) | 「ทำสีรถยนต์」 | 「ทำสีเฉพาะจุด ทั้งชิ้น หรือทำสีรอบคัน เก็บงานละเอียด ขัดเงาให้ก่อนส่งรถ」 |
| 3 | `inspection.jpg` (keep) | 「เคลมประกัน / เงินสด」 | 「มีใบเคลมก็เอารถเข้ามาได้เลย เราคุยกับประกันให้ ไม่มีประกันก็จ่ายเงินสดได้ บอกราคาก่อนทุกครั้ง」 |

### 2.4 All brands (NEW, replaces "ชำนาญรถหรู")
- Section label: 「รับทุกยี่ห้อ」
- H2: 「รถญี่ปุ่น รถยุโรป รถไฟฟ้า ซ่อมได้ทุกคัน」
- Sub: 「เก๋ง กระบะ SUV รถตู้ จะรถบ้านหรือรถหรูก็ดูแลเท่ากันทุกคัน」
- **Brand row** (plain text pills, or grey logos if we get them):
  「Toyota · Honda · Isuzu · Mazda · Nissan · Mitsubishi · Mercedes-Benz · BMW · Volvo · Porsche · BYD · Tesla · MG · ORA · และยี่ห้ออื่นๆ」
- **3 cards:**

| Photo | Title | Text |
|---|---|---|
| `benz-repair.jpg` (keep) | 「รถยุโรป」 | 「สีเงิน สีดำ สีมุก ผสมเทียบสีทีละคันให้กลืนกับสีเดิม」 |
| `photos/tow-truck-van-arrival-front.jpg` (new) | 「รถตู้ / SUV」 | 「Alphard, Vellfire, Fortuner คันใหญ่แค่ไหนก็เข้าห้องอบได้」 |
| `photos/ev-workshop-floor.jpg` (new) | 「รถไฟฟ้า EV」 | 「ซ่อมรถไฟฟ้าได้มาตรฐาน ทั้งงานตัวถังและงานสี เคลมประกันได้เหมือนรถทั่วไป」 |

### 2.5 Insurance claims (keep layout, change text)
- Section label: 「งานเคลมประกัน」
- H2: 「เคลมที่นี่ ไม่ต้องวิ่งเรื่องเอง」
- Sub: 「แจ้งประกันว่าจะซ่อมที่ LAP ลีออโต้เพ้นท์ ที่เหลือเราจัดการให้」
- Logos: all current ones **minus LMG**. Count text: 「รับเคลม [count] บริษัท」. Show Roojai as a separate badge: 「อู่ในเครือรู้ใจ」
- **Steps: cut from 5 to 4:**
  1. 「แจ้งเคลม」: 「โทรแจ้งประกัน จดเลขเคลมไว้」
  2. 「เอารถเข้าอู่」: 「ช่างเช็คความเสียหาย ถ่ายรูปเก็บไว้」
  3. 「รออนุมัติ」: 「อู่ส่งราคาให้ประกันเอง ไม่ต้องตามเรื่อง」
  4. 「ซ่อมเสร็จ รับรถ」: 「ดูงานกับช่างให้พอใจก่อนเซ็นรับ」
- Documents title: 「เอกสารที่ต้องใช้」
- Documents list: 「บัตรประชาชน · ใบขับขี่ · สำเนาเล่มทะเบียน · กรมธรรม์ · ใบเคลม · ใบแจ้งความ (ถ้าประกันขอ)」
- Under list: 「เอกสารไม่ครบ โทรถามก่อนได้ 081-542-8799」

### 2.6 Our team (REPLACES "อู่จริง ทีมช่างจริง" / owner quote block)
This section should feel like a family business, not a corporate one. Use the new photos.

- Section label: 「ทีมงาน LAP」
- H2: 「ทีมงานพร้อมให้บริการ」 *(the owner's own phrase from FB)*
- Sub: 「ช่างเคาะ ช่างสี ช่างประกอบ ประชุมงานกันทุกเช้า ทุกคันมีคนรับผิดชอบชัดเจน」
- **Big photo (left):** `photos/team-briefing-1.jpg`
- **Owner quote card (right, orange card like now):**
  - Quote: 「รถลูกค้าก็เหมือนรถเรา ไม่เนียนไม่ส่ง」
  - Name: 「เสี่ยลี · เจ้าของอู่」 *(get the owner's OK on the quote before launch)*
- **Gallery row (4 small photos with Thai captions):**

| Photo | Caption |
|---|---|
| `photos/fb-team-briefing-3.jpg` | 「ประชุมงานเช้า」 |
| `paint-mixing-axalta.jpg` (keep) | 「ห้องผสมสี」 |
| `photos/team-briefing-2.jpg` | 「ทีมช่าง」 |
| `photos/fb-final-check-before-delivery.jpg` | 「เช็คงานก่อนส่งรถ」 |

- **Team trip strip (NEW, small block at bottom of this section):**
  - Photo: `photos/team-trip-group-1.jpg` (wide, rounded corners). Optional: make it a mini carousel with `team-trip-group-2.jpg` and `team-trip-candid.jpg`
  - Title: 「ทริปพนักงานประจำปี」
  - Text: 「ทำงานหนักทั้งปี ก็ต้องพักผ่อนด้วยกัน ทีมที่มีความสุข งานก็ออกมาดี」
  - ⚠️ The shop sign in these photos still shows the old name and number. That's fine for a team photo, but **don't use these as the location/shopfront photo**

### 2.7 How we paint (keep 3 steps, swap photos + text)
- H2: 「กว่าจะเงาได้ขนาดนี้」

| Step | Photo | Title | Text |
|---|---|---|---|
| 1 | `photos/tow-truck-van-arrival-rear.jpg` (new) | 「รับรถ」 | 「ขับมาไม่ได้ เรียกรถสไลด์ไปรับได้」 |
| 2 | `jaguar-primer-booth.jpg` (keep) | 「ลงพื้น」 | 「ขัดสีเก่า โป๊ว ลงพื้น เตรียมผิวให้เรียบก่อน」 |
| 3 | `photos/paint-booth-porsche-spraying.jpg` (new) | 「พ่น อบ ขัดเงา」 | 「พ่นสีจริง เคลียร์ทับ อบให้แห้งสนิท ขัดเงาแล้วประกอบกลับ」 |

### 2.8 Our work (before/after)
- **Remove the slider and its instruction text** (stock photos, different cars).
- Replace with a simple photo grid, H2: 「งานจริงจากในอู่」
- Photos: `jaguar-arrival-tow.jpg`, `jaguar-primer-booth.jpg`, `photos/fb-paint-booth-sedan-primer.jpg`, `photos/fb-final-check-before-delivery.jpg`
- Caption under grid: 「รูปจริงทุกรูป ไม่ใช่ภาพประกอบ」

### 2.9 FAQ (all items must have an answer)
- H2: 「ถามบ่อย」

| Question | Answer |
|---|---|
| 「ต้องนัดก่อนไหม?」 | 「ไม่ต้อง เข้ามาได้เลยในเวลาทำการ แต่โทรบอกก่อนจะได้ไม่ต้องรอ」 |
| 「ขอราคาก่อนได้ไหม?」 | 「ได้ ส่งรูปมาให้ดู ช่างบอกราคาคร่าวๆ ให้ฟรี ราคาจริงแจ้งอีกทีตอนเห็นรถ」 |
| 「ไม่มีประกัน จ่ายเงินสดได้ไหม?」 | 「ได้ เคลมประกันหรือเงินสดก็ซ่อมได้ บอกราคาก่อนเริ่มงานทุกครั้ง」 |
| 「รถไฟฟ้ารับซ่อมไหม?」 | 「รับ BYD, Tesla, MG, ORA และยี่ห้ออื่นๆ ทั้งงานตัวถังและงานสี」 |
| 「ซ่อมกี่วันเสร็จ?」 | 「แผลเล็ก [ ] วัน ชนหนัก [ ] วัน ช่างบอกวันรับรถให้ตั้งแต่ตอนประเมิน」 |
| 「รถขับมาไม่ได้ทำยังไง?」 | 「โทรมา เราส่งรถสไลด์ไปรับให้」 |
| 「มีรับประกันงานไหม?」 | 「งานสีรับประกัน [ ] ปี」 |

### 2.10 Map / Contact
- H2: 「มาที่อู่」
- Address: 「98/63 หมู่ 4 ต.บางแม่นาง อ.บางใหญ่ นนทบุรี 11140」
- Phones: 「โทร 081-542-8799」 (big) · 「099-396-9187」 (smaller)
- Hours: 「เปิด จันทร์–เสาร์ 08:00–17:00 · หยุดวันอาทิตย์」
- Remove "รอยืนยันหมุดแผนที่" note. Keep the Google Maps button: 「นำทางด้วย Google Maps」

### 2.11 Bottom CTA band
- H2: 「รถเป็นรอย อย่าปล่อยไว้นาน」
- Sub: 「เคลมประกันหรือเงินสด โทรถามได้เลย ไม่แพงอย่างที่คิด」
- Big number: 「081-542-8799」
- Buttons: 「โทรเลย」 · 「ส่งรูปทางไลน์」

### 2.12 Footer
- 「LAP ลีออโต้เพ้นท์ · เคาะ พ่น อบสี เคลมประกัน · รับทุกยี่ห้อ · บางใหญ่ นนทบุรี」
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

Alt text: write it in Thai, short, describing the photo (e.g. 「ช่างพ่นสีรถในห้องอบสี」).
