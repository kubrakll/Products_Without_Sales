# Products Without Sales Hacker Rank
SQL : 
SELECT DISTINCT p.sku, p.product_name
FROM Product p
LEFT JOIN INVOICE_ITEM o on p.id=o.product_id
WHERE p.id not in(
  SELECT product_id from INVOICE_ITEM
)
ORDER BY p.sku ASC

![image](https://github.com/kubrakll/Products_Without_Sales/assets/69002604/608e7047-3ea7-4df8-9e61-ce788eb073d4)
