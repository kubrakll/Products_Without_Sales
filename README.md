# Products Without Sales Hacker Rank
SQL : <p>
SELECT DISTINCT p.sku, p.product_name <p>
FROM Product p <p>
LEFT JOIN INVOICE_ITEM o on p.id=o.product_id <p>
WHERE p.id not in( <p>
  SELECT product_id from INVOICE_ITEM <p>
) ORDER BY p.sku ASC <p>

![image](https://github.com/kubrakll/Products_Without_Sales/assets/69002604/608e7047-3ea7-4df8-9e61-ce788eb073d4)
