# การใช้งาน git

### ตั้งค่าเริ่มต้นด้วยการ กรอก user และ email

```bash
git config --global user.name "username"
git config --global user.email "user@email.com"
```

### เปิดการใช้งาน git ในโฟลเดอร์โปรเจคที่ต้องการ

```bash
cd ./myproject
git init
```

### เพิ่มไฟล์ที่มีการเปลี่ยนแปลง

```bash
# เพิ่มไฟล์ทั้งหมดในโฟลเดอร์
git add .

# เพิ่มทีละไฟล์
git add filename.ext
```

### ยกเลิกการเพิ่มไฟล์

```bash
git reset
```

### เช็คสถานะการเปลี่ยนแปลงของไฟล์

```bash
git status
```

### บันทึกการเปลี่ยนแปลงของไฟล์

```bash
git commit -m "ข้อความ"
```

### ดูประวัติการบันทึก

```bash
git log
```

### ยกเลิกการแก้ไขไฟล์

ยกเลิกการแก้ไขไฟล์ กลับไปใช้ข้อมูลตอนที่บันทึกล่าสุด

```bash
git checkout -- filename.ext
```

### ลบ commit

```bash
# ลบ commit ล่าสุด
git reset --hard HEAD^
```

### ลบ branch

```bash
git branch -d branch-name
```

### รวม branch

```bash
# กลับไป branch หลักที่จะรวม ตัวอย่างคือ master
git checkout master

# รวม branch dev เข้ากับ master
git merge dev
```

### update repository บน github ให้ตรงกับ local

```bash
git push origin -f
```
