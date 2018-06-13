# DISTINCT 查詢不同的值

我們需要知道這個表格內有哪些不同的值可以使用 `DISTINCT` 語法查詢

## 範例
我們以下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_price|
| -------- | ---------- | ----------- |
|    1     |    C語言    |100|
|    2     |    Java    |110|
|    3     |   JavaScript |110|
|    4     |   Python   |80|


##### 1.查詢有哪幾種不同價格

```sql
SELECT DISTINCT product_price FROM Product 
```

![](/assets/img3-1.png)

##### 1.查詢有哪幾種不同價格的數量

```sql
SELECT COUNT(DISTINCT product_price) FROM Product 
```

![](/assets/img3-2.png)
