#Basic Git Commands

### ดึงข้อมูลจาก Server มายังเครื่อง  
```
$ git clone "repo"
```
### เชื่อมต่อ Local กับ Git Server
```
$ git remote add origin "repo" 
```
### การตรวจสอบสถานะ
```
$ git status
```
### การเพิ่มไฟล์ ถ้าใช้ . จะเพิ่มไฟล์ทั้งหมด จะได้สถานะ ติดตาม
```
$ git add file
```
### การเก็บไฟล์ 
```
$ git commit -m "Comment"
```
### ส่งไปยัง Server 
```
$ git push -u origin master   | * ครั้งต่อไปใช้แค่ git push 
```
### การตวรจสอบแล้วดึงไฟล์เข้ามาที่ local 
```
$ git pull
```
### Log out 
```
$ git config --global --unset user.name
$ git config --global --unset user.email
```
### File Undo
```
$ git checkout test.txt
```
### การ undo ไฟล์  โดยที่ไฟล์นั้น ได้ add ไปแล้ว  > จะได้สถานะ untrack
```
$ git reset HEAD test.txt
```
### การยกเลิกการ Commit
```
$ git reset --soft "HEAD^"  
```
### การดูรายละเอียด
```
$ git log --oneline
```
### Delete file, After committed
```
$ git rm test.txt
```
* Recovery
```
$ git reset HEAD test.txt
$ git checkout test.txt
```