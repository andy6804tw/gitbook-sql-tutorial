# Between 取得連續的值
BETWEEN 是讓我們可以使用一個範圍 (range) 內抓出資料庫中的值。

## 範例
我們以下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_price|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |99|
| 4 | Python |85|

##### 1.查詢價格在於100和80之間的資料

```sql
SELECT * FROM Product WHERE product_price BETWEEN 80 AND 100
```

![](/assets/img6-1.png)