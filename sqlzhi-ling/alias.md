# ALIAS 別名
最常用到的別名有兩種：欄位別名與表格別名。

欄位別名和表格別名的語法：
```sql
SELECT "表格別名"."欄位1" "欄位別名" FROM "表格名" "表格別名";
```

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


##### 1. 依據 `product_name` 分類計算該類庫存(product_stock)
跟 `GROUP BY` 範例一樣不過仔細看我們在語法上添加了欄位別名與表格別名，目的是為了讓 SQL 產生的結果易讀，且能夠自訂顯示的欄位名稱，下面範例 `A1` 就是所謂的別名(可自由命名)。

```sql
SELECT A1.product_name name,SUM(A1.product_stock) stock FROM product A1 GROUP BY A1.product_name 
```

