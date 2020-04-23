---
title: Konfigurācijas pārvaldnieka ierīces, kas nav portālā
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789908"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="be782-102">Konfigurācijas pārvaldnieka ierīces, kas nav portālā</span><span class="sxs-lookup"><span data-stu-id="be782-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="be782-103">Lai ierīces sinhronizācija darbotos, [nepieciešamie interneta galapunktiem](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) jābūt sasniedzamiem no lokālā servera, kurā tiek viesota pakalpojuma savienojuma punkta loma.</span><span class="sxs-lookup"><span data-stu-id="be782-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="be782-104">Lai novērstu problēmas ar ierīces sinhronizēšanu, lūdzu, pārskatiet **CMGatewaySyncUploadWorker.log**, kas atrodas pakalpojuma savienojuma punktā.</span><span class="sxs-lookup"><span data-stu-id="be782-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="be782-105">Papildinformācija par [nomnieka pievienošanu Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="be782-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
