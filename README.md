# Git Tutorial

1. Cấu hình Git  
- Cấu hình Git  
 Lấy và đặt các biến cấu hình để kiểm soát tất cả các khía cạnh của giao diện và hoạt động của Git.  
 Đặt tên:  
 **git config –global user.name “Tên người dùng”**  
 Đặt email:  
 **git config –global user.email “hmq@gmail.com”**  
 Đặt trình soạn thảo mặc định (opinion):  
 **git config –global core. editor "code --wait"**    
 Kiểm tra cài đặt:  
 **git config -list**    
 - Git Alias  
Thiết lập bí danh cho mỗi lệnh:  
**git config –global alias.co checkout**      
**git config –global alias.br branch**     
**git config –global alias.ci commit**    
**git config –global alias.st status**    

2. Bắt đầu một dự án  
- **Git init**    
Tạo kho lưu trữ cục bộ:  
**git init**  
- **Git clone**   
**Tạo bản sao cục bộ** của kho lưu trữ máy chủ.  
**git clone**  

3. Thay đổi cục bộ
- **Git add**
**Thêm file** vào vùng dàn dựng (Chỉ mục – index):  
**git add Tên file**  
**Thêm tất cả file** của kho vào vùng dàn (Chỉ mục):  
**git add .**  
- **Git commit**  
**Ghi lại** hoặc chụp nhanh các file một cách vĩnh viễn trong lịch sử phiên bản **với một tin nhắn.**  
  - **git commit -m “Tin nhắn của commit”** 

4. Theo dõi các thay đổi
-  Git diff  
Theo dõi các thay đổi chưa được dàn dựng: $ git diff  
Theo dõi các thay đổi đã được dàn dựng nhưng chưa được commit:  
**git diff –staged**  
Theo dõi các thay đổi sau khi commit một file:  
**git diff HEAD**  
Theo dõi các thay đổi giữa hai lần commit:  
**git diff branch**  
-  Git Diff:  
**git diff <nhánh 2>**  
- **Git status:**  
Hiển thị trạng thái của thư mục làm việc và vùng dàn dựng.  
**git status**  
-  Git show Hiển thị các đối tượng:
**git show**

5. Lịch sử commit
Git log
Hiển thị các commit gần đây nhất và trạng thái của phần đầu:
git log
Hiển thị đầu ra dưới dạng một commit trên mỗi dòng:
git log -oneline
Hiển thị các file đã được sửa đổi:
git log –stat
Hiển thị các file đã sửa đổi với vị trí :
git log -p
Git blu
Hiển thị sửa đổi trên mỗi dòng của file:
git blu <tên file>

6. file bỏ qua(gitignore)
.gitignore
Chỉ định các file không được theo dõi mình muốn mà Git nên bỏ qua.
Tạo .gitignore:
touch .gitignore
Liệt kê các file bị bỏ qua:
git ls-files -i –exclude-standard
