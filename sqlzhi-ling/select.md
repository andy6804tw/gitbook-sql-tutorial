# SELECT 查詢資料
使用 `SELECT` 語法可唷查詢資料庫某個欄位裡的值，是 SQL 中最長賞用到的指令。

```sql
SELECT "欄位名" FROM "表格名";
```

## 範例
我們已下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_price|
| -------- | ---------- | ----------- |
|    1     |    C語言    |100|
|    2     |    Java    |110|
|    3     |   Python   |80|

##### 1.查詢所有欄位資料

```sql
 SELECT * FROM Product
``` 

![](/assets/img1-1.png)

##### 2.查詢某個欄位資料

```sql
 SELECT product_name FROM Product
``` 

![](/assets/img1-2.png)

若想將輸出欄位名稱改名可以使用 `AS` 語法。

```sql
 SELECT product_name AS "Name" FROM Product
``` 

![](/assets/img1-3.png)



