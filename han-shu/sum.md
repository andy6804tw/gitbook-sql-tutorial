# SUM 總和
使用 SUM( ) 函數來計算所有欄位的總和。

## 範例
我們已下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_price|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |99|
| 4 | Python |85|

##### 1. 計算所有總額

```sql
SELECT SUM(product_price) FROM Product 
```

![](/assets/img13-1.png)