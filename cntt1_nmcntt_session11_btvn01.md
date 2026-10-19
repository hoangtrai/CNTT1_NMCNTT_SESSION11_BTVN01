

# Phần 1: Phân tích lỗi : 
## 1.  lỗi cụ thể của từng dòng tiêu đề trong bảng trên :
|Tiêu đề|Các lỗi|Cấp heading đúng|Lý do khiến Auto TOC rỗng/sai|
|:-:|:-:|:-:|:-:|
|**1. Thông tin chung hội nghị**|Chữ thường, cỡ 16, In đậm, Tô vàng|**heading 1**|Sử dụng định dạng thủ công |
|**1.1. Tên hội nghị**| Normal + in đậm + cỡ 14|**heading 2**|Là style `Normal` kèm định dạng trực tiếp. Auto TOC bỏ qua dòng này.|
|**1.2. thời gian và địa điểm**|Normal + in đậm + cỡ 14|**Heading 2** |Tương tự dòng 1.1, vẫn mang bản chất kiểu văn bản thường|
|**Cơ cấu ban tổ chức**|Chữ thường, cỡ 16, In đậm, Tô vàng|**Heading 1**|Sử dụng định dạng thủ công trên nền `Normal`. Auto TOC bỏ qua|
|**2. Ban Nội dung**|Normal + cỡ 13 + màu xanh|**Heading 2**|Định dạng màu sắc/cỡ chữ thủ công trên nền `Normal`|
|**2.1.1. Tiểu ban Kỹ thuật**|Normal + cỡ 13 + màu xanh|**Heading 3**| _(Đang bị nhầm)_Vừa bị lỗi định dạng thủ công (nền `Normal`), vừa bị xác định sai phân cấp logic trong bảng|
|**3. Lịch trình sự kiện**|Normal, không định dạng gì cả|**Heading 1**|Chưa được gắn thẻ `Heading 1`. Được hiểu là một đoạn văn bản thô bình thường.|
## 2. định dạng thủ công khiến Auto TOC không hoạt động vì : 
- **Định dạng thủ công** — ví dụ như bôi đen chữ rồi đổi cỡ chữ, chỉnh in đậm — chỉ thay đổi vẻ ngoài thị giác  chứ **không thay đổi bản chất Style của đoạn văn
-  Vì vậy, khi bấm _References → Table of Contents_, Word quét toàn bộ tài liệu nhưng không tìm thấy bất kỳ thẻ Heading nào, dẫn đến Mục lục xuất ra rỗng
## 3. cơ chế hoạt động của tính năng quét tiêu đề : 
1. thu thập dữ liệu 
2. phân tích cú pháp và nhận diện 
3. trích xuất 
## 4. việc nhầm H2 sang H3 hay ngược lại sẽ làm mục lục trông sai lệch về mặt thụt đầu dòng : 
-  **2.1.1. Tiểu ban Kỹ thuật** bị gán nhầm thành **Heading 2**, trên mục lục nó sẽ nằm **thẳng hàng lề trái với mục 2.1. Ban Nội dung** . Điều này phá vỡ cấu trúc logic phân cấp, khiến người đọc hiểu nhầm "Tiểu ban Kỹ thuật" là một mục ngang hàng với "Ban Nội dung" chứ không phải là bộ phận trực thuộc.
    
# Phần 2: Sửa lỗi & Nghiệm thu : 
## 1. các bước thao tác để sửa đúng cấu trúc Heading cho cả 7 dòng tiêu đề trong bảng trên : 
 - ###  Bước 1: Sửa chuẩn cho từng dòng tiêu đề

    1.  **Dòng `1. Thông tin chung hội nghị`:**
    
        -   Bôi đen dòng → Bấm **Ctrl + Shift + N** 
        
        -   Bấm **Ctrl + Alt + 1** để gán **Heading 1**.
        
   2.  **Dòng `1.1. Tên hội nghị`:**
    
       -   Bôi đen dòng → Bấm **Ctrl + Shift + N**.
        
       -   Bấm **Ctrl + Alt + 2** để gán **Heading 2**.
        
   3.  **Dòng `1.2. Thời gian & địa điểm`:**
    
       -   Bôi đen dòng → Bấm **Ctrl + Shift + N**.
        
       -   Bấm **Ctrl + Alt + 2** để gán **Heading 2**.
        
      4.  **Dòng `2. Cơ cấu ban tổ chức`:**
    
          -   Bôi đen dòng → Bấm **Ctrl + Shift + N**.
        
           -   Bấm **Ctrl + Alt + 1** để gán **Heading 1**.
        
    5.  **Dòng `2.1. Ban Nội dung`:**
    
           -   Bôi đen dòng → Bấm **Ctrl + Shift + N**.
        
        -   Bấm **Ctrl + Alt + 2** để gán **Heading 2**.
        
   6.  **Dòng `2.1.1. Tiểu ban Kỹ thuật`:**
    
        -   Bôi đen dòng → Bấm **Ctrl + Shift + N**.
        
       -   Bấm **Ctrl + Alt + 3** để gán đúng cấp **Heading 3** 
        
   7.  **Dòng `3. Lịch trình sự kiện`:**
    
        -   Bôi đen dòng → Bấm **Ctrl + Alt + 1** để gán **Heading 1**.
        

#### Bước 2: Chèn lại Mục lục tự động (Auto TOC)

-   Đặt con trỏ chuột tại vị trí trang đầu tiên.
    
-   Vào thẻ **References** → Chọn **Table of Contents** → Chọn mẫu **Automatic Table 1** hoặc **Automatic Table 2**.
## 2. bẫy dữ liệu 
-   Câu trả lời: **không**. Mục lục tự động trong Word **không tự động thay đổi số trang ngay lập tức** 
    
-   **Mô tả thao tác cập nhật:**
    

        
-   **Phím tắt nhanh:**
    

    

