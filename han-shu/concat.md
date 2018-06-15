# CONCAT 字串連接
有的時候，我們有需要將由不同欄位獲得的資料串連在一起，可以使用 CONCAT()。

```sql
CONCAT(欄位1,欄位2,...)
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

##### 1. `id` 與 `name` 字串相連

```sql
SELECT CONCAT(product_id,product_name) FROM Product
```

![](/assets/img19-1.png)