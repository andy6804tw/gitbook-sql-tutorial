# LENGTH 長度
在 SQL 中，長度函數是用來找出一個字串的長度。長度函數的語法如下：

```sql
LENGTH(str)
```

## 範例
我們以下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_stock|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |99|
| 4 | Python |85|
| 5 | Java |12|
| 6 | C語言 |14|

##### 1. 取得 `product_name` 每筆字串長度

```sql
SELECT product_name, LENGTH(product_name) FROM Product
```

> 中文字佔3個字元，英文字佔1個字元

![](/assets/img22-1.png)