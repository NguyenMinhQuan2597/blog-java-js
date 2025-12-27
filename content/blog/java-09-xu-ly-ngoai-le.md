---
title: "Xử lý ngoại lệ (Exception) trong Java"
---

## Giới thiệu

Trong quá trình chạy chương trình Java, lỗi có thể xảy ra như chia cho 0, nhập sai dữ liệu hoặc truy cập file không tồn tại.  
Java cung cấp cơ chế **Exception Handling** để xử lý các lỗi này một cách an toàn.

---

## 1. Exception là gì?

Exception là sự kiện xảy ra trong lúc chạy chương trình làm gián đoạn luồng thực thi bình thường.

#### Ví dụ lỗi chia cho 0:

```java
int a = 10 / 0;
```

## 2. Khối try – catch

Cú pháp xử lý ngoại lệ cơ bản:

```java
try {
    // code có thể gây lỗi
} catch (Exception e) {
    // code xử lý lỗi
}
```

#### Ví dụ:

```java
public class DemoException {
    public static void main(String[] args) {
        try {
            int a = 10 / 0;
            System.out.println(a);
        } catch (Exception e) {
            System.out.println("Co loi xay ra");
        }
    }
}
```

## 3. Khối finally

finally luôn được thực thi dù có lỗi hay không.

```java
try {
    int a = 10 / 2;
    System.out.println(a);
} catch (Exception e) {
    System.out.println("Loi");
} finally {
    System.out.println("Ket thuc chuong trinh");
}
```

## 4. Nhiều catch

```java
try {
    int[] arr = new int[3];
    arr[5] = 10;
} catch (ArithmeticException e) {
    System.out.println("Loi toan hoc");
} catch (ArrayIndexOutOfBoundsException e) {
    System.out.println("Loi truy cap mang");
}
```

## 5. Tạo Exception riêng

```java
class LoiTuTao extends Exception {
    public LoiTuTao(String message) {
        super(message);
    }
}
```

#### Sử dụng:

```java
public class DemoCustomException {
    static void kiemTraTuoi(int tuoi) throws LoiTuTao {
        if (tuoi < 18) {
            throw new LoiTuTao("Tuoi phai >= 18");
        }
    }

    public static void main(String[] args) {
        try {
            kiemTraTuoi(16);
        } catch (LoiTuTao e) {
            System.out.println(e.getMessage());
        }
    }
}
```

## Kết luận

#### + Exception giúp chương trình không bị crash

#### + Giúp xử lý lỗi rõ ràng, chuyên nghiệp

#### + Là kỹ năng rất quan trọng khi lập trình Java thực tế