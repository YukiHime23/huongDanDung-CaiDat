- Kiem tra phien ban \ `git --version`

Kiem tra lich su thay doi cua repository
 - `git log`
Kiem tra lich su thay doi cua repository voi 2 commit gan nhat
 - `git log -2`
Kien tra lich su rut gon
 - `git log --oneline`

Liet ke cac remote url hien tai
 - `git remote -v`

Tao 1 repository moi
 - `git init`

De clone 1 repository co san tren may cuc bo:
 - `git clone /duong-dan-den/repository/`

Neu repository o may chu khac:
 - `git clone tênusername@diachimaychu:/duong-dan-den/repository`

Thiet lap config, username va email
 - `git config --global user.name "<Tên nguoi dung>"`

 - `git config --global user.email "<Ðia chi mail>"`

tao mau cho phan xuat ra cua git
 - `git config --global color.ui auto`

thiet lap bi danh (aliases) gian luoc "checkout" thanh "co"
 - $ git config --global alias.co checkout
Liet ke nhung config dang su dung
 - $ git config --list

Tao repository tren local. Tao 1 thu muc tren may hoac dung 1 thu muc co san
Tro den thu muc do de dat thu muc duoi su quan ly cua git
 * Tao thu muc moi
 - $ mkdir `ten thu muc`
 - $ cd `duong dan`/`ten thu muc`
 - $ git init

Kiem tra trang thai working tree va index cua thu muc
 - $ git status

Chi dinh ( Dang ky ) file vao index trong <file>
 - $ git add <file>
co the chi dinh nhieu cai bang khoang trang phan cach
khi chi dinh "." trong tham so thi co the dang ky tat ca file trong index
 - $ git add .

Commit nhung thay doi
 - $ git commit -m "<ghi chu commit>"

Tao 1 repository tren GitHub
Clone len repostory vua tao
Dang ky url cua repostitory
 - $ git remote add origin https://[your_space_id].backlogtool.com/git/[your_project_key]/tutorial.git
push len 
 - $ git push -u origin master

Branches(nhanh)
Danh sach nhanh
 - $ git branch
Tao 1 nhanh moi
 - $ git checkout -b tennhanh
Tro lai nhanh master
 - $ git checkout master
Xoa nhanh
 - $ git branch -d tennhanh
push vs nhanh
 - $ git push origin <nhanh>
 
checkout branch mới trên remote
 - git fetch // update thông tin mới nhất trên remote
 - git switch <branch cần checkout>

Thay doi origin url
 - $ git remote set-url origin <https://github.com/repo.git>
 
Lay lay code da commit truoc day
- $ git reset --hard <ma commit ssh vd:0ad5a7a6>

- S git stash

Merge commit tu branch khac
 - $ git checkout master
 - $ git merge branch-name

De cap nhap thay doi tu remote repository
 - $ git pull origin master 

De tao SSH key
 - $ ssh-keygen -t rsa -b 4096 -C "luutruhocit@gmail.com"
De thay doi SSH key
 - $  ssh-keygen -p

Ket Noi
$ eval $(ssh-agent -s)
$ ssh-add 'keo tha file key'
