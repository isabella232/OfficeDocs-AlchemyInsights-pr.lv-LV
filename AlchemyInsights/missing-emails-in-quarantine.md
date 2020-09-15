---
title: Trūkstošie e-pasta ziņojumi karantīnā
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673721"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="c522f-102">Trūkstošie e-pasta ziņojumi karantīnā</span><span class="sxs-lookup"><span data-stu-id="c522f-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="c522f-103">Administratori var [Skatīt, izlaist vai izdzēst šos ziņojumus.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="c522f-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="c522f-104">Lai atvērtu drošības & atbilstības centru, dodieties uz [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="c522f-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="c522f-105">Lai tieši atvērtu karantīnas lapu, dodieties uz [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="c522f-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="c522f-106">Varat meklēt pēc šādām vērtībām:</span><span class="sxs-lookup"><span data-stu-id="c522f-106">You can search by the following values:</span></span>  

- <span data-ttu-id="c522f-107">**Ziņojuma ID**: ziņojuma globāli unikālais identifikators.</span><span class="sxs-lookup"><span data-stu-id="c522f-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="c522f-108">Ja sarakstā atlasāt ziņojumu,  **ziņojuma ID**  vērtība tiek rādīta rūtī  **Detalizēta informācija**  , kas tiek parādīta.</span><span class="sxs-lookup"><span data-stu-id="c522f-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="c522f-109">Administratori var izmantot [ziņojumu izsekošanu](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) , lai atrastu ziņojumus un to atbilstošos ziņojuma ID vērtības.</span><span class="sxs-lookup"><span data-stu-id="c522f-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="c522f-110">**Sūtītāja e-pasta adrese**: viena sūtītāja e-pasta adrese.</span><span class="sxs-lookup"><span data-stu-id="c522f-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="c522f-111">**Adresāta e-pasta adrese**: viena adresāta e-pasta adrese.</span><span class="sxs-lookup"><span data-stu-id="c522f-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="c522f-112">**Tēma**: izmantojiet visu ziņojuma tēmu.</span><span class="sxs-lookup"><span data-stu-id="c522f-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="c522f-113">Meklēšana nav reģistrjutīga.</span><span class="sxs-lookup"><span data-stu-id="c522f-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="c522f-114">Pēc meklēšanas kritēriju ievadīšanas noklikšķiniet uz ![ Atsvaidzināt pogas Atsvaidzināt ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **,** lai filtrētu rezultātus.  </span><span class="sxs-lookup"><span data-stu-id="c522f-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="c522f-115">Cmdlet, ko izmantojat, lai skatītu un pārvaldītu ziņojumus un failus karantīnā, ir šādi:</span><span class="sxs-lookup"><span data-stu-id="c522f-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="c522f-116">Dzēst-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="c522f-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="c522f-117">Eksportēšana — QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="c522f-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="c522f-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="c522f-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="c522f-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): ievērojiet, ka šajā cmdlet ir tikai ziņojumi, nevis ļaunprogrammatūras faili no ATP pakalpojumam SharePoint Online, OneDrive darbam vai Teams.</span><span class="sxs-lookup"><span data-stu-id="c522f-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="c522f-120">Laidiens — QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="c522f-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)