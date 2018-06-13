# AS 指定別名
AS 關鍵字是用來指定欄位別名或是表格別名的。它是被放在欄位名和欄位別名之間，或是放在表格名和表格別名之間。AS 的語法如下：
```sql
SELECT "表格別名"."欄位1" AS "欄位別名" FROM "表格名" AS "表格別名";
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
跟 `ALIAS(別名)` 範例一樣，若要改寫欄位名稱可以加上 `AS` 關鍵字。

```sql
SELECT A1.product_name as name,SUM(A1.product_stock) as stock FROM Product as  A1 GROUP BY A1.product_name 
```

