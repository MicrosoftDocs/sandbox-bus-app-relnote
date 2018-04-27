---

title: Access modern approvals in the Common Data Service for Apps
description: Modern approvals data in Flow is now built on the latest version of the Common Data Service for Apps.
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
#  Access modern approvals in the Common Data Service for Apps




[!include[banner](../../../includes/banner.md)]

Modern approvals data in Flow is now built on the latest version of the Common
Data Service for Apps. This means that you can build flows that read the status
of approvals you send or receive with the CDS connector. Examples include:

-   Send automatic reminders for pending approval requests.

-   Create to-do tasks in Microsoft To-Do, Trello, or Todoist when an approval
    is waiting to you.

-   Post a message to Teams when a new approval request matching specific
    parameters waiting for you.

You can [use this
template](https://flow.microsoft.com/galleries/public/templates/33d7ad77f610418d8cf3d61fe39fd507/get-an-email-report-of-approvals-waiting-for-my-response/)
as an example to start with. Customize this template and add or remove actions
as needed, such as creating a To-Do or posting to Microsoft Teams.



![](media/access-modern-approvals-the-common-data-service-apps-1.png "")
<!-- Picture 2 -->


*Approvals in CDS Template*

Today, all new environments created by an administrator use the latest version
Common Data Service for Apps. A few important notes for using this new
functionality:

1.  To have Approvals installed in an environment, the administrator must first
    create an Approval flow before any other users in the environment can use
    approvals.

2.  It can potentially take up to 10 minutes (or in some rare cases, longer)
    after creation for Approvals to begin functioning in the environment.

3.  For these templates to function, the person using these templates must be
    assigned the **Common Data Service User** security role in the CDS
    environment. If they are not assigned this role, they will be unable to
    access the Approval records through the CDS connector. However, Approvals
    will continue to function as they do today through the Approval center,
    irrespective of what roles are assigned to the user.

Existing environments that use Approvals will be updated in the coming weeks
with these new capabilities.
