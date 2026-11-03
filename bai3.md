### **Bài 3 : Xử lý Sự cố Giao diện Website Doanh nghiệp** 

### **1\. Nguyên nhân lỗi hiển thị** 

- Chi tiết Box Model đang bị sai:  
+ Content: Chiều rộng chiếm tới 65% \!important.  
+ Margin: Đang bị đặt giá trị âm margin-right: \-20px.  
     
- Lý do bị đè:  
+ Thuộc tính margin-right: \-20px kéo phần tử kế tiếp ("Danh sách video") lùi về bên trái, đè trực tiếp lên phần tử này.

+ Kết hợp với chiều rộng 65% quá lớn khiến kích thước quá lớn so với không gian hiển thị.

**2\. Giải pháp khắc phục**

- Tại bảng Styles chọn div.lesson-content, chỉnh sửa các thuộc tính sau:  
1. Bỏ margin âm:  
- Đổi margin-right: \-20px thành margin-right: 20px   
2. Kiểm soát lại độ rộng   
- Giảm độ rộng width: 65% \!important; xuống khoảng 55% \- 60% để chừa đủ không gian cho khung bên phải.  
   
   

