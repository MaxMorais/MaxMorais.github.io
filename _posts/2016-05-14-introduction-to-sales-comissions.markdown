---
published: true
title: Introduction to Sales Comissions
layout: post
tags: [ERPNext, Sales, Comissions, Customization]
categories: [ERPNext, Sales, Comission, Customization]
---
For some companies perform and account **Sales Comissions** is a really hard task! Thinking about this I started developing a small solution to determine the comissions of each member in the **Sales Team**.

These comissions can be managed like as **Pricing Rules**, or **Tax Rules** due a combination of various fields and values:

![Sales Comission](//www.diigo.com/file/image/eoaccapzdbeqorcaczccsspoor/Montagem+-+SCMS-000001.jpg)

- _Reference_ is a human readable name of the **Sales Comission**
- _Comission Base_ indicates if a comission is based in a **Item** or **Item Group**
- _Comisson To_ indicates the record name of the _Comission Base_
- _Party Type_ indicates if a comission is based in a **Customer** or **Customer Group**
- _Party_ indicates the record name of the **Party Type**
- _Sales Person_ indicates the Person or the **Group** that the comission will be assigned
- _Comission On_ indicates the transaction where the comission will be computed, it should be **Quotation**, **Sales Order** or **Sales Invoice**
- _Comission Type_ indicates the type of the comission, it can be **Value** for a fixed comission, or **Percent** to a variant comission.
- _Fieldname_ indicates the base field to compute the **Percent** comission
- _Comission Rate (%)/Value_ indicates the rate or the comission value

These rules are evaluated at the validation method of the Transactions, and it compute the right values in the **Sales Team** table, under the transaction.

In the given example the comission should be computed based in the _PO Amount_ custom field in the body of the **Sales Order** 

![Comission Base](//www.diigo.com/file/image/eoaccapzdbeqorsbozccssppca/Cliente+Padr%C3%A3o+-+SO-00002.jpg) 

How you can see, the comission is right computed for the **Sales Person** in the below image

![Computed Comission](//www.diigo.com/file/image/eoaccapzdbeqosabpzccssppeb/Cliente+Padr%C3%A3o+-+SO-00002.jpg)

Don't matter if the Comission is based on the _Transaction Amount_, or if it is a _Fixed Value_, this customization ever will lookup to the right comission and store in the _Incentives_ field, the other fields are filled just to continue using the standard behavior of **ERPNext**.

The rule to determine the hierarchy of the comission is based from the **Group** (Customer Group or Item Group) to the *Party or Item* how more high the level of record that the comission is attached , less important is this! So, a comission attached to a **Item** overrides a comission to his parent group!