---
title: "Cấu trúc điều khiển trong Java"
---

## Giới thiệu
Cấu trúc điều khiển giúp chương trình Java đưa ra quyết định và lặp lại các hành động theo điều kiện xác định.  
Bài viết này trình bày các cấu trúc điều khiển phổ biến như câu lệnh điều kiện và vòng lặp, giúp chương trình hoạt động linh hoạt và logic hơn.

---
## 1. Câu lệnh if – else
Câu lệnh if – else dùng để kiểm tra điều kiện và rẽ nhánh chương trình.

```java

int diem = 7;

if (diem >= 5) {
    System.out.println("Dat");
} else {
    System.out.println("Khong dat");
}
int ngay = 2;
```
## 2. Câu lệnh Switch - case
Switch – case giúp kiểm tra nhiều giá trị của một biến.

```java

int ngay = 2;

switch (ngay) {
    case 2:
        System.out.println("Thu Hai");
        break;
    case 3:
        System.out.println("Thu Ba");
        break;
    default:
        System.out.println("Ngay khac");
}
```
## Kết luận

#### Thông qua bài viết này, người học đã hiểu được vai trò của các cấu trúc điều khiển trong Java như câu lệnh điều kiện và vòng lặp.  
#### Những kiến thức này giúp chương trình xử lý logic hiệu quả và là nền tảng quan trọng trong việc phát triển các ứng dụng Java thực tế.
