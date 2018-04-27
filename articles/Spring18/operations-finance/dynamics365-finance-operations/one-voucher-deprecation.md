---

title: One voucher deprecation
description: The existing functionality for financial journals (general journal, fixed asset journal, vendor payment journal, and so on) lets you enter multiple subledger transactions in the context of a single voucher.
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
#  One voucher deprecation




[!include[banner](../../../includes/banner.md)]

The existing functionality for financial journals (general journal, fixed asset
journal, vendor payment journal, and so on) lets you enter multiple subledger
transactions in the context of a single voucher. This functionality is referred
to as “One voucher.” The One voucher functionality causes issues during
settlement, tax calculation, reconciliation of a subledger to the general
ledger, financial reporting, and more. Because of these issues, the One voucher
functionality will be made obsolete. However, because there are functional gaps
that depend on this functionality, the functionality won't become obsolete all
at once. Instead, we will use the following schedule:

-   **Spring '18 release** – The functionality will be turned off by default,
    through a General ledger parameter. However, you can turn the functionality
    on if your organization has a scenario that falls in the business scenario
    gaps that are listed in the One voucher documentation.

-   If a customer has a business scenario that doesn't require One voucher,
    don't turn the functionality on. We won't fix “bugs” in the areas that are
    identified in the One voucher documentation if this functionality is used.

-   Stop using One voucher for integrations into Microsoft Dynamics 365 Finance
    and Operations, unless the functionality is required for one of the
    functional gaps.

-   **Fall '18 and later releases** – The functional gaps will be filled. After
    the functional gaps are filled, the One voucher functionality will be
    permanently turned off.

See the [One voucher
documentation](https://go.microsoft.com/fwlink/?linkid=869389) for detailed
information about the use and deprecation of this functionality.
