# Assignment 1: Design a Logical Model

## Question 1
Create a logical model for a small bookstore. 📚

At the minimum it should have employee, order, sales, customer, and book entities (tables). Determine sensible column and table design based on what you know about these concepts. Keep it simple, but work out sensible relationships to keep tables reasonably sized. Include a date table. There are several tools online you can use, I'd recommend [_Draw.io_](https://www.drawio.com/) or [_LucidChart_](https://www.lucidchart.com/pages/).

See file in DSI folder labelled "Assign_chart_without_dates.png"

## Question 2
We want to create employee shifts, splitting up the day into morning and evening. Add this to the ERD.

See file in DSI folder labelled "Assign_chart_with_dates.png"

## Question 3
The store wants to keep customer addresses. Propose two architectures for the CUSTOMER_ADDRESS table, one that will retain changes, and another that will overwrite. Which is type 1, which is type 2?

_Hint, search type 1 vs type 2 slowly changing dimensions._

Bonus: Are there privacy implications to this, why or why not?
```
Architecture Type 1 - Replaces Data

Table: CustomerAddress

CustomerID (Foreign Key)
StreetAddress
City
State
PostalCode


Architecture Type 2 - Replaces data
Table: CustomerAddress

CustomerAddressID (Primary Key)
CustomerID (Foreign Key)
StreetAddress
City
State
PostalCode
StartDate (When this address became valid)
EndDate (When this address was superseded)
IsCurrent (Boolean to indicate current address)

A new row/data is added each time there is a change of address, with StartDate and EndDate fields to track the period during which each address was valid. This will keep record of all changes. Although this will come with come privacy implications as greater volume of data storage presents with greater exposure threat to unauthourized users. More data requires more protections.

...
```

## Question 4
Review the AdventureWorks Schema [here](https://i.stack.imgur.com/LMu4W.gif)

Highlight at least two differences between it and your ERD. Would you change anything in yours?
```
1)My ERD is simplistic, as if the managment was under one peron. However AdventureWorks Schema is built for multiple departments (multiple users) HR, Purchasing etc. It is more complex. 

2)In my ERD the a single table is used for multiple applications. Address and contact info is in the same table for the bookstore ERD, but broken down into small tables for AdventureWorks possibly to avoid unnecessary exposure of private data for unauthorized users. 
```

# Criteria

[Assignment Rubric](./assignment_rubric.md)

# Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `June 1, 2024`
* The branch name for your repo should be: `model-design`
* What to submit for this assignment:
    * This markdown (design_a_logical_model.md) should be populated.
    * Two Entity-Relationship Diagrams (preferably in a pdf, jpeg, png format).
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/sql/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `model-design`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack at `#cohort-3-help`. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
