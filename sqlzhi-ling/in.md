# IN 多筆內容同時撈出
使用 `IN` 的時機在於當一個欄位有多筆資料的值提供時可以把要被撈出來的值放在括號內。

## 範例
我們已下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_price|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |110|
| 4 | Python |80|

##### 1.查詢價格等於100或80的資料

```sql
SELECT * FROM Product WHERE product_price IN(100,80)
```

![](/assets/img5-1.png)