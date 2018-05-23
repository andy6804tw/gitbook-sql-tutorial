# AVG 平均值
使用 AVG() 函數來計算平均值。

## 範例
我們已下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_price|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |99|
| 4 | Python |85|

##### 1.計算所有價錢平均

```sql
SELECT AVG(product_price) FROM Product 
```

![](/assets/img9-1.png)