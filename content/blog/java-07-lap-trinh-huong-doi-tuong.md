---
title: "Collections trong Java"
---

## Giới thiệu

Collections trong Java là tập hợp các lớp và interface giúp lưu trữ, quản lý và xử lý dữ liệu hiệu quả hơn so với mảng truyền thống.

---

## 1. List trong Java

`List` là tập hợp có thứ tự, cho phép phần tử trùng lặp.

#### Ví dụ với `ArrayList`:

```java
import java.util.ArrayList;

public class DemoList {
    public static void main(String[] args) {
        ArrayList<String> ds = new ArrayList<>();

        ds.add("Java");
        ds.add("Python");
        ds.add("C++");

        System.out.println(ds);
    }
}
```

## 2. Duyệt List

```java
for (String mon : ds) {
    System.out.println(mon);
}
```

## 3. Set trong Java

```java
import java.util.HashSet;

public class DemoSet {
    public static void main(String[] args) {
        HashSet<Integer> so = new HashSet<>();

        so.add(1);
        so.add(2);
        so.add(2);

        System.out.println(so);
    }
}
```

## 4. Map trong Java

Map lưu dữ liệu theo dạng key – value.

#### Ví dụ với HashMap:

```java
import java.util.HashMap;

public class DemoMap {
    public static void main(String[] args) {
        HashMap<String, Integer> diem = new HashMap<>();

        diem.put("Toan", 8);
        diem.put("Ly", 7);

        System.out.println(diem.get("Toan"));
    }
}
```

## 5. Khi nào dùng List, Set, Map?

#### +List: cần thứ tự, cho phép trùng

#### +Set: không cho trùng

#### +Map: lưu theo cặp khóa – giá trị