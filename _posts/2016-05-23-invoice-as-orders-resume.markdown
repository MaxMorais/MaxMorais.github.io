---
published: true
title: Invoice as Orders resume
layout: post
tags: [ERPNext, Customization, Invoicing]
categories: [ERPNext, Customization, Invoicing]
---
In the service market segment, is very common that the companies open various Orders during the month to a customer, and in the end of the month, generate a single Invoice.

Thinking about this, I made a small change for one of our customer, but that will increase a lot your productively!

How do you can see in the below image, the customer issue a various service orders in a week, to each customer

![Sales Orders to Bill](https://www.diigo.com/file/image/eoaccapzdbopseoqdzcdbaorqp/Sales+Orders+to+Bill.jpg)

The _Accounts Manager_, two times per month issue a invoice, to each customer, the major issue, in this case is.

The _Accounts Manager_, need get all Orders in a single Invoice, and in **ERPNext** it is very hard to get!

So, we introduced a small button called *Bill Issuer* in the **Sales Invoice**, this button opens the below Dialog.

![Bill Issuer](https://www.diigo.com/file/image/eoaccapzdbopsocobzcdbaosba/Bill+Issuer.jpg)

The _Accounts Manager_, select the customer, and wait the list of  **Orders Pending to Bill**, so, with this, the _Accounts Manager_, selects the *Orders* that him need in the Invoice, and click in the *Bill* button, and get the *Invoice* issued with the most important information to the customer.

This is a silly change, but for the customer, represents a lot of time earned, that him can invest in the management of they business, instead of get blocked by a bureaucratic UI.