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


  
