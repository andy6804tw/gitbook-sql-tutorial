# LIKE
LIKE 是另一個在 WHERE 子句中會用到的指令，他的表達方式類似正則表示法，使用萬用字元來篩選出符合條件的資料。

## 範例
我們以下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|product_price|
| -------- | ---------- | ----------- |
| 1 | C語言 |100|
| 2 | Java |110|
| 3 | JavaScript |99|
| 4 | Python |85|

##### 1.查詢名稱開頭含有 Java 的資料

```sql
SELECT * FROM Product WHERE product_name LIKE 'Java%'
```

![](/assets/img7-1.png)

## 萬用字元(Wildcard) 
SQL 中有兩個萬用字元：
- % (百分比符號)：代表零個、一個、或數個字母。
- _ (底線)：代表剛好一個字母。

### 範例
1. 'A_Z': 
    - (正確) AAZ、ABZ、A1Z 
    - (錯誤) A12Z、ASDZ
2. 'ABC%': 
    - (正確) ABCA、ABCASD
    - (錯誤) AABCA