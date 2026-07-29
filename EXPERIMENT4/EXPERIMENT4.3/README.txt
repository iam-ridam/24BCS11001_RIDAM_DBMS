SELECT C.CUSTOMER_NAME,O.* FROM ORDERS AS O
LEFT JOIN customers AS C 
ON C.CUSTOMER_ID = O.CUSTOMER_ID;

SELECT P.PRODUCT_NAME, C.category_name FROM products AS P
FULL OUTER JOIN CATEGORIES AS C
ON P.CATEGORY_ID = C.CATEGORY_ID;

SELECT C.category_name, P.product_name, P.price FROM products AS P
RIGHT JOIN categories AS C 
ON P.category_id = C.category_id;