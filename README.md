# Git Commands
## คำสั่งพื้นฐาน
### ดึงข้อมูลจาก Server มายังเครื่อง  
```
$ git clone "repo"
```
### เชื่อมต่อ Local กับ git Server
```
$ git remote add origin "repo" 
```
### การตรวจสอบสถานะ
```
$ git status
```
### การเพิ่มไฟล์ ถ้าใช้ . จะเพิ่มไฟล์ทั้งหมด จะได้ สถานะ ติดตาม
```
$ git add file
```
### การเก็บไฟล์ 
```
$ git commit -m "Comment"
```
### ส่งไปยัง Server 
```
$ git push -u origin master 
  * ครั้งต่อไปใช้แค่ git push 
```
### การตวรจสอบแล้วดึงไฟล์เข้ามาที่ local 
```
$ git pull
```
### Log out 
```
$ git config --global --unset user.name | git config --global --unset user.email
```
### การ undo ไฟล์ 
```
$ git checkout test.txt
```
