---
title: Problēmas ar pārstāstās vai pārtrauktās ierīces noņemšanu no ierīču krājumiem
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564341"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="d33fe-102">Problēmas ar pārstāstās vai pārtrauktās ierīces noņemšanu no ierīču krājumiem</span><span class="sxs-lookup"><span data-stu-id="d33fe-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="d33fe-103">Microsoft Defender galapunktam pašlaik neļauj manuāli noņemt no ierīces izņemto vai pārtraukto ierīču ierakstu no ierīču krājumiem.</span><span class="sxs-lookup"><span data-stu-id="d33fe-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="d33fe-104">Drošības nolūkā ierīce paliek portālā kā vēsturisks ieraksts līdz 180 dienām.</span><span class="sxs-lookup"><span data-stu-id="d33fe-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="d33fe-105">Tomēr ierīces dati tiek iztīrīti atbilstoši jūsu konfigurētam saglabāšanas periodam.</span><span class="sxs-lookup"><span data-stu-id="d33fe-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="d33fe-106">**Piezīme.** Pēc septiņām dienām pārslēgsies pār pēc **pārstāstās** vai pēc lietošanas pārtraukšanas ierīce automātiski tiks pārslēgta uz neaktīvu stāvokli.</span><span class="sxs-lookup"><span data-stu-id="d33fe-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="d33fe-107">Turklāt pēdējo 30 dienu laikā neaktīviem ierīcēm netiek ņemti vērā dati, kas atspoguļo jūsu organizāciju un draudu un ievainojamības pārvaldība rezultātu vai Microsoft drošo rādītāju ierīcēm.</span><span class="sxs-lookup"><span data-stu-id="d33fe-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="d33fe-108">Ja joprojām nevēlaties skatīt noteiktas ierīces skatā Ierīču krājumi, mēģiniet novietot ierīces atzīmi, lai filtrētu pārtraukto ierīci no skata Ierīču krājumi.</span><span class="sxs-lookup"><span data-stu-id="d33fe-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="d33fe-109">Papildinformāciju skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="d33fe-109">For more information, see:</span></span>

[<span data-ttu-id="d33fe-110">Offboard devices from the Microsoft Defender for Endpoint service</span><span class="sxs-lookup"><span data-stu-id="d33fe-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="d33fe-111">Ekspozīcijas rezultāts draudu un ievainojamības pārvaldība</span><span class="sxs-lookup"><span data-stu-id="d33fe-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="d33fe-112">Neveselīgu sensoru labošana programmatūrā Microsoft Defender for Endpoint</span><span class="sxs-lookup"><span data-stu-id="d33fe-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="d33fe-113">Kā efektīvi izmantot atzīmes (1. daļa)</span><span class="sxs-lookup"><span data-stu-id="d33fe-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="d33fe-114">Kā efektīvi izmantot atzīmes (2. daļa)</span><span class="sxs-lookup"><span data-stu-id="d33fe-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="d33fe-115">Kā efektīvi izmantot atzīmes (3. daļa)</span><span class="sxs-lookup"><span data-stu-id="d33fe-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




