<!--
//Mark Down Comments
Documents are written in a markdown format and converted to pdf with a tool 'pandoc'

Pdf build command on Kumar machine

pandoc -s -F pantable -o backlog.pdf backlog.md

vim command 

:!pandoc -s -F pantable -o %:r.pdf %

// There is an extension pantable that reads the data between ```{.table} and ``` and generate a table based on comma seperated values
The data between --- and --- are yaml configuration data

-->
---
title:
- 'Project'
author:
- Kumar Sookram
- Kimberly
- Jayron
theme:
- Berkeley
geometry:
- margin=1cm
---


# Backlog

```{.table}
---
alignment: LLLLLCR
caption: '**Product Backlog**'
header: true
markdown: true
table-width: 1
width: [0.05, 0.1, 0.3, 0.3, 0.1, 0.05, 0.1]

---
ID, As a..., I want to be able to..., So that..., Priority, Sprint, Status  
C1, Customer, Login to App , I can do transactions, Must, 2, TBD
C2, Customer, Notified of incorrect credentials, I can re-enter correct credentials, Must, 2, TBD
C3, Customer, View products listing, I can choose what items to order, Must, 2, TBD
C4, Customer, Add items from the product listing to my cart, I can review items I am interested in buying, Must, 2, TBD
C5, Customer, Remove items from my cart, I don't buy something I don't want,  Must, 2, TBD
C6, Customer, Create a standing order, I can request items I want and it's frequency, Must, 3, TBD 
C7, Customer, View my standing orders, I can tell what my standing orders are, Must, 3, TBD
C8, Customer, Edit a standing order, I can adjust my standing orders, Must, 3, TBD
C9, Customer, Check my current balance, I can determine how much is due to the Bakery, Must, 3, TBD
C10, Customer, Print an invoice, I have a physical copy of an invoice, Must, 3, TBD
C11, Customer, View a listing of all Invoices, I can view my history, Must, 3, TBD
C12, Customer, Log out of my account, Only I can make purchases on my account, Must, 2, TBD
```
