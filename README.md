# GEDCOM Parser
## GEDCOM Parser for Stevens CS555
## Contributors: [SecondThrow](https://github.com/SecondThrow), [tmitche2](https://github.com/tmitche2), [lsachs98](https://github.com/lsachs98)

### Semester Project to Demonstrate Agile Methodologies
Uses Python 3.5, [Tabulate](https://pypi.org/project/tabulate/), [Family Echo GEDCOM Format](https://www.familyecho.com/).
Attempts to find errors within the GEDCOM file and print the results in a nice table.

## Completed User Stories

| Story Id | Story Name | Story Description |
| :-: | :-: | :-: |
| US01 | Dates Before Current Date | Dates (birth, marriage, divorce, death) should not be after the current date. |
| US02 | Birth Before Marriage | Birth should occur before marriage of an individual. |
| US03 | Birth Before Death | Birth should occur before death of an individual. |
| US04 | Marriage Before Divorce | Marriage should occur before divorce of spouses, and divorce can only occur after marriage. |
| US05 | Marriage Before Death | Marriage should occur before death of either spouse. |
| US06 | Divorce Before Death | Divorce can only occur before death of both spouses. |
| US07 | Less Than 150 Years Old | Death should be less than 150 years after birth for dead people, and current date should be less than 150 years after birth for all living people. |
| US09 | Birth Before Death of Parents | Child should be born before death of mother and before 9 months after death of father. |
| US10 | Marriage After 14 Years Old | Marriage should be at least 14 years after birth of both spouses (parents must be at least 14 years old). |
| US11 | No Bigamy | Marriage should not occur during marriage to another spouse. |
| US12 | Parents Not Too Old | Mother should be less than 60 years older than her children and father should be less than 80 years older than his children. |
| US13 | Siblings Spacing |	Birth dates of siblings should be more than 8 months apart or less than 2 days apart (twins may be born one day apart, e.g. 11:59 PM and 12:02 AM the following calendar day). |
| US15 | Fewer Than 15 Siblings |	There should be fewer than 15 siblings in a family. |
| US16 | Male Last Names |	All male members of a family should have the same last name. |
| US17 | No Marriages to Descendants |	Parents should not marry any of their descendants. |
| US18 | Siblings Should Not Marry |	Siblings should not marry one another. |
| US28 | Order Siblings by Age | List siblings in families by decreasing age, i.e. oldest siblings first. |
| US29 | List Deceased | List all deceased individuals in a GEDCOM file. |
| US30 | List Living Married |	List all living married people in a GEDCOM file. |
| US31 | List Living Single |	List all living people over 30 who have never been married in a GEDCOM file. |
| US35 | List Recent Births |	List all people in a GEDCOM file who were born in the last 30 days. |
| US36 | List Recent Deaths | List all people in a GEDCOM file who died in the last 30 days. |
| US38 | List Upcoming Birthdays | List all living people in a GEDCOM file whose birthdays occur in the next 30 days. |
| US42 | Reject illegitimate dates | All dates should be legitimate dates for the months specified (e.g., 2/30/2015 is not legitimate). |

## Available User Stories

| Story ID | Story Name | Story Description |
| :-: | :-: | :-: |
| US01 |	Dates before current date | Dates (birth, marriage, divorce, death) should not be after the current date. |
| US02 |	Birth before marriage |	Birth should occur before marriage of an individual. |
| US03 |	Birth before death | Birth should occur before death of an individual. |
| US04 |	Marriage before divorce |	Marriage should occur before divorce of spouses, and divorce can only occur after marriage. |
| US05 |	Marriage before death |	Marriage should occur before death of either spouse. |
| US06 |	Divorce before death |	Divorce can only occur before death of both spouses. |
| US07 |	Less then 150 years old |	Death should be less than 150 years after birth for dead people, and current date should be less than 150 years after birth for all living people. |
| US08 |	Birth before marriage of parents |	Children should be born after marriage of parents (and not more than 9 months after their divorce). |
| US09 |	Birth before death of parents |	Child should be born before death of mother and before 9 months after death of father. |
| US10 |	Marriage after 14 |	Marriage should be at least 14 years after birth of both spouses (parents must be at least 14 years old). |
| US11 |	No bigamy |	Marriage should not occur during marriage to another spouse. |
| US12 |	Parents not too old |	Mother should be less than 60 years older than her children and father should be less than 80 years older than his children. |
| US13 |	Siblings spacing |	Birth dates of siblings should be more than 8 months apart or less than 2 days apart (twins may be born one day apart, e.g. 11:59 PM and 12:02 AM the following calendar day). |
| US14 |	Multiple births <= 5 |	No more than five siblings should be born at the same time. |
| US15 |	Fewer than 15 siblings |	There should be fewer than 15 siblings in a family. |
| US16 |	Male last names |	All male members of a family should have the same last name. |
| US17 |	No marriages to descendants |	Parents should not marry any of their descendants. |
| US18 |	Siblings should not marry |	Siblings should not marry one another. |
| US19 |	First cousins should not marry |	First cousins should not marry one another. |
| US20 |	Aunts and uncles |	Aunts and uncles should not marry their nieces or nephews. |
| US21 |	Correct gender for role |	Husband in family should be male and wife in family should be female. *LDS based system (not our choice)* |
| US22 |	Unique IDs |	All individual IDs should be unique and all family IDs should be unique. |
| US23 |	Unique name and birth date |	No more than one individual with the same name and birth date should appear in a GEDCOM file. |
| US24 |	Unique families by spouses |	No more than one family with the same spouses by name and the same marriage date should appear in a GEDCOM file. |
| US25 |	Unique first names in families |	No more than one child with the same name and birth date should appear in a family. |
| US26 |	Corresponding entries |	All family roles (spouse, child) specified in an individual record should have corresponding entries in the corresponding family records. Likewise, all individual roles (spouse, child) specified in family records should have corresponding entries in the corresponding  individual's records.  I.e. the information in the individual and family records should be consistent. |
| US27 |	Include individual ages |	Include person's current age when listing individuals. |
| US28 |	Order siblings by age |	List siblings in families by decreasing age, i.e. oldest siblings first. |
| US29 |	List deceased |	List all deceased individuals in a GEDCOM file. |
| US30 |	List living married |	List all living married people in a GEDCOM file. |
| US31 |	List living single |	List all living people over 30 who have never been married in a GEDCOM file. |
| US32 |	List multiple births |	List all multiple births in a GEDCOM file. |
| US33 |	List orphans |	List all orphaned children (both parents dead and child < 18 years old) in a GEDCOM file. |
| US34 |	List large age difference |	List all couples who were married when the older spouse was more than twice as old as the younger spouse. |
| US35 |	List recent births |	List all people in a GEDCOM file who were born in the last 30 days. |
| US36 |	List recent deaths |	List all people in a GEDCOM file who died in the last 30 days. |
| US37 |	List recent survivors |	List all living spouses and descendants of people in a GEDCOM file who died in the last 30 days. |
| US38 |	List upcoming birthdays |	List all living people in a GEDCOM file whose birthdays occur in the next 30 days. |
| US39 |	List upcoming anniversaries |	List all living couples in a GEDCOM file whose marriage anniversaries occur in the next 30 days. |
| US40 |	Include input line numbers |	List line numbers from GEDCOM source file when reporting errors. |
| US41 |	Include partial dates |	Accept and use dates without days or without days and months. |
| US42 |	Reject illegitimate dates |	All dates should be legitimate dates for the months specified (e.g., 2/30/2015 is not legitimate). |
