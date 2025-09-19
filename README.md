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
