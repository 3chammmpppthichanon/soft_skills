# Soft Skills

กิจกรรมส่งเสริมทักษะการเรียนรู้

## วิธีการดาวน์โหลดและใช้งาน

### ขั้นตอนที่ 1: Fork Repository
1. เข้าไปที่หน้า GitHub ของ repository นี้
2. หาปุ่ม **Fork** ที่อยู่มุมขวาบนของหน้าเว็บ (ดังรูป)
3. กดปุ่ม Fork เพื่อสร้างสำเนาของ repository นี้ไว้ใน GitHub account ของคุณ

<img src="./assets/fork-button.png" alt="Fork Button" width="400">

### ขั้นตอนที่ 2: ดาวน์โหลดมาใช้งานในเครื่อง
1. ติดตั้ง Git (หากยังไม่มี): [https://git-scm.com](https://git-scm.com)
2. เปิด Command Prompt หรือ Terminal
3. ดาวน์โหลด repository ที่คุณ fork มาแล้ว:
   ```bash
   git clone https://github.com/<your-username>/soft_skills.git
   ```
   > **หมายเหตุ**: เปลี่ยน `<your-username>` เป็นชื่อ GitHub account ของคุณ
4. เข้าไปในโฟลเดอร์:
   ```bash
   cd soft_skills
   ```

## โครงการนี้ประกอบด้วยไฟล์ดังนี้:

- `/docs` - โฟลเดอร์สำหรับเก็บเอกสารต่างๆ
- `/problems` - โฟลเดอร์สำหรับเก็บไฟล์งานที่ได้รับมอบหมาย
- `README.md` - คำแนะนำและคู่มือการใช้งาน Git
- `SUMMARY.md` - สรุปผลการเรียนรู้และการพัฒนาทักษะ

## 📝 คู่มือการใช้งาน Git

### การจัดการ Branch

#### สร้าง Branch ใหม่
```bash
# สร้าง branch ใหม่และสลับไปใช้งาน
git checkout -b <branch-name>
```

#### สลับ Branch
```bash
# สลับไปยัง branch ที่มีอยู่แล้ว
git checkout <branch-name>

# กลับไปยัง branch หลัก
git checkout master
```

### 💾 การเตรียมไฟล์และบันทึกการเปลี่ยนแปลง (Staging & Commit)

#### เลือกไฟล์ที่จะบันทึก (Staging Area)
> **คำอธิบาย**: Staging Area คือพื้นที่กลางที่เก็บไฟล์ที่เราต้องการบันทึกในครั้งนี้ เหมือนการใส่ของลงตะกร้าก่อนไปจ่ายเงิน
```bash
# เลือกไฟล์เดี่ยวที่ต้องการบันทึก
git add <filename>

# เลือกไฟล์ทั้งหมดที่มีการเปลี่ยนแปลง
git add .
```

#### บันทึกการเปลี่ยนแปลง (Commit)
```bash
# บันทึกการเปลี่ยนแปลงพร้อมข้อความอธิบาย
git commit -m "<commit-message>"
```

### 📤 การส่งการเปลี่ยนแปลงไปยัง Remote Repository

```bash
# ส่งการเปลี่ยนแปลงไปยัง remote repository
git push origin -u <branch-name>
```
