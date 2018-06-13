# 表格連接
假設我們有兩個表格，其中有相同欄位的資料我們要將他們兩個合併。

## 範例
我們以下面這個 Product 與 Category 表格來做查詢。

Product表格：

|product_id|product_name|product_stock|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |99|
| 4 | Python |85|
| 5 | Java |12|
| 6 | C語言 |14|

Category表格：

|category_id|category_name|product_name|
| -------- | ---------- | ----------- |
| 1 |大一| C語言 |
| 2 |大二| Python |
| 3 |大三|Java |
| 4 |大四| JavaScript |



##### 1. 將兩資料表合併

```sql
SELECT  Category.`category_name`, Product.`product_name`, product.`product_stock` FROM Product, Category WHERE Product.`product_name` = Category.`product_name`
```

![](/assets/img18-1.png)