---

title: Lifecycle Services: Telemetry-based KB recommendation
description: LCS has been extended to include telemetry-driven KB recommendations to customers.
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
#  Lifecycle Services: Telemetry-based KB recommendation




[!include[banner](../../../includes/banner.md)]

LCS has been extended to include telemetry-driven KB recommendations to
customers. The goal of this functionality is to help us understand the extent to
which hotfixes have solved an issue and to proactively push out hotfixes to
customers. This will allow customers to spend less time looking for solutions to
issues that a hotfix already exists for. In addition, it will provide telemetry
that gives us better insight into which fixes have solved specific customer
issues. This enhancement also lets us ship additional telemetry to gain
additional insight where needed. The first example of telemetry-based KB
recommendations is the Critical X++ updates tile.

Critical X++ updates are hotfixes that we recommend based on the telemetry data
from your production environment. These updates are specific to your production
environment and can be downloaded only from your production environment.

To test and apply critical X++ updates, you should first download the updates
from the production environment, and then apply them in a development
environment, build a deployable package, and then deploy and test it in your
sandbox environment. After it's fully tested, you can then deploy it to your
production environment.

![A screenshot showing LCS Telemetry-based KB recommendations](media/lifecycle-services-telemetry-based-kb-recommendation-1.png "A screenshot showing LCS Telemetry-based KB recommendations")
<!-- FO_LCS_telemtry_KB_A.png -->


*LCS telemetry-based KB recommendations*
