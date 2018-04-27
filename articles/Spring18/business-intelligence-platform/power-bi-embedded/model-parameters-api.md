---

title: Model parameters API
description: Users can uses model parameters to define parameters and make them a part of their reports and data models, such as a query filter, a data source reference, and a measure definition, dependent on one or more parameter values.
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
#  Model parameters API




[!include[banner](../../../includes/banner.md)]

Users can uses model parameters to define parameters and make them a part of
their reports and data models, such as a query filter, a data source reference,
and a measure definition, dependent on one or more parameter values. Parameters
are defined on the PBIX file through Power BI Desktop. For more information, see
this [blog
post](https://powerbi.microsoft.com/en-us/blog/deep-dive-into-query-parameters-and-power-bi-templates/).

Developers can use our new API to dynamically change the values of the
parameters and automate the process of working with them. The API includes a
call to get all parameters defined on a specific dataset, and a call to set
parameter values to set new values for existing parameters.

With this new API, you can automate many processes for multiple customers. A few
examples are:

-   **Change connection string.** By configuring parameters on the connection
    string, you can use the API whenever you onboard a new customer. Just clone
    the report and change the parameter values to connect to the customer’s
    database. It can also help automate connection updates to data sources that
    are not supported through [Update
    DataSources](https://msdn.microsoft.com/en-us/library/mt814715.aspx) API.

-   **Change query parameters.** By defining parameters on the API, you can set
    the values and get different results and data to reflect only what this
    report’s users should see.

-   **Measure parameters.** Dynamically change different calculated measures to
    answer each customer’s needs on the same report. For example, you can set
    the currency through parameters for different customers or branches based in
    different countries.

The parameters are based on the dataset; therefore, they’re defined per report
or dashboard, but they’re not defined on the user’s session level. It means that
different users using the same report at the same time will always see the same
parameter’s value.
