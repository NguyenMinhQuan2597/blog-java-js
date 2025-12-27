---
title: "Kế thừa và Đa hình trong Java"
---

## Giới thiệu

Kế thừa (Inheritance) và Đa hình (Polymorphism) là hai khái niệm cốt lõi của lập trình hướng đối tượng trong Java.  
Chúng giúp chương trình **tái sử dụng code**, **mở rộng dễ dàng** và **linh hoạt hơn**.

---

## 1. Kế thừa trong Java

Kế thừa cho phép một lớp con (subclass) **kế thừa thuộc tính và phương thức** của lớp cha (superclass).  
Java sử dụng từ khóa `extends` để thực hiện kế thừa.
#### Ví dụ lớp cha:

```java
class Nguoi {
    String ten;

    void chao() {
        System.out.println("Xin chao, toi la " + ten);
    }
}
```

#### Lớp con kế thừa lớp cha:

```java
class SinhVien extends Nguoi {
    String maSV;

    void hocTap() {
        System.out.println("Sinh vien dang hoc tap");
    }
}
```

## 2. Sử dụng đối tượng kế thừa

```java
public class Main {
    public static void main(String[] args) {
        SinhVien sv = new SinhVien();
        sv.ten = "Nguyen Van A";
        sv.maSV = "SV01";

        sv.chao();
        sv.hocTap();
    }
}
```

## 3. Ghi đè phương thức (Method Overriding)
Lớp con có thể ghi đè phương thức của lớp cha để thay đổi cách hoạt động.

```java
class SinhVien extends Nguoi {

    @Override
    void chao() {
        System.out.println("Xin chao, toi la sinh vien");
    }
}
```

## 4. Đa hình trong Java

Đa hình cho phép một phương thức có nhiều cách thực hiện khác nhau, tùy thuộc vào đối tượng cụ thể.

#### Ví dụ:

```java
Nguoi n = new SinhVien();
n.chao();
```
#### Dù biến n có kiểu Nguoi, nhưng phương thức chao() của SinhVien vẫn được gọi.


## 5. Ví dụ tổng hợp kế thừa và đa hình

```java
class DongVat {
    void keu() {
        System.out.println("Dong vat keu");
    }
}

class Cho extends DongVat {
    @Override
    void keu() {
        System.out.println("Cho keu gau gau");
    }
}

class Meo extends DongVat {
    @Override
    void keu() {
        System.out.println("Meo keu meo meo");
    }
}

public class Main {
    public static void main(String[] args) {
        DongVat dv1 = new Cho();
        DongVat dv2 = new Meo();

        dv1.keu();
        dv2.keu();
    }
}
```

## Kết luận

#### +Kế thừa giúp tái sử dụng code

#### +Đa hình giúp chương trình linh hoạt

#### +Hai khái niệm này là nền tảng của OOP trong Java

### -Nắm vững kế thừa và đa hình sẽ giúp bạn xây dựng các chương trình Java lớn và dễ mở rộng.