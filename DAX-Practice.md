# DAX Practice Reference Guide

## **Aggregation Functions**
- **`SUM(Table[ColName])`**  
  - Provides the summation of all values in a column.
- **`SUMX(<Table>, <Expression>)`**  
  - Evaluates expressions row by row and returns the sum.
- **`AVERAGE(Table[ColName])`**  
  - Returns the arithmetic average of the column.
- **`AVERAGEX(<Table>, <Expression>)`**  
  - Iterates over the table, evaluates an expression row by row, and returns the average.
- **`MAX(Table[ColumnName])`**  
  - Returns the maximum value in a column.
- **`MIN(Table[ColumnName])`**  
  - Returns the minimum value in a column.

## **Counting Functions**
- **`COUNT(Table[ColName])`**  
  - Counts non-blank numeric entries in a column.
- **`COUNTA(Table[ColName])`**  
  - Counts all types of non-blank entries (numeric, text, string, etc.).
- **`COUNTX(<Table_Name>, <Expression>)`**  
  - Evaluates an expression row by row, similar to COUNTA but for calculated expressions.
- **`DISTINCTCOUNT(Table[ColName])`**  
  - Returns a unique count of values in a column (duplicates counted only once).
- **`COUNTBLANK(Table[ColName])`**  
  - Counts the number of blank (empty) values in a column.

## **Range Functions**
- **`RANGE(Table[ColName])`**  
  - Returns the difference between the maximum and minimum value in a column.
- **`RANGEX(<Table>, <Expression>)`**  
  - Evaluates an expression row by row and finds the range in calculated values.

## **Filtering & Conditional Functions**
- **`CALCULATE(<Expression>, <Filter1>, ...)`**  
  - Modifies the filter context before evaluating expressions.
- **`FILTER(<Table>, <Expression>)`**  
  - Returns a virtual table based on the applied filter expression. *(Not recommended for large datasets due to performance impact.)*
- **`IF(<Expression>, <True Value>, <False Value>)`**  
  - Defines conditions and labels data accordingly.
- **`SWITCH(<Expression>, <Value1>, <Result1>, <Value2>, <Result2>, ..., <Else>)`**  
  - Evaluates an expression against a list of values and returns corresponding results.

## **Table Relationships**
- **`RELATED(Table[Col Name])`**  
  - Returns a related value from another table.
- **`RELATEDTABLE(Table)`**  
  - Returns a table containing related values.
- **`ALL(Table[Col Name])`**  
  - Removes all filters from a column or table.
- **`ALLEXCEPT(<Table>, <Column1>, <Column2>, ...)`**  
  - Removes all filters except those on specified columns.

## **Mathematical & Ranking Functions**
- **`DIVIDE(<Numerator>, <Denominator>, <Alternative>)`**  
  - Performs division with an optional alternative result for division by zero.
- **`RANKX(<Table>, <Expression>, [Value], [Order], [Ties])`**  
  - Returns the rank of a value in a column.

This guide serves as a handy reference for practicing DAX functions efficiently! 🚀
