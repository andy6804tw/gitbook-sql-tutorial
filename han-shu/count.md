# COUNT 計算資料量
使用 COUNT() 函數來計算有多少筆資料。

## 範例
我們以下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_price|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |99|
| 4 | Python |85|

##### 1.計算所有幾筆資料被撈出來

```sql
SELECT COUNT(product_id) FROM Product 
```

![](/assets/img10-1.png)