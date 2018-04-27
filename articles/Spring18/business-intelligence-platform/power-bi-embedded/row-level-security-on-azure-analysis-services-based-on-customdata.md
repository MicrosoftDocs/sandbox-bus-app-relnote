---

title: Row-level security on Azure Analysis Services based on CustomData
description: Use row-level security and filter data based on the CustomData function in Azure Analysis Services.
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
#  Row-level security on Azure Analysis Services based on CustomData




[!include[banner](../../../includes/banner.md)]

Use row-level security and filter data based on the CustomData function in Azure
Analysis Services. You can customize and filter data retrieved from Analysis
Services for each user session, which controls the data exposed to each user.

For Azure Analysis Services users, a property is added on token generation, so
you can set the **CustomData** property on the connection string. This property
can also be used by the **CustomData** function. The property can be applied for
all embedded objects: reports, visuals, dashboards, and tiles. The feature works
only with Azure Analysis Services.
