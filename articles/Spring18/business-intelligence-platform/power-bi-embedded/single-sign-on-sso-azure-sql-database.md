---

title: Single sign-on (SSO) for Azure SQL database
description: Power BI Embedded has no awareness and information about the application’s user.
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
#  Single sign-on (SSO) for Azure SQL database




[!include[banner](../../../includes/banner.md)]

Power BI Embedded has no awareness and information about the application’s user.
For applications that do want to set row-level security in Azure SQL database,
there’s a need to pass the application’s user information back to Azure SQL.

When the SSO option is enabled and your users access reports built on top of the
data source, Power BI sends their authenticated Azure AD credentials in the
queries to the Azure SQL database. This enables Power BI Embedded to respect the
security settings that are configured at the data source level.
