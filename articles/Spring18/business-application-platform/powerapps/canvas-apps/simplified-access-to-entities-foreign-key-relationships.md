---

title: Simplified access to entities through foreign key relationships
description: Makers can now write formulas that work seamlessly between entities, following lookups for related information.
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
#  Simplified access to entities through foreign key relationships




[!include[banner](../../../../includes/banner.md)]

Makers can now write formulas that work seamlessly between entities, following
lookups for related information.

For example, a record in the Accounts entity might have a Primary Contact field
that is a lookup to a record in the Contacts entity. Previously, the maker had
to manually look up records across entities, which meant knowing about and
working with a foreign key. Now, a maker can simply write:

     First( Accounts ).PrimaryContact.FullName

The maker then has access to all the PrimaryContact fields, such as Fullname,
EmailAddress, or any other field.
