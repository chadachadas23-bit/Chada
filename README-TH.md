# Stock Inventory Dashboard (GitHub Pages)

## ไฟล์
- `index.html` — หน้า Dashboard
- `stock-data.json` — ข้อมูลที่แปลงจากรายงาน Stock ที่ผู้ใช้ส่งมา

## เปิดทดสอบบนเครื่อง
แนะนำเปิดผ่าน local web server เพราะหน้าเว็บโหลด JSON ด้วย fetch:
1. ติดตั้ง Python หากยังไม่มี
2. เปิด Terminal / Command Prompt ในโฟลเดอร์นี้
3. รัน `python -m http.server 8000`
4. เปิด `http://localhost:8000`

## เผยแพร่ด้วย GitHub Pages
1. สร้าง Repository ใหม่ใน GitHub
2. อัปโหลดทั้ง `index.html` และ `stock-data.json` ไว้ที่ root ของ repository
3. เข้า Settings → Pages
4. ใน Build and deployment เลือก Deploy from a branch
5. เลือก branch `main` และ folder `/(root)` แล้วกด Save
6. รอ GitHub สร้างลิงก์ Pages และเปิดทดสอบ

## ข้อควรระวัง
- GitHub Pages โดยทั่วไปเป็นเว็บไซต์สาธารณะ ข้อมูลนี้เป็นรายงาน Stock ภายใน โปรดได้รับอนุญาตจากองค์กรก่อนเผยแพร่
- Dashboard จัดกลุ่มแบรนด์โดยอัตโนมัติจากชื่อสินค้า จึงอาจมีบางรายการอยู่ใน “ไม่ระบุแบรนด์” หรือจัดกลุ่มคลาดเคลื่อน ควรตรวจสอบก่อนใช้สั่งซื้อ
- KPI และกราฟใช้คอลัมน์ `NET_BALANCE`; สถานะใกล้หมดตั้งเกณฑ์ตัวอย่างไว้ที่ 1–5 หน่วย สามารถปรับภายหลังได้
