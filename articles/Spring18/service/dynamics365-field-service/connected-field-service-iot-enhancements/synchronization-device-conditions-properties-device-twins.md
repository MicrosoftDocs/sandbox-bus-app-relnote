---

title: Synchronization of device conditions and properties with device twins
description: Connected Field Service includes a representation of customer assets and devices that can be registered within Azure IoT Hub to enable messages to flow through Azure IoT Hub to create alerts.
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
#  Synchronization of device conditions and properties with device twins 




[!include[banner](../../../../includes/banner.md)]

Connected Field Service includes a representation of customer assets and devices
that can be registered within Azure IoT Hub to enable messages to flow through
Azure IoT Hub to create alerts.

In the Spring ‘18 release, in addition to receiving messages that require
action, Connected Field Service uses the Azure IoT device twin capability. The
device twin, which is kept in sync with physical devices, is a JSON document
that holds metadata and configuration data, as well as a virtual cloud
representation of physical devices.

Connected Field Service communicates with device twins to allow devices to
report operating conditions such as device state, heartbeat for connectivity
speed, and machine vibration. Field service operations managers gain visibility
into device conditions and properties on a graphical dashboard. For example, the
capacity of a tank can be monitored through IoT Hub and represented on the
dashboard. When capacity reaches a threshold, an alert is sent to designated
users for follow-up action.
