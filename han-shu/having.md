# HAVING 條件篩選
當某些情況 WHERE 無法使用時，像是篩選總數(SUM)，可以使用 HAVING 將撈出的資料做篩選。

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


##### 1. 依據 `product_name` 分類計算庫存(product_stock)大於100的商品

```sql
SELECT product_name,SUM(product_stock) FROM Product GROUP BY product_name HAVING SUM(product_stock)>100
```

![](/assets/img15-1.png)