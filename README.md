# Lab-7_202001101
# Lab-7_202001101
Section A:

1)Consider a program for determining the previous date. Its input is triple of day, month and year with the
following ranges 1 <= month <= 12, 1 <= day <= 31, 1900 <= year <= 2015.The possible output dates would be
previous date or invalid date. Design the equivalence class test cases?


SOLUTION:

To design the equivalence class test cases for the program, we need to consider the input ranges and identify the valid and invalid equivalence classes. Here are the equivalence classes for the input parameters:

Valid equivalence classes:

Valid day, month, and year
Valid day, month, and minimum year (1900)
Valid day, month, and maximum year (2015)
Invalid equivalence classes:

Invalid day, month, and year (e.g., day 0, day 32, month 0, month 13, year < 1900 or year > 2015)
Invalid day for a given month and year (e.g., Feb 29 in a non-leap year, Apr 31, Jun 31, Sep 31, Nov 31)
Based on these equivalence classes, here are the test cases that should be considered:

Valid equivalence class test cases:

Test case 1: Valid day, month, and year (e.g., 15, 7, 2005)
Test case 2: Valid day, month, and minimum year (e.g., 1, 1, 1900)
Test case 3: Valid day, month, and maximum year (e.g., 31, 12, 2015)

Invalid equivalence class test cases:

Test case 4: Invalid day, month, and year (e.g., 0, 0, 1899)
Test case 5: Invalid day, month, and year (e.g., 32, 13, 2016)
Test case 6: Invalid day for a given month and year (e.g., Feb 29 in a non-leap year, such as 29, 2, 2001)
Test case 7: Invalid day for a given month and year (e.g., Apr 31, such as 31, 4, 2005)
Test case 8: Invalid day for a given month and year (e.g., Jun 31, such as 31, 6, 2005)
Test case 9: Invalid day for a given month and year (e.g., Sep 31, such as 31, 9, 2005)
Test case 10: Invalid day for a given month and year (e.g., Nov 31, such as 31, 11, 2005)
The above test cases cover all the equivalence classes for the input parameters and should be sufficient to test the program for determining the previous date.

Q)Write a set of test cases (i.e., test suite) – specific set of data – to properly test the programs. Your test suite
should include both correct and incorrect inputs.
1. Enlist which set of test cases have been identified using Equivalence Partitioning and Boundary Value
Analysis separately.
2. Modify your programs such that it runs on eclipse IDE, and then execute your test suites on 
the
program. While executing your input data in a program, check whether the identified expected
outcome (mentioned by you) is correct or not.

P1]



Equivalence Partitioning:

If a is empty, an error message should be returned.
If v is not in a, -1 should be returned.
If v is the first element of a, the function should return 0.
If v is in the middle of a, the function should return the first index i such that a[i] == v, where i is greater than 0 and less than a.length - 1.
If v is the last element of a, the function should return a.length - 1.

Boundary Value Analysis:
If a has one element and it's not v, -1 should be returned.
If a has one element and it's v, the function should return 0.
If a has two elements and v is the first element, the function should return 0.
If a has two elements and v is the second element, the function should return 1.
If a has n elements and v is the first element, the function should return 0.
If a has n elements and v is the last element, the function should return n-1.
If a has n elements and v is not in a, -1 should be returned.


