---

title: Phased embedding
description: Load the embedded content in the background to improve performance and get metadata on the object.
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
#  Phased embedding




[!include[banner](../../../includes/banner.md)]

Load the embedded content in the background to improve performance and get
metadata on the object. The loading of an embedded artifact is done using the
embed call, containing an embed configuration object and the **\<div\>** element
that contains the iFrame. After the embedded object is called, it’s loaded for
the user, and any interaction with the object is done while the object is
displayed.

With the Spring ’18 release, there are more JavaScript calls that add phases to
the embedding process:

-   **Preload.** The **powerbi.preload()** call uses the browser’s cache and
    download scripts before showing the embedded object itself. This can be
    useful for applications hosting several embedded reports. After the
    **preload** action completes, a **ready** event fires.

-   **Load metadata.** The **powerbi.load()** call helps retrieve information
    about the embedded object, and dynamically changes the settings or the
    **\<div\>** element in the background, before the object is displayed to the
    user. For example, you can use this function to get pages and then decide
    the page to show to the user. Or, you can get visuals and then decide which
    visuals you want to show or hide from the users. If you use this function,
    you need to call the **render** function to show the embedded object. After
    the load completes, a loaded event fires.

-   **Render object.** The final call, in case you implemented the
    **powerbi.load** function, is **render**. The **render** completes the last
    actions needed to render and show the embedded object to the user. After the
    **render** completes, a rendered event fires.

Although the **load** and **render** functions must be used together,
**preload** is independent of them. You can use the **embed** function to show
the embedded object after preload. You can also utilize the full-phased
procedure by calling **preload**, **load**, and **render** in order.

For more information, see [Phased Embedding
API](https://github.com/Microsoft/PowerBI-JavaScript/wiki/Phased-Embedding-API).
