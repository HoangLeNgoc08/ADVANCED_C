A) Quá trình biên dịch gồm 4 giai đoạn
1. Preprocessor (tạo ra các file.i)
- Copy toàn bộ mã nguồn đã thêm vào
- Xóa bỏ các chú thích
- Thay thế các Macro được định nghĩa ở file.c
- Các phần tử còn lại được giữa nguyên

2. Compiler ( tạo ra file.s)
- file.s là file assembly ( ngôn ngữ gần với phần cứng nhất)
3. Assembler (tạo ra file.0)
- File.o chứ ngôn ngữ nhị phân gần với ngôn ngữ máy nhất
4. Linker (tạo ra file.exe)
- Mỗi project có nhiều file.c muốn biên dịch được thì phải tạo liên kết chúng lại
- Tạo mỗi file.o cho mỗi file.c rồi sau đó liên kết lại để được file.exe

B) Macro là gì?

Có 3 loại Macro
- Chỉ thị bao hàm tiệp (#include)
- Chỉ thi đinh nghĩa (#define, #undef)
- Chỉ thi biên dich có điều kiện (#if, #elif, #else, #ifdef, #ifndef)

1. CHỉ thị bao hàm tiệp
- Có 2 loại
+ #include <thư viện> - Tìm kiếm ở trong phần cài đặt
+ #include <file chúng ta viết> - Tìm kiếm ở thư mục hiện hành
2. Chỉ thị định nghĩa 
- Dùng để định nghĩa tập hợp ( số, biểu thức, hàm,...)
- #undef dùng để xóa định nghĩa đã định nghĩa

Lưu ý: Khi định nghĩa nhiều dòng thì cuối hàng phải có dấu \ để liên kết các hàng lại với nhau
3. Chỉ thị biên dịch có điều kiện
- #if, #elif, #else : dùng để kiểm tra một Macro
- #ifdef : dùng để kiểm tra Macro đã định nghĩa chưa nếu RỒI thì thực thi
- #ifndef : dùng để kiểm tra Macro đã đinh nghĩa chưa nếu CHƯA thì thực thi 

Lưu ý:
- khi sử dụng #ifdef & #ifndef thì phải dùng #endif để kết thúc
- Sử dụng #ifndef để viết thư viện

Sự khác nhau giữa file.c và file.h

- file.h chứa khai báo (declaration) của các hàm, biến, hằng số, kiểu dữ liệu, macro. không chứa phần thân của hàm.

- file.c Chứa định nghĩa (definition) của hàm, tức là phần cài đặt chi tiết. Có thể chứa main() hoặc bất kỳ hàm xử lý logic nào.

