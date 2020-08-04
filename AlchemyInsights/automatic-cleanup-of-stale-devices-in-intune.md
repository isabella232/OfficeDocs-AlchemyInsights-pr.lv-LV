---
title: Novecojušu ierīču automātiska tīrīšana sistēmā Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555223"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="0dbcd-102">Novecojušu ierīču automātiska tīrīšana sistēmā Intune</span><span class="sxs-lookup"><span data-stu-id="0dbcd-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="0dbcd-103">Intune sniedz administratoram iespēju konfigurēt laika intervālu starp 90 un 270 dienām, pēc kura sasmacis ierīces tiek noņemtas no pakalpojuma.</span><span class="sxs-lookup"><span data-stu-id="0dbcd-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="0dbcd-104">Šis iestatījums ir organizācijas mērogs, un pēc tam, kad tā ir aktivizēta, ir spēkā nekavējoties.</span><span class="sxs-lookup"><span data-stu-id="0dbcd-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="0dbcd-105">Visas ierīces, kuras nav pārbaudījušas Intune serverī uz periodu, kas pārsniedz iestatījumu, tiek neatgriezeniski izdzēstas.</span><span class="sxs-lookup"><span data-stu-id="0dbcd-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="0dbcd-106">**Piezīmes** Šī tīrīšanas darbība atbilst tikai MDM ierīces objektiem.</span><span class="sxs-lookup"><span data-stu-id="0dbcd-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="0dbcd-107">Tikai EAS ierīces objekti tiek izslēgti.</span><span class="sxs-lookup"><span data-stu-id="0dbcd-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="0dbcd-108">Lai iegūtu papildinformāciju par to, kad ierīce ir piemērota dzēšanai, ņemot vērā ierīces tīrīšanas iestatījumu un tās "stāvokli":</span><span class="sxs-lookup"><span data-stu-id="0dbcd-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="0dbcd-109">Iestatījums: **izdzēsiet ierīces pēc pēdējā atdošanas datuma: Jā (zināma vērtība (N) noteiktās dienās)**</span><span class="sxs-lookup"><span data-stu-id="0dbcd-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="0dbcd-110">Atkarībā no parametra Value (N), Intune pakalpojums izdzēš ierīci norādītajās dienās pēc tam, kad tā pēdējoreiz ir veiksmīgi pārbaudīta.</span><span class="sxs-lookup"><span data-stu-id="0dbcd-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="0dbcd-111">Iestatījums: **pēc pēdējā atdošanas datuma dzēst ierīces: Nē**</span><span class="sxs-lookup"><span data-stu-id="0dbcd-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="0dbcd-112">180 dienas pēc tam, kad ierīces sertifikāts ir beidzies un nav atjaunots, ierīce tiek izdzēsta.</span><span class="sxs-lookup"><span data-stu-id="0dbcd-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="0dbcd-113">**Piezīmes** Abos gadījumos ierīce ir veiksmīgi reģistrēta Intune.</span><span class="sxs-lookup"><span data-stu-id="0dbcd-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="0dbcd-114">Reģistrācija notiek pirmās ierīces atdošanas laikā ar Intune pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="0dbcd-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="0dbcd-115">Ja ierīce veiksmīgi piesakās Intune, bet nekļūst par Intune reģistrēto, šī ierīce tiek izdzēsta 270 dienās pēc reģistrācijas.</span><span class="sxs-lookup"><span data-stu-id="0dbcd-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="0dbcd-116">(90 dienas, lai atzīmētu ierīci kā atsauktu, un pēc tam vēl 180 dienas, lai dzēstu ierakstu.)</span><span class="sxs-lookup"><span data-stu-id="0dbcd-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="0dbcd-117">Šobrīd Intune konsolē nepastāv mehānisms, lai noteiktu ierīces sertificēšanas derīguma termiņu katrai ierīcei.</span><span class="sxs-lookup"><span data-stu-id="0dbcd-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>