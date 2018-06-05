# SUM 總和
使用 SUM( ) 函數來計算所有欄位的總和。

## 範例
我們已下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_stock|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |99|
| 4 | Python |85|
| 5 | Java |12|
| 6 | C語言 |14|


##### 1. 依據 `product_name` 計算該類庫存

```sql
SELECT product_name,SUM(product_stock) FROM product GROUP BY product_name
```

![](/assets/img14-1.png)