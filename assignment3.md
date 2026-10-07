# Assignment 3: Where and when theft is reported near AU

[Original and Pivot Table Spreadsheet](https://american0-my.sharepoint.com/:x:/g/personal/tg0408a_american_edu/IQAAO6d6db74T4Fo17k72JcbAenq-T1WQ_5aM6SdmikSXHU?e=R5i3P7)

## 1. Question and newsworthiness

**Question:** Within one mile of AU's campus, which areas have the most reported thefts, and during which shift do they happen?

AU students walk, bike, and park in this area every day, and theft is the kind of crime they are most likely to experience. If reports occur in a few places or at a certain time of day, students can change their habits, such as not leaving belongings in cars or avoiding certain areas after dark.

Newsworthiness for AU's audience:

- **Close to home:** it covers the streets students use daily.
- **Widely relevant:** theft affects many people.
- **Actionable:** readers can change their behavior based on the pattern.

## 2. Steps

1. Downloaded the AU crimes file from the class GitHub repository and opened it in Excel for the web.
2. Reviewed the columns and selected the ones needed: OFFENSE, SHIFT, BLOCK_GROUP, and CCN.
3. Inserted a PivotTable on a new sheet (**Insert > PivotTable**).
4. Built the pivot table with these fields:
    A) Filters - OFFENSE - theft/other and theft f/auto only 
    B) Rows - BLOCK_GROUP
    C) Columns - SHIFT
    D) Values - CCN - Count (changed from the default Sum)
5. Changed CCN from **Sum** to **Count**. Sum added up the case numbers and produced meaningless totals.
6. Sorted the Grand Total column from largest to smallest.
7. Checked that the rows add up to the grand total (1,886) and that the day, evening, and midnight columns add up too.

## 3. Answer

Theft reports are concentrated in a few places. The pivot table counted **1,886** theft reports across **30** block groups. 

Most thefts are reported on the day and evening shifts:

- **Day:** 857 reports
- **Evening:** 881 reports
- **Midnight:** 148 reports

In each of the top three block groups, evening has more reports than day. 

## Final Project
[Link for group project](https://github.com/mg3428a/datajournalism-fall2026/blob/main/assignment3.md)

## AI Disclosure 
I did not use AI to assist me with this assignment.
