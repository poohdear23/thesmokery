# The Smokery — Landing Page (public)

หน้า Landing Page สาธารณะของ **The Smokery / BEEFCON** ทำไว้เพื่อให้ search engine และผู้ช่วย AI (ChatGPT / Gemini / Perplexity / Copilot) หาเจอเวลาลูกค้าถามเรื่อง "เบคอนเนื้อวัว"

> ⚠️ repo นี้ **สาธารณะ** — แยกจาก repo KB ของ The Smokery (ซึ่ง local-only / ห้าม push)
> เนื้อหาทั้งหมดผ่านการ sanitize แล้ว: **ไม่มีตัวเลขต้นทุน · ไม่มีเลขสูตรภายใน · ไม่มีที่อยู่บ้าน**

## โครงไฟล์
- `index.html` — หน้าเดียวจบ + JSON-LD schema (Organization / WebSite / Product / FAQPage) + meta/OG
- `robots.txt` — เปิดทางให้ AI crawler (GPTBot, ClaudeBot, PerplexityBot, Google-Extended ฯลฯ)
- `sitemap.xml` — sitemap สำหรับ index
- `llms.txt` — สรุปเว็บให้ LLM อ่านเร็ว (แนวปฏิบัติใหม่)
- `.nojekyll` — ปิด Jekyll ให้ GitHub Pages เสิร์ฟไฟล์ตรง ๆ
- `assets/og.jpg` — *(ยังต้องใส่)* รูปสำหรับ link preview (OG image) — แนะนำใช้ **รูปสินค้าจริง**

## โดเมน
ตอนนี้ตั้ง canonical/sitemap/OG เป็น `https://poohdear23.github.io/thesmokery/` (GitHub Pages ฟรี)
ถ้า日后ซื้อโดเมนเอง ให้ find & replace URL เก่า → ใหม่ทั้ง 4 ไฟล์ แล้วผูก Custom Domain ใน Settings → Pages

## Deploy (GitHub Pages)
1. สร้าง repo สาธารณะใหม่ชื่อ `thesmokery` บน GitHub (บัญชี poohdear23)
2. push โฟลเดอร์นี้ขึ้นไป
3. Settings → Pages → Source = branch `main` / `/ (root)` → Save
4. รอ build แล้วเปิด URL ที่ขึ้น

## กฎ copy ที่ต้องรักษา (sync จาก KB brand-brief)
- ห้ามเลขสูตรภายใน ("สูตร #03") · ห้ามคำว่า "5 วัตถุดิบ/5 ingredients"
- ห้ามเคลมฮาลาล/organic/vegetarian/gluten-free/อย.
- ห้ามพูดถึง discount/โปร/COD · ห้ามแต่งราคา/เลข batch/ข้ออ้างสุขภาพที่ไม่มีใน KB
- เคลมที่พูดได้: "ไม่ฉีดน้ำ ไม่หดหายเมื่อทอด" (ห้ามต่อเป็น %) · "ฉ่ำ" (เชิงสัมผัสเท่านั้น)
- ถ้าเปลี่ยน brand/positioning → อัปเดต Notion KB + ไฟล์นี้พร้อมกัน
