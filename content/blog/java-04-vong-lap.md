---
title: "Vòng lặp trong Java"
---
## Giới thiệu
Trong lập trình Java, vòng lặp được sử dụng để thực hiện một đoạn chương trình nhiều lần mà không cần viết lặp lại mã nguồn. Việc sử dụng vòng lặp giúp chương trình ngắn gọn, dễ đọc và hiệu quả hơn. Bài học này giới thiệu các vòng lặp cơ bản trong Java như for, while và do…while.
---

## 1. Vòng lặp for
Vòng lặp for dùng khi biết trước số lần lặp.
```java
for (int i = 1; i <= 5; i++) {
    System.out.println("Gia tri i = " + i);
}
```
## 2. Vòng lặp while
Vòng lặp while dùng khi chưa biết trước số lần lặp.
```java
int i = 1;

while (i <= 5) {
    System.out.println("Gia tri i = " + i);
    i++;
}
```
## 3. Vòng lặp do - while 
Vòng lặp do – while luôn chạy ít nhất một lần.
```java
int j = 1;

do {
    System.out.println("Gia tri j = " + j);
    j++;
} while (j <= 5);
```
## Kết luận

### -Vòng lặp là kiến thức cực kỳ quan trọng trong Java và thường xuất hiện trong hầu hết chương trình thực tế.
### -Nắm vững các loại vòng lặp sẽ giúp bạn xử lý dữ liệu hiệu quả và viết code rõ ràng hơn.