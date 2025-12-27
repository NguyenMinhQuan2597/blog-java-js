---
title: "Phương thức (Method) trong Java"
---
## Giới thiệu

Trong Java, phương thức (method) là một khối lệnh dùng để thực hiện một chức năng cụ thể.  
Việc sử dụng phương thức giúp chương trình **dễ đọc, dễ bảo trì và tái sử dụng code**.

---

## 1. Cú pháp khai báo phương thức

Cú pháp chung:

```java
kieuTraVe tenPhuongThuc(danhSachThamSo) {
    // các câu lệnh
}
```
#### Ví dụ phương thức tính tổng hai số:

```java
static int tinhTong(int a, int b) {
    return a + b;
}
```
## 2. Gọi phương thức
Sau khi khai báo, ta có thể gọi phương thức trong hàm main hoặc phương thức khác.

```java
public static void main(String[] args) {
    int ketQua = tinhTong(3, 5);
    System.out.println("Tong = " + ketQua);
}
```
## 3. Phương thức không trả về giá trị (void)

```java
static void xinChao() {
    System.out.println("Xin chao Java");
}
```
#### Gọi phương thức:

```java
xinChao();
```
## 4. Phương thức có tham số

```java
static void hienThiTen(String ten) {
    System.out.println("Xin chao " + ten);
}
```

## 5. Phương thức trả về giá trị

```java
static double tinhDiemTrungBinh(double a, double b) {
    return (a + b) / 2;
}
```

## 6. Ví dụ tổng hợp

```java
public class MethodDemo {

    static int cong(int a, int b) {
        return a + b;
    }

    static void hienThi() {
        System.out.println("Demo phuong thuc trong Java");
    }

    public static void main(String[] args) {
        hienThi();
        int kq = cong(4, 6);
        System.out.println("Ket qua = " + kq);
    }
}
```

## Kết luận

#### +Phương thức giúp chia nhỏ chương trình
#### +Tái sử dụng code hiệu quả
#### +Là nền tảng cho lập trình hướng đối tượng trong Java

### -Phương thức là kiến thức rất quan trọng, cần nắm vững trước khi học OOP.
