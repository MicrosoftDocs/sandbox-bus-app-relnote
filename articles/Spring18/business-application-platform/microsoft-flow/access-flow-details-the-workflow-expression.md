---

title: Access flow details with the workflow() expression
description: The last feature we added is a new output property called **tags** to the **workflow()** expression.
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
#  Access flow details with the workflow() expression




[!include[banner](../../../includes/banner.md)]

The last feature we added is a new output property called **tags** to
the **workflow()** expression. The tags contain properties
like **flowDisplayName** and **environmentName**. This means that - from the
flow itself, you can send custom email notifications that link back to the flow.
For example, this will create an HTML link back to the flow with the display
name of the flow in the title:

\<a
href="https://flow.microsoft.com/manage/environments/\@{workflow()['tags']['environmentName']}/flows/\@{workflow()['name']}/details"\>Open
flow \@{workflow()['tags']['flowDisplayName']}\</a\>
