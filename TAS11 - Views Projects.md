# TAS11 - Views Projects

### 1. Invoice_view
- Sentencia:
```
CREATE VIEW invoice_view AS 
SELECT
  i.id,
  i.code,
  i.create_at,
  i.total,
  c.fullname
FROM
  invoice i
JOIN
 client c ON i.client_id = c.id;
```

- Captura

<img src="./TAS11-capturas/Pasted image 20240623213513.png" alt="drawing0" width="500"/>

### 2. detail_view
---
- Sentencia:
```
CREATE VIEW detail_view AS 
SELECT
  d.id,
  d.quantify,
  p.description,
  d.price,
  d.subtotal
FROM
  detail d
JOIN
  product p ON d.product_id = p.id;
```

- Captura

<img src="./TAS11-capturas/Pasted image 20240623213814.png" alt="drawing0" width="500"/>