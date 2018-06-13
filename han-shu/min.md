# MIN 最小值
使用 MIN( ) 函數來計算一個欄位的最小值。

## 範例
我們以下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_price|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |99|
| 4 | Python |85|

##### 1. 找出價格最便宜的數

```sql
SELECT MIN(product_price) FROM Product 
```

![](/assets/img12-1.png)