---

title: Batch balancing enabled for advanced warehousing processes
description: Batch balancing is a process where the amount of ingredients to use in a production batch is calculated from the concentration of active ingredients in product batches selected by the user.
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
#  Batch balancing enabled for advanced warehousing processes




[!include[banner](../../../includes/banner.md)]

Batch balancing is a process where the amount of ingredients to use in a
production batch is calculated from the concentration of active ingredients in
product batches selected by the user. The batch balancing process is now
available for products that are set up for warehouse management processes (in
earlier releases, the batch balancing process was enabled only for products that
were not set up for warehouse management processes). This enhancement makes it
possible for the user to release ingredients to picking after the batch
balancing process has been completed.

The batch balancing process is performed from the Batch balancing page. Select
Cost management \> Batch orders, and then, on the Process tab, select Batch
balancing. Batch balancing is available for batch orders that have a status of
Started.

In general, the following rule applies: Batch orders are applicable for batch
balancing if the formula has at least one formula line where the ingredient type
is Active.

The batch balancing process can be divided into two sub-processes:

**Balance batch ingredients**. In the Balance batch ingredients sub-process, the
amount of ingredients to use for the production batch is calculated based on the
selected batches that have active ingredients. As a rule, the calculation can be
completed only if there is full coverage of all ingredients. You can't balance
only part of the batch that the batch order is set up to produce.

**Confirm and release the formula**. After the ingredient quantities have been
calculated, you can confirm and release the formula. The release process
differs, depending on whether the products are enabled for the warehouse
management processes.

There is one exception to the rule that batch orders are applicable for batch
balancing if the formula has at least one formula line where the ingredient type
is Active. If a formula contains an active ingredient for a product that is
enabled for warehouse management processes, but Batch number is below Location
in the reservation hierarchy, the batch order isn't applicable for batch
balancing. A batch order that isn't applicable for batch balancing goes through
the regular process cycle for batch orders.
