For accurate accounting all incoming ingots in cargo are numbered.

Ingots in each consignment are numbered in the row from A1 to Z9 as
A1, A2,..., A9, B1, B2, ..., Z9. Each consignment are marked by the last ingots in it.
So you can define the quantity of ingots by marks.

You are given a report of daily consignments as marks written in string separated by commas.
Count the total quantity of ingots. 
For example, "A2,B1" -- here we can see two consignments with 2 (A2) and 10 (B1) ingots, so the result is 12.

**Input:** A daily report as a string. 

**Output:** The total quantity of ingots as an integer.

**Example:**

```python
count_ingots("A2,B1") == 12
count_ingots("A1,A1,A1") == 3
count_ingots("Z9,X8,Y7") == 672
count_ingots("C1,D1,B1,E1,F1") == 140
```

**How it is used:**

This concept is modified numeral system and basis for work with strings.

**Precondition:**
```python
re.match("[A-Z][1-9](,[A-Z][1-9])*", report)
```
