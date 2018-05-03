---

title: App-only token support
description: App-only token support
author: MargoC
manager: AnnBe
ms.date: 05/01/2018
ms.assetid: f403650f-1438-465f-8164-71f8625d60a3
ms.topic: article
ms.prod: 
ms.service: business-applications
ms.technology: 
ms.author: margoc
audience: Admin

---
#  App-only token support




[!include[banner](../../../includes/banner.md)]

Currently, building a Power BI Embedded application (also known as “app owns the
data scenario”) requires creating a so-called master user account, storing the
credentials for that account, and using them in the application code for
performing non-interactive sign-in to Power BI. On the other hand, Azure AD has
special support for applications authenticating using their own identity without
a user context. This support was specially designed for app-only authentication,
allows higher control and security, has less limitations, and is in general the
recommended approach. We’re adding support for application authentication to
Power BI Embedded. This enhances the deployment, security, and ALM for ISV apps
that are using Power BI Embedded.
