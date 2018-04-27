---

title: Field Service Integration template
description: The Data Integrator supports scenarios where Dynamics 365 for Field Service activities are done outside Dynamics 365 for Finance and Operations.
author: MargoC
manager: AnnBe
ms.date: 4/26/2018
ms.topic: article
ms.prod: 
ms.service: business-applications
ms.technology: 
ms.author: margoc
audience: Admin

---
#  Field Service Integration template 


[!include[banner](../../../includes/banner.md)]

The Data Integrator supports scenarios where Dynamics 365 for Field Service
activities are done outside Dynamics 365 for Finance and Operations.
Capabilities include:

-   Enabling invoicing of Field Service work orders and agreements in Finance
    and Operations.

-   Integration of a warehouse with on-hand inventory, item reservations, usage,
    adjustments, and transfers.

-   Support for purchase order integration with synchronization of vendors,
    purchase orders, and receipts.

The first phase of feature work focuses on enabling invoicing of Field Service
work orders and agreements in Finance and Operations. The supported flow starts
in Field Service, where information from work orders is synchronized to Finance
and Operations as sales orders. In Finance and Operations, the sales orders are
invoiced to generate invoice documents. In addition, the information from Field
Service agreement invoices is synchronized to Finance and Operations.

![Diagram graphic of how data integrators work between Field Service and Finance and Operations](media/field-service-integration-template-1.png "Diagram graphic of how data integrators work between Field Service and Finance and Operations")
<!-- picture -->


*Integrating Field Service with Finance and Operations*
