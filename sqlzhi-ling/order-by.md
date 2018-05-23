# ORDER BY 排序
使用此語法能夠將撈出來的資料做排序，ASC(ascending) 代表結果會以由小往大的順序列出，而 DESC(descending) 代表結果會以由大往小的順序列出。 如果兩者皆沒有被寫出的話，那我們就會用 ASC。

## 範例
我們已下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_price|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |99|
| 4 | Python |85|

##### 1.由小到大排序

```sql
SELECT * FROM Product ORDER BY product_price ASC
```

> ASC 可省略

![](/assets/img8-1.png)

##### 1.由大到小排序

```sql
SELECT * FROM Product ORDER BY product_price DESC
```

![](/assets/img8-2.png)