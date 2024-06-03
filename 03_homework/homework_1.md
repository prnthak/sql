# pasting the link to the image, hope it works 
# https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1#R3VrbcqM4EP0aP84WF18fEyczu1WztVOV2tnNvrgUUEATkIhoYjNfvw0IY8DY4BibzJPRQS2J1uk%2BLfDIXPqbL5IE7p%2FCpt7I0OzNyLwbGYauLyb4kyBxhkzNWQY4ktmqUwE8sJ9UgZpCI2bTsNQRhPCABWXQEpxTC0oYkVKsy92ehVeeNSAOrQEPFvHq6D%2FMBjdD5xOtwH%2BnzHHzmXVN3fFJ3lkBoUtssd6BzPuRuZRCQHblb5bUS5yX%2ByWz%2B9xwd7swSTm0MQjW3%2BO%2F%2Fvv7Ubdd3%2F1KH78w4n9So7wRL1IP%2FJ1yW0i1ZIhzP4Rr5nuEY%2Bt27TKgDwGxkltr3HbEXPA9bOl4qUakEuimcan61gHIHCp8CjLGLspgZiqfKdKYY8WidbEFRu5od9f9uSFR2%2B5sxy48gxfKOR0cZdQcNTKmHk57G6Ht1IH0yTPEYznyljpzhSOrWzh3cbexPyc%2B7WYBcdDRQqw5latnJkPA5zphymwAj4Rw3BjBXTdVuIVEgTKH9lFMIKWevTSCXGbblCMmRcRtmuyb1pZ5zWFQp2OcU60l%2B7S%2B2Gc2hql2iwnExd%2BbMGQO95PnHFTsTrSW3lv05bzxRUL3KdmHFY%2F8JypbmvhEvlBY2QQ%2BdvSYZ4meeV%2F7P2kOnj84bjMINcnVYmYbI7neTdrqndGX06YnBU1bRhfIa0Q4MIi7aU%2FrqAyksCML2hsIyRzGibcKJLM%2BdlhOBi5qsxrFvmW7heASGeS8Ly5DIBLUgcIwzyRu43KgGuNrJ7f5SXGaI2FAeMm%2F09dIpGpGrBcnJeInS3iYK82bZCWcASNeNoDqWY00S%2B1cOeSyicqTP8k9EXUoNi%2Bx6kopu2%2FdHzIZzM6SDKZ90VivH0S3yWBIymy0rWb7U2b9tKNoZyXMDTqcDHOTMMm63Uz2p402lq8QHz%2F%2BDj089aGfQHWz5jVqO%2FRBNYUEVzgCC6f7Aq14p%2BjzVYhAOfoHBYiVSpMIRHkb0Gky%2Fne38ZgM9psxydt3GzV61orz1obB1g6vd82wWVgljdzIxeLvp%2BBAiuntm%2BQdIja5SDMOIp9Z4rmd%2FU78cDi9oNtEJC16wL8qqLFmceghooz380RSjwB7K69jHwlSU3woEu90CATjEO6M%2FC0Biiy4mFXOJ4vKq8Yj%2FSdjrULAbAUFHbeP8g6G1s%2F56t3IoErIqqK0fj%2FSo6LUT8hXKiIbXqIMtXrMlpueFFcefUs%2BfXSvHC%2BwQpuGlmQBMMEHusKKgP8yZbfekK%2BHo%2BvTq%2Bi6kudcgjN5PqzOJ9cC15T1cUtZ1xte1vSr6zO9okXTw7pe66%2B%2By%2FWr6%2FOrVp7acNh2lEXGOUhU3%2FVKxTKufmTNokBZFXTozMaGedqysWv%2FShXbE3sXQ2LvMfKGIMULXWbKfWfTZxKlMntBDs8vwuHa18YGDp%2BLBts%2FgQxAZmctdbZr5rugrE7byup7M2JDbYXN4o87GUeKvz%2BZ9%2F8D


# Homework 1: farmersmarket.db

- Due on Thursday, May 16 at 11:59pm
- Weight: 8% of total grade

## Get to know the farmersmarket.db
Steps to complete this part of the homework:

#### 1) Load Database
- Open DB Browser for SQLite
- Go to File > Open Database
- Navigate to your farmersmarket.db 
	- This will be wherever you cloned the GH Repo (within the **SQL** folder)
	- ![db_browser_for_sqlite_choose_db.png](./images/01_db_browser_for_sqlite_choose_db.png)

#### 2) Configure your windows
By default, DB Browser for SQLite has three windows, with four tabs in the main window and three tabs in the bottom right window
- Window 1: Main Window (Centre)
	- Stay in the Database Structure tab for now
- Window 2: Edit Database Cell (Top Right)
- Window 3: Remote (Bottom Right)
	- Switch this to DB Schema tab (very bottom)

Your screen should look like this (or very similar)
![db_browser_for_sqlite.png](./images/01_db_browser_for_sqlite.png)

#### 3) The farmersmarket.db
There are 10 tables in the Main Window:
1) booth
2) customer
3) customer_purchases
4) market_date_info
5) product
6) product_category
7) vendor
8) vendor_booth_assignments
9) vendor_inventory
10) zip_data

Switch to the Browse Data tab, booth is selected by default
 ![01_the_browse_data_tab.png](./images/01_the_browse_data_tab.png) 


Using the table drop down at the top left, explore some of the contents of the database
![01_the_table_drop_down_at_the_top_left.png](./images/01_the_table_drop_down_at_the_top_left.png)

Move on to the Logical Data Model task when you have looked through the tables


## Logical Data Model

Recall during the module:

I diagramed the following four tables:
- product
- product_category
- vendor
- vendor_inventory

![01_farmers_market_logical_model_partial.png](./images/01_farmers_market_logical_model_partial.png)


Your task: choose two tables and create a logical data model. There are lots of tools you can do this (including drawing this by hand), but I'd recommend [Draw.io](https://www.drawio.com/) or [LucidChart](https://www.lucidchart.com/pages/). 

A logical data model must contain:
- table name
- column names
- relationship type

Please do not pick the exact same tables that I have already diagramed. For example, you shouldn't diagram the relationship between `product` and `product_category`, but you could diagram `product` and `customer_purchases`.

**A few hints**:
- You will need to use the Browse Data tab in the main window to figure out the relationship types.
- You can't diagram tables that don't share a common column
	- These are the tables that are connected
	-  ![01_farmers_market_conceptual_model.png](./images/01_farmers_market_conceptual_model.png)
- The column names can be found in a few spots (DB Schema window in the bottom right, the Database Structure tab in the main window by expanding each table entry, at the top of the Browse Data tab in the main window)

