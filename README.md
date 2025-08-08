# 🚀 C Advanced Training 
-Đây là repo chứa toàn bộ nội dung, tài liệu và bài thực hành

## Mục tiêu khóa học
- Nắm vững lập trình C advanced

### Nội dung training/
**Unit 1: Memory layout và static keywords**
- Memory layout: Text-->Initialize data--> Uniinitialed data--> Heap-->unillocated memmory-->Stack--> argv,env
<img width="446" height="520" alt="image" src="https://github.com/user-attachments/assets/940a5ec4-19c4-4ce1-bfc4-e45579ec95ae" />

  
**Unit 2:Biến và kiểu dữ liệu tự định nghĩa**

- Extern keyword: + cho phép các tệp mã nguồn khác nhau cùng một dự án chia sẻ và truy cập chung một biến toàn cục
                  + Đối với hàm không cần khai báo extern, gọi lại hàm
  
- Sự thông minh của gcc: cờ -02 -03
  
- Volatile: ngăn chặn và tối ưu hóa
  
- Register: báo cho trình biên dịch biến cụ thể sẽ được sử dụng thường xuyên. Biến sẽ được lưu trữ trong CPU register thay vì trong RAM ( chỉ áp dụng cho local variable)
  
- Cấu trúc struct: typedef, sử dụng dấu . cho đối tượng struct, -> cho con trỏ trỏ đến struct.
  
- Padding: để đảm bảo các thành viên được căn chỉnh đúng, trình biên dịch sẽ tự chèn các byte trống ( sử dụng _attribute((packed) để chọn chính xác số byte).
  
- Alignment: Căn chỉnh địa chỉ
+ Một uint16_t 2bytes nên được đặt ở địa chỉ chẵn ( chia hết cho 2)
+ Một uint32_t 4bytes nên được dặt ở địa chỉ chia hết cho
  
- Bit field: trường bit cho phép định nghĩa số bit chính xác của cấu trúc struct
  
- Cấu trúc Union: giống struct nhưng chỉ được lưu trữ tại một vùng bộ nhớ ( bị ghi đè )
+ Union - Type punning: kỹ thuật diễn giải lại các bit của một kiểu dữ liệu này như một kiểu dữ liệu khác
+ Tagged Union: tiết kiệm bộ nhớ
  
- Enum: kiểu liệt kê hằng số, tự động gán giá trị
  
**Unit 3:Standard IO**
- Formated I/O
<img width="1340" height="642" alt="image" src="https://github.com/user-attachments/assets/99b03454-d730-4bec-ad01-eb8f863b57c6" />
- String IO:
  <img width="646" height="265" alt="image" src="https://github.com/user-attachments/assets/15df527c-9b1b-47e2-b9a0-a852f6d680ab" />
- Tối ưu hiệu suất I/O:
  <img width="647" height="217" alt="image" src="https://github.com/user-attachments/assets/b63e10c7-3340-4907-80d6-cc49d566daee" />
  <img width="686" height="309" alt="image" src="https://github.com/user-attachments/assets/14f6eaf0-f59d-409f-9fb4-37f4a2aa4721" />

- Đọc ghi theo khối
  <img width="973" height="283" alt="image" src="https://github.com/user-attachments/assets/854f613e-0e17-407e-8fcd-008b3bb9de15" />
  
**Unit 4:Operators and Control structure**
- Các loại toán tử:
  <img width="1045" height="438" alt="image" src="https://github.com/user-attachments/assets/4b481814-638a-4dac-9f2b-38c4e756e186" />
- Toán tử thao tác với thanh ghi:
  <img width="1050" height="484" alt="image" src="https://github.com/user-attachments/assets/4f7136f9-d64f-4835-a795-bc4ff70172ad" />
- Câu lệnh điều kiện:
- Tối ưu hóa switch case Jumple table:
  <img width="1006" height="458" alt="image" src="https://github.com/user-attachments/assets/116fc7d5-2d30-48cf-91e8-0ff270a8543f" />
- Vòng lặp:
  <img width="1005" height="536" alt="image" src="https://github.com/user-attachments/assets/2fd60621-37d9-4ddb-99a4-efdce04323d3" />
**Unit 5:Array and Pointer**
- Mô hình bộ nhớ trong C và biến:
  <img width="1040" height="253" alt="image" src="https://github.com/user-attachments/assets/38c7d7b0-1939-4d33-85bb-0ab3d95b89bc" />
- Con trỏ:
  <img width="994" height="415" alt="image" src="https://github.com/user-attachments/assets/d1e73388-31a2-4305-9404-68712a6e6073" />
- khai báo con trỏ:
  <img width="1001" height="443" alt="image" src="https://github.com/user-attachments/assets/f1773774-2b22-46eb-a742-143fb8b54e3b" />
- Con trỏ Null:
  <img width="1037" height="475" alt="image" src="https://github.com/user-attachments/assets/aee8cfb5-3010-467e-895a-da92f8d9d8ad" />
- Toán thử tham chiếu ngược con trỏ:
  <img width="1024" height="335" alt="image" src="https://github.com/user-attachments/assets/ea0751ff-b9bb-42b3-a98d-6522d94be5d9" />
- Mảng và con trỏ:
  <img width="1002" height="409" alt="image" src="https://github.com/user-attachments/assets/6fecd437-3673-45b3-a2f9-ebd323783e7b" />
- Tên của mảng là một giá trị hằng không thể thay đổi
**Ứng dụng của con trỏ hàm**
- Con trỏ hàm:
  <img width="1017" height="477" alt="image" src="https://github.com/user-attachments/assets/21f3c33e-78c8-4ac6-bb6b-e9278b6a418e" />
- Callbacks:
 <img width="1008" height="499" alt="image" src="https://github.com/user-attachments/assets/0b640c05-d223-4381-9e7e-e27dfb09bfae" />
 <img width="1005" height="469" alt="image" src="https://github.com/user-attachments/assets/54729323-e779-4c3f-be31-8572380a21bd" />
- Bảng điều phối lệnh:
  <img width="1019" height="454" alt="image" src="https://github.com/user-attachments/assets/2059e800-e678-4474-b41d-2e13c321c824" />
**Unit 6:LINUX file system**
- Introduction:
  <img width="1036" height="485" alt="image" src="https://github.com/user-attachments/assets/36d8dde9-8f47-4c0a-89bb-b2843b399ead" />
- Bộ nhớ Cache
- File lock flock và file lock control fcntl
  **Unit 7:Debugging Tool GDB**


  






  
