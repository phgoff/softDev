# GIT  COMMANDS
คำสั่งพื้นฐาน การใช้ Git
### การเชื่อมต่อ local กับ Repository โดยการใช้ remote
```
git remote add origin "yourRepo"
```
### การสร้างไฟล์ .git
```
git init
```
### การเพิ่มไฟล์เข้าไปใน Repository  |  สามารถใช้ . เพื่อเป็นการเพิ่มไฟล์ทั้งหมด
```
git add README.md
```
### การเก็บข้อมูล
```
git commit -m "Your Comment"
```
### การส่งข้อมูลจาก Local ไปยัง Repository | -u คือ จำ parameter origin master เอ่ไว้
```
git push -u origin master
```
