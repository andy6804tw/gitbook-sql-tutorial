# AND OR 且或查詢
通常搭配 `WHERE` 來做判斷式。

## 範例
我們已下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_price|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |110|
| 4 | Python |80|

##### 1.查詢價格等於100或110的資料

```sql
SELECT * FROM Product WHERE product_price=100 OR product_price=110
```

![](/assets/img4-1.png)


##### 2.查詢價格大於等於 80 小於 100 的資料

```sql
SELECT * FROM Product WHERE product_price>=80 AND product_price<=100
```

![](/assets/img2-2.png)