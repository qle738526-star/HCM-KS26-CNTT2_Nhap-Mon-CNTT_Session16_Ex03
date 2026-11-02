  
**Bài 3 : Xử lý Sự cố Giao diện Website Doanh nghiệp**   
Phần 1: Báo cáo phân tích (I/O)

* Khung "Nội dung" : Bị phình to hơn Width khai báo do cộng dồn Padding và Border.  
*   
* Khung "Video": Đang bị gán Margin âm, khiến nó tự kéo giật lùi và chui vào diện tích của khung nội dung.  
* 

Phần 2: Thiết kế giải pháp (Chỉnh tại bảng Styles)

1. Khóa kích thước: Thêm box-sizing: border-box; cho cả hai khung để Padding/Border tự động ép vào trong Width, không làm phình phần tử.  
2.   
3. Xóa lỗi lề: Trả các thông số margin âm của khung Video về margin: 0;.  
4.   
5. Chia lại tỷ lệ: Set Width theo phần trăm an toàn (VD: Khung nội dung 65%, Khung video 30%).  
6.   
7. Tạo khoảng cách tĩnh: Chọn thẻ cha bọc ngoài hai khung, thêm display: flex; và justify-content: space-between; để tự động đẩy hai khung ra xa nhau một cách hoàn hảo.  
   

