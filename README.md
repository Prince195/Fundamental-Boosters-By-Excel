# Fundamental-Boosters-By-Excel

### 1. Introduction

This project focuses on strengthening the fundamental concepts of **Microsoft Excel formulas and data analysis techniques**. The objective is to practice important Excel functions such as **IF, COUNTIFS, SUMIFS, VLOOKUP, XLOOKUP, INDEX-MATCH, TEXT functions, and dynamic referencing tools like INDIRECT and OFFSET**. These functions help in organizing, analyzing, and retrieving data efficiently in real-world scenarios such as student records, employee data, and sales management.

Excel is widely used in industries for **data processing, financial calculations, reporting, and decision making**. By completing this project, students gain practical knowledge of how formulas and functions work together to automate calculations and data analysis.

---

# 2. Objectives

The main objectives of this project are:

* To understand **relative and absolute cell references**.
* To apply **logical formulas such as IF and Nested IF**.
* To perform conditional calculations using **COUNTIFS, SUMIFS, and AVERAGEIFS**.
* To retrieve information using **lookup functions like VLOOKUP, XLOOKUP, and INDEX-MATCH**.
* To manipulate text using **TEXT functions**.
* To work with **date and time calculations**.
* To create **dynamic references using INDIRECT and OFFSET**.
* To filter and extract data using the **FILTER function**.

---

# 3. Relative and Absolute References

Excel formulas use cell references to perform calculations.

**Relative Reference:**
A relative reference changes when the formula is copied to another cell.
Example:
`=A1+B1`

**Absolute Reference:**
An absolute reference remains constant when the formula is copied.
Example:
`=$A$1+$B$1`

Absolute references are useful when a fixed value such as **tax rate or constant value** is used in multiple calculations.

---

# 4. IF Function and Nested IF

The **IF function** is used to perform logical tests and return values based on conditions.

Example:
`=IF(A2>=60,"Pass","Fail")`

This formula checks whether a student's score is **60 or above**.

**Nested IF** allows multiple conditions in one formula.

Example:

```
=IF(A2>=90,"A",IF(A2>=75,"B",IF(A2>=60,"C","Fail")))
```

This helps in **grading students based on marks**.

---

# 5. IF with AND / OR Functions

These functions allow multiple logical conditions.

**IF with AND:**
Checks if all conditions are true.

Example:

```
=IF(AND(B2>=80,C2>=80),"Excellent","Average")
```

**IF with OR:**
Returns TRUE if at least one condition is true.

Example:

```
=IF(OR(D2>5000,E2="Yes"),"Discount","No Discount")
```

These formulas help in **decision making based on multiple criteria**.

---

# 6. COUNTIFS, SUMIFS, and AVERAGEIFS

### COUNTIFS

Counts cells based on multiple conditions.

Example:

```
=COUNTIFS(B2:B20,">60")
```

Counts students scoring above 60.

### SUMIFS

Adds values based on conditions.

Example:

```
=SUMIFS(C2:C20,A2:A20,"North")
```

### AVERAGEIFS

Calculates the average based on conditions.

Example:

```
=AVERAGEIFS(B2:B20,B2:B20,">60")
```

These functions are useful for **data analysis and reporting**.

---

# 7. VLOOKUP Function

VLOOKUP is used to search for data in a table vertically.

Example:

```
=VLOOKUP(A2,Sheet2!A2:C20,2,FALSE)
```

This formula searches for a **student ID** and returns the corresponding **name or value**.

It is commonly used for **product price lookup, employee information, and database retrieval**.

---

# 8. XLOOKUP Function

XLOOKUP is a modern and more flexible lookup function.

Example:

```
=XLOOKUP(A2,A2:A20,B2:B20)
```

Advantages of XLOOKUP:

* Works in **any direction**
* No column number required
* Handles **missing values easily**

---

# 9. INDEX and MATCH

INDEX and MATCH together provide a powerful lookup alternative.

Example:

```
=INDEX(B2:B20,MATCH(A2,A2:A20,0))
```

This combination allows **flexible and dynamic searches without column restrictions**.

---

# 10. TEXT Functions

Text functions help in manipulating and formatting text data.

Examples:

**LEFT**

```
=LEFT(A2,5)
```

**UPPER**

```
=UPPER(A2)
```

**LOWER**

```
=LOWER(A2)
```

These functions help in **cleaning and formatting textual data**.

---

# 11. INDIRECT and OFFSET

These functions create **dynamic references**.

**INDIRECT Example**

```
=INDIRECT("A"&B1)
```

**OFFSET Example**

```
=OFFSET(A1,2,1)
```

They are useful when working with **dynamic ranges or flexible references**.

---

# 12. Date and Time Functions

Excel can calculate time-based values.

Example:

Calculate Age:

```
=DATEDIF(A2,TODAY(),"Y")
```

Find difference between dates:

```
=B2-A2
```

These functions help in **employee records and time analysis**.

---

# 13. Math Functions

Excel includes several mathematical functions.

Examples:

ROUND

```
=ROUND(A2,2)
```

CEILING

```
=CEILING(A2,5)
```

FLOOR

```
=FLOOR(A2,5)
```

These functions help in **financial calculations and rounding values**.

---

# 14. FILTER Function

The FILTER function extracts data that meets specific conditions.

Example:

```
=FILTER(A2:C20,B2:B20>80)
```

This formula returns a list of **students scoring above 80**.

---

# 15. Conclusion

This project demonstrates the practical use of Excel formulas and functions for data analysis. By applying logical functions, lookup tools, and dynamic references, large datasets can be processed efficiently. These skills are essential in fields such as **business analysis, accounting, data management, and reporting**.
