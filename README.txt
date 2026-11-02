Lhekcal — คู่มืออัปโหลดหน้า Privacy + Support ขึ้น GitHub Pages
=================================================================
(สำหรับ MAG ทำตามนี้ ใช้เวลาไม่ถึง 5 นาที ไม่ต้องรู้โค้ด)

มีไฟล์ในโฟลเดอร์นี้ 4 ไฟล์ที่ต้องอัปโหลด:
  1. index.html      -> หน้าซัพพอร์ตหลัก
  2. privacy.html    -> หน้า Privacy Policy
  3. app-ads.txt      -> ไฟล์ยืนยันโฆษณา AdMob (ต้องชื่อนี้เป๊ะ ห้ามเปลี่ยน)
  4. README.txt       -> ไฟล์คู่มือนี้เอง (ไม่จำเป็นต้องอัปโหลดก็ได้ แต่อัปก็ไม่เสียหาย)

ขั้นตอน (5 คลิกหลัก):
-----------------------
1. เข้า https://github.com แล้ว login ด้วยบัญชี GitHub ของตัวเอง
   (ถ้ายังไม่มีบัญชี ให้สมัครฟรีก่อน — ใช้ email ส่วนตัวของ MAG ได้)

2. กดปุ่ม "+" มุมขวาบน -> เลือก "New repository"
   - Repository name: lhekcal-support
   - เลือก "Public" (ต้องเป็น public ไม่งั้น GitHub Pages ใช้ไม่ได้ฟรี)
   - ไม่ต้องติ๊ก "Add a README file"
   - กด "Create repository"

3. ในหน้า repo ที่เพิ่งสร้าง กด "Add file" -> "Upload files"
   -> ลากไฟล์ทั้ง 4 ไฟล์จากโฟลเดอร์นี้มาวางในหน้าเว็บ
   -> เลื่อนลงกด "Commit changes"

4. ไปที่แท็บ "Settings" (บนสุดของ repo) -> เมนูซ้าย "Pages"
   - หัวข้อ "Build and deployment" -> "Source" เลือก "Deploy from a branch"
   - "Branch" เลือก "main" และช่องโฟลเดอร์เลือก "/ (root)"
   - กด "Save"

5. รอ 1-2 นาที แล้วรีเฟรชหน้า Settings -> Pages อีกครั้ง
   จะเห็นข้อความ "Your site is live at ..." พร้อม URL

URL ที่คาดว่าจะได้ (ถ้าตั้งชื่อ repo และ username ตรงตามนี้):
  หน้าซัพพอร์ต : https://nuttavutwet-collab.github.io/lhekcal-support/
  หน้า Privacy : https://nuttavutwet-collab.github.io/lhekcal-support/privacy.html

  *** หมายเหตุสำคัญ: URL จริงขึ้นกับ "username" ของบัญชี GitHub ที่ใช้สร้าง repo
  ถ้า username ไม่ใช่ nuttavutwet-collab ให้แทนที่ด้วย username จริงของบัญชีนั้น
  รูปแบบคือ: https://<username>.github.io/lhekcal-support/

หลังได้ URL แล้ว เอาไปใส่ที่ 2 จุดนี้:
-----------------------
(ก) AdMob -> Privacy & messaging -> UMP consent message
    -> ช่อง "Privacy policy URL" ใส่ URL หน้า privacy.html ด้านบน
    -> กด Publish อีกครั้ง (ตอนนี้ป้ายแดง Fix ควรหายไป)

(ข) App Store Connect -> เลือกแอป Lhekcal -> App Information
    -> "Privacy Policy URL" ใส่ URL หน้า privacy.html
    -> ถ้ามีช่อง "Support URL" แยก (อยู่ตอนสร้างเวอร์ชัน/Version Information)
       ใส่ URL หน้าซัพพอร์ต (index.html, ไม่ต้องมี /privacy.html ต่อท้าย)

ตรวจสอบก่อนใช้งานจริง:
-----------------------
- เปิด URL ทั้ง 2 หน้าในเบราว์เซอร์ดูว่าโหลดได้ ไม่มีหน้า 404
- app-ads.txt ต้องเปิดได้ที่: https://<username>.github.io/lhekcal-support/app-ads.txt
  (เนื้อหาควรเป็นบรรทัดเดียว: google.com, pub-6955019542182219, DIRECT, f08c47fec0942fa0)
  - หมายเหตุ: app-ads.txt ของแอป iOS ตามสเปก IAB ต้องอยู่ที่ root domain ของเว็บไซต์ของผู้พัฒนา
    (เช่น developer website ที่ใส่ใน App Store Connect) ไม่ใช่ที่ repo GitHub Pages เสมอไป
    ถ้า Lhekcal ยังไม่มี developer website อื่น ให้ใช้ลิงก์ GitHub Pages นี้ไปก่อน
    แต่ถ้าในอนาคตมีเว็บไซต์หลักของแอป ควรย้าย app-ads.txt ไปไว้ที่ root ของเว็บนั้นด้วย
- ลองเปิดบนมือถือ (จอแคบ) ดูว่าตัวหนังสือไม่ล้นจอ อ่านง่าย

ถ้าติดปัญหาขั้นตอนไหน ถ่ายสกรีนช็อตส่งมาได้เลย
