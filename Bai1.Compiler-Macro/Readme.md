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
- CHỉ thi đinh nghĩa (#define, #undef)
- Chỉ thi biên dich có điều kien (#if, #elif, #else, #ifdef, #ifndef)


