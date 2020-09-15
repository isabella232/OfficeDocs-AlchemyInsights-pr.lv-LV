---
title: ATP darbam ar SharePoint, OneDrive un Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715568"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="13eb7-102">ATP darbam ar SharePoint, OneDrive un Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="13eb7-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="13eb7-103">Veiciet šīs darbības, lai iespējotu uzlabotu apdraudējumu aizsardzību:</span><span class="sxs-lookup"><span data-stu-id="13eb7-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="13eb7-104">Dodieties uz [https://protection.office.com](https://protection.office.com) un pierakstieties, izmantojot globālo administratora vai drošības administratora kontu.</span><span class="sxs-lookup"><span data-stu-id="13eb7-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="13eb7-105">Kreisajā navigācijas rūtī sadaļā **draudu pārvaldība**izvēlieties **politikas** \> **droši pielikumi**.</span><span class="sxs-lookup"><span data-stu-id="13eb7-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="13eb7-106">Atlasiet **Ieslēgt ATP pakalpojumam SharePoint, OneDrive un Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="13eb7-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="13eb7-107">[Izveidojiet darbību brīdinājumu politiku](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) , lai saņemtu paziņojumus, kad atklājam ļaunprātīgus failus.</span><span class="sxs-lookup"><span data-stu-id="13eb7-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="13eb7-108">Pilnus norādījumus skatiet šajā [tēmā](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="13eb7-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="13eb7-109">**Piezīme**: pēc noformējuma ATP neskenē nevienu failu pakalpojumā SharePoint Online, OneDrive darbam vai Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="13eb7-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="13eb7-110">Faili tiek skenēti asinhroni, veicot procesu, kas izmanto koplietošanas aktivitāti, viesa aktivitāti un draudu signālus, lai identificētu ļaunprātīgus failus.</span><span class="sxs-lookup"><span data-stu-id="13eb7-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="13eb7-111">Papildinformāciju skatiet šajā [tēmā](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="13eb7-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
