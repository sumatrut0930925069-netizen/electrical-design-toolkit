# Electrical Design Toolkit — Standalone

เว็บไซต์เวอร์ชันภายนอกที่ไม่ต้องใช้ ChatGPT Plus และไม่มีค่าใช้จ่ายรายเดือนจากตัวเว็บไซต์

## ใช้งานในเครื่อง

เปิดไฟล์ `index.html` ด้วย Chrome, Edge หรือ Safari ได้ทันที ฟังก์ชันคำนวณ การพิมพ์ PDF การบันทึกโครงการ และการส่งออกไฟล์ทำงานในเบราว์เซอร์

เพื่อให้ระบบ Offline/PWA และกล้องทำงานครบ แนะนำเปิดผ่านเว็บเซิร์ฟเวอร์ HTTPS หรือรันในโฟลเดอร์นี้ด้วย:

`python -m http.server 8080`

จากนั้นเปิด `http://localhost:8080`

## เผยแพร่ฟรีด้วย GitHub Pages

1. สร้าง Public Repository ใหม่ใน GitHub
2. อัปโหลดไฟล์ทั้งหมดในโฟลเดอร์นี้ไว้ที่ root ของ repository
3. เปิด Settings > Pages
4. เลือก Deploy from a branch, branch `main`, folder `/ (root)`
5. รอประมาณ 1–5 นาที แล้วเปิด URL ที่ GitHub แสดง

## เผยแพร่ฟรีด้วย Cloudflare Pages

1. สร้าง Pages project และเชื่อม GitHub repository
2. Framework preset เลือก None
3. Build command เว้นว่าง
4. Output directory ใช้ `.`

## ข้อมูลและการสำรอง

- ข้อมูลโครงการและรูปภาพบันทึกใน IndexedDB ของเบราว์เซอร์แต่ละเครื่อง
- ก่อนเปลี่ยนเครื่องหรือล้าง Browser Data ให้กด “สำรอง” เป็น JSON
- นำไฟล์ JSON กลับเข้าระบบด้วยปุ่ม “นำเข้า”
- เว็บไซต์นี้ไม่ส่งข้อมูลโครงการไปยัง ChatGPT หรือเซิร์ฟเวอร์ภายนอก

## ข้อจำกัดทางวิศวกรรม

ใช้สำหรับ Preliminary Design ต้องยืนยันข้อมูล Utility, Manufacturer Catalogue, Installation Method, Protection Curve และ Approved Drawing ก่อนก่อสร้างจริง
