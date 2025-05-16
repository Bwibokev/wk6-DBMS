Week 6 Assignment Guide

/* Question 1 */

SELECT 
    firstName, lastName, email, officeCode
FROM
    employees
        INNER JOIN
    offices USING (officeCode);

/* Question 2 */

SELECT 
    productName, productVendor, productLine
FROM
    products
        LEFT JOIN
    productlines USING (productLine);

/* Question 3 */

SELECT 
    orderDate, shippedDate, status, customerNumber
FROM
    customers
        RIGHT JOIN
    orders USING (customerNumber)
LIMIT 10;
