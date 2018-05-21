# WHERE 篩選資料


通常 `WHERE` 會搭配 `SELECT` 用於資料篩選用，有時會想撈取特定區間的資料所以這時就可以使用此語法做篩選。


## 範例
我們已下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_price|
| -------- | ---------- | ----------- |
|    1     |    C語言    |100|
|    2     |    Java    |110|
|    3     |   JavaScript |110|
|    4     |   Python   |80|


##### 1.查詢價格等於 110 的資料

```sql
SELECT * FROM Product WHERE product_price=110
```

![](/assets/img2-1.png)

##### 2.查詢價格大於等於 80 小於 100 的資料

```sql
SELECT * FROM Product WHERE product_price>=80 AND product_price<=100
```

![](/assets/img2-2.png)