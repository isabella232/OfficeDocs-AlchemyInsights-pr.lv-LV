---
title: E-pasta ziņojumu meklēšana un dzēšana savā organizācijā
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525434"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="9dc04-102">E-pasta ziņojumu meklēšana un dzēšana savā organizācijā</span><span class="sxs-lookup"><span data-stu-id="9dc04-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="9dc04-103">Izpildiet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="9dc04-103">Follow these steps:</span></span>

1. <span data-ttu-id="9dc04-104">Ja neesat globālais administrators, varat meklēt ziņojumus, kas jūsu kontam ir jāpievieno **e-datu atklāšanas pārvaldnieka lomu grupai** vai **atbilstības meklēšanas pārvaldības lomai**.</span><span class="sxs-lookup"><span data-stu-id="9dc04-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="9dc04-105">Lai izdzēstu ziņojumus, ir jāpievienojas **organizācijas pārvaldības lomu grupai** vai **meklēšanas un iztīrīšanas pārvaldības lomai**.</span><span class="sxs-lookup"><span data-stu-id="9dc04-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="9dc04-106">Atļaujas šīm lomām tiek piešķirtas [drošības & atbilstības centrā.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="9dc04-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="9dc04-107">[Izveidojiet satura meklēšanu](https://docs.microsoft.com/office365/securitycompliance/content-search) , lai atrastu dzēšamo ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="9dc04-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="9dc04-108">[Savienojuma izveide ar drošības & atbilstības centra PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="9dc04-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="9dc04-109">Ja izmantojat MFA, skatiet šos norādījumus: savienojuma izveide [ar drošības & atbilstības centra PowerShell, izmantojot daudzfaktoru autentifikāciju](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="9dc04-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="9dc04-110">Dzēst ziņojumu: palaidiet `New-ComplianceSearchAction` cmdlet, lai izdzēstu ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="9dc04-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="9dc04-111">Izdzēstie ziņojumi tiek pārvietoti uz lietotāja atkopto vienumu mapi.</span><span class="sxs-lookup"><span data-stu-id="9dc04-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="9dc04-112">Lai iegūtu komandu piemērs, skatiet sadaļu [3. darbība: ziņojuma dzēšana.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="9dc04-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
