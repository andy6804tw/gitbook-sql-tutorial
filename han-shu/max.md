# MAX 最大值
使用 MAX( ) 函數來計算一個欄位的最大值。

## 範例
我們已下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_price|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |99|
| 4 | Python |85|

##### 1. 找出價格最貴的數

```sql
SELECT MAX(product_price) FROM Product 
```

![](/assets/img11-1.png)