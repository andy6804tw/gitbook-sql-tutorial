# SUBSTRING 子字串
SQL 中的 SUBSTRING 函數是用來抓出一個欄位資料中的其中一部分。

- MySQL: SUBSTR( ), SUBSTRING( )

```sql
SUBSTR (str, pos, len)
```
以上語法的意思是，由 <str> 中的第 <pos> 位置開始(從1開始)，選出接下去的 <len> 個字元。

## 範例
我們以下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_stock|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |99|
| 4 | Python |85|
| 5 | Java |12|
| 6 | C語言 |14|

##### 1. 取得 `product_name` 並從第二個字母開始 

```sql
SELECT SUBSTR(product_name,2) FROM Product
```

![](/assets/img20-1.png)