---

title: Add an action to a business process flow
description: You can add an action that triggers a workflow to run processes on your data.
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
#  Add an action to a business process flow




[!include[banner](../../../includes/banner.md)]

You can add an action that triggers a workflow to run processes on your data.

For example, as part of the opportunity qualification process, the Contoso
organization requires all opportunities to be reviewed by a designated reviewer.
They need an action they can run on demand that:

-   Creates a task record that is assigned to the opportunity reviewer.

-   Appends “Ready for review” to the opportunity topic.

To integrate these tasks into the opportunity qualification process, the actions
must appear on the opportunity business process flow.

To enable this functionality, under Available to Run, select As a Business
Process Flow action step.

![A screenshot showing "available to run as a business process flow" configuration](media/add-action-to-business-process-flow-1.png "A screenshot showing "available to run as a business process flow" configuration")
<!-- Picture 17 -->


*Available to run as a business process flow*

Next, add the action step to Contoso’s Opportunity business process flow, and
validate the process.

![A screenshot of an action added to the Opportunity business process flow](media/add-action-to-business-process-flow-2.png "A screenshot of an action added to the Opportunity business process flow")
<!-- Picture 18 -->


*Action added to the Opportunity business process flow*

Now, members of Contoso’s salesforce can start the action from the Opportunity
Qualify business process step whenever they want by selecting Execute.

![A screenshot demonstrating how to execute an action](media/add-action-to-business-process-flow-3.png "A screenshot demonstrating how to execute an action")
<!-- Picture 19 -->


*Execute action*

To be able to execute an action or workflow on demand:

-   The business process flow must include an action step. If the action step
    runs a workflow, the workflow must be configured to run on demand.

-   The entity associated with the action or workflow must be the same as the
    entity associated with the business process flow.
