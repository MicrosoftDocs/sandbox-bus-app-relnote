---

title: Mobile layout support
description: Reports and dashboard support layouts are optimized to consume on mobile devices.
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
#  Mobile layout support




[!include[banner](../../../includes/banner.md)]

Reports and dashboard support layouts are optimized to consume on mobile
devices.

For reports, you can open report pages in [phone
layout](https://docs.microsoft.com/en-us/power-bi/desktop-create-phone-report),
if they were created through Power BI Desktop. You can use a [new JavaScript
API](https://github.com/Microsoft/PowerBI-JavaScript/wiki/Embed-For-Mobile) to
check whether a report page has a phone layout defined, and if it does, embeds
it. It’s the optimal layout to use when devices are in the portrait orientation.
When devices are in landscape orientation, the optimal layout is the original
report layout. Using the JavaScript API, you can switch views during the user’s
session according to the phone layout, offering an optimal experience at any
state.

Dashboards can be rendered on mobile devices using the one column layout, which
sets all tiles in a single column, one above the other. As in the reports, this
view is optimal for portrait orientation. The application can also switch back
to original layout during the session.
