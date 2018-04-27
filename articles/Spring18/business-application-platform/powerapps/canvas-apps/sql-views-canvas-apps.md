---

title: SQL views for canvas apps
description: Use SQL views to combine data in SQL Server before bringing it into PowerApps.
author: MargoC
manager: AnnBe
ms.date: 4/27/2018
ms.topic: article
ms.prod: 
ms.service: business-applications
ms.technology: 
ms.author: margoc
audience: Admin

---
#  SQL views for canvas apps




[!include[banner](../../../../includes/banner.md)]

Use SQL views to combine data in SQL Server before bringing it into PowerApps.

A common scenario is to have a single table (Product Category) with lookups to
another table (Products) that contains data points such as the product number,
name, and price.

Previously, you had to bring both tables into PowerApps, create a gallery of
categories, and then look up the detail information for the product information.
If this was done incorrectly, it could cause performance issues due to the
number of data calls to SQL Server.

Another possible scenario is to aggregate (group and sum) data before bringing
it into PowerApps. Rather than bringing all the records into PowerApps and using
the Sum feature, you can do all of the advanced processing in SQL Server first.
