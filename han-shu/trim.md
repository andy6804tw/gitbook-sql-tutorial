# TRIM 空白處理
SQL 中的 TRIM 函數是用來移除掉一個字串中的字頭或字尾。最常見的用途是移除字首或字尾的空白。

- MySQL: TRIM( ), RTRIM( ), LTRIM( )

各種 trim 函數的語法如下：

- TRIM 
將字串前後空白移除。

- LTRIM 
將所有字串起頭的空白移除。

- RTRIM 
將所有字串結尾的空白移除。

## 範例
我們以下面這個 Product 表格來做查詢。

Product表格：

|product_id|product_name|
| -------- | ---------- |
| 1 | ` Sample `|

> ` Sample ` 前後有留空白

##### 1. TRIM

```sql
SELECT TRIM(product_name) FROM Product
```

結果:

```sql
'Sample'
```

##### 2. LTRIM

```sql
SELECT LTRIM(product_name) FROM Product
```

結果:

```sql
'Sample '
```

##### 3. RTRIM

```sql
SELECT RTRIM(product_name) FROM Product
```

結果:

```sql
' Sample'
```