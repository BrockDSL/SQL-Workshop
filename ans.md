# SQL Workshop Answers

## Q1

```SQL

SELECT * FROM Products WHERE UnitPrice > 10;


```

## Q2

```SQL

SELECT CompanyName, Country FROM Suppliers ORDER BY Country;


```

## Q3

```SQL

SELECT ProductName,UnitPrice FROM Products WHERE UnitsInStock > 20;


```

## Q4

```SQL

SELECT ProductName, MAX(UnitsInStock) from Products;


```

## Q5

```SQL

SELECT ProductName, MAX(UnitsOnOrder) From Products;


```

## Q6

```SQL

SELECT SUM(UnitsInStock) FROM Products WHERE CategoryID = 2;


```

## Q7

```SQL


SELECT * FROM Products WHERE SupplierID

IN(SELECT SupplierID FROM Suppliers WHERE CompanyName = "Exotic Liquids");


```

## Q8

```SQL

SELECT CategoryID FROM Products WHERE ProductID

IN(SELECT SupplierID FROM Suppliers WHERE CompanyName = "Leka Trading");

```

## Q9

```SQL

SELECT ProductName FROM Products WHERE SupplierID

IN (SELECT SupplierID FROM Suppliers WHERE CompanyName = "Bigfoot Breweries")


```

## Q10

```SQL

SELECT 
    EmployeeID, 
    COUNT(EmployeeID) 
FROM 
    Orders 
GROUP BY 
    EmployeeID;
    

```