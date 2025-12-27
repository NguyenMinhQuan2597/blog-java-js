---
title: "Mảng trong Java"
---
## Giới thiệu

Mảng (Array) trong Java dùng để **lưu nhiều giá trị cùng kiểu dữ liệu** trong một biến duy nhất.  
Mỗi phần tử trong mảng được truy cập thông qua **chỉ số (index)**, bắt đầu từ 0.

---
## 1. Khai báo và khởi tạo mảng

### Cách 1: Khai báo rồi gán giá trị
```java
int[] numbers = new int[5];
numbers[0] = 10;
numbers[1] = 20;
numbers[2] = 30;
numbers[3] = 40;
numbers[4] = 50;
```

### Cách 2: Khai báo và khởi tạo nhanh
```java
int[] numbers = {10, 20, 30, 40, 50};
```

## 2. Truy cập phần tử trong mảng
Sử dụng chỉ số (index) để truy cập phần tử:
```java
int[] numbers = {10, 20, 30};

System.out.println(numbers[0]); // 10
System.out.println(numbers[1]); // 20
System.out.println(numbers[2]); // 30
```
## 3. Duyệt mảng bằng vòng lặp for
```java
int[] numbers = {10, 20, 30, 40, 50};

for (int i = 0; i < numbers.length; i++) {
    System.out.println(numbers[i]);
}
```
## 4. Duyệt mảng bằng vòng lặp for-each
```java
int[] numbers = {10, 20, 30, 40, 50};

for (int x : numbers) {
    System.out.println(x);
}
```
## 5. Mảng chuỗi (String Array)
```java
String[] names = {"An", "Binh", "Cuong"};

for (String name : names) {
    System.out.println(name);
}
```
## 6. Tính tổng các phần tử trong mảng
```java
int[] numbers = {1, 2, 3, 4, 5};
int sum = 0;

for (int x : numbers) {
    sum += x;
}

System.out.println("Tong = " + sum);
```
## 7. Mảng 2 chiều
Mảng 2 chiều thường dùng để biểu diễn bảng, ma trận.
```java
int[][] matrix = {
    {1, 2, 3},
    {4, 5, 6}
};

for (int i = 0; i < matrix.length; i++) {
    for (int j = 0; j < matrix[i].length; j++) {
        System.out.print(matrix[i][j] + " ");
    }
    System.out.println();
}
```
## Kết luận

#### +Mảng giúp quản lý nhiều dữ liệu cùng kiểu

#### +Index của mảng bắt đầu từ 0

#### +Có thể dùng for hoặc for-each để duyệt mảng

#### +Mảng 2 chiều dùng cho bảng và ma trận

### -Mảng là kiến thức rất quan trọng, xuất hiện trong hầu hết chương trình Java.
