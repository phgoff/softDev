# GIT  COMMANDS
คำสั่งพื้นฐาน การใช้ Git
### การเชื่อมต่อ local กับ Repository โดยการใช้ remote
```
git remote add origin "yourRepo"
```
### การสร้างโฟลเดอร์ .git 
```
git init
```
### การเพิ่มไฟล์เข้าไปใน Repository  |  สามารถใช้ . แทนที่ชื่อไฟล์ จะเป็นการเพิ่มไฟล์ทั้งหมด
```
git add README.md
```
### การเก็บข้อมูล
```
git commit -m "Your Comment"
```
### การส่งข้อมูลจาก Local ไปยัง Repository | -u คือ จำ parameter origin master เอาไว้
```
git push -u origin master
```
### การดึงข้อมูลจาก Repository มายัง Local
```
git pull 
```
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
### Hide your Update
```
$ git add file
$ git stash    
$ git pull 
$ git stash pop  #recovery data 
$ git add > commit > push
```
### Branch
```
$ git branch yourbranch 	  	     // Create Branch
$ git checkour yourbranch		     //Move to branch yourbranch
$ git checkout -b yourbranch 	  	    //Create branch and move to new branch
$ git branch -a 			    // Status branch
$ git branch -d yourbranch 		   //Delete branch |Move to master first.
$ git push -u origin yourbranch	
-- Upload branch to master -- 
$ git checkout master 
$ git merge --no-ff dev 		 // merge dev to master | --no-ff 
``` 


