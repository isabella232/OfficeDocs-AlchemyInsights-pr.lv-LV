---
title: Trūkstoši e-pasta ziņojumi karantīnā
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831741"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="14525-102">Missing emails in quarantine"</span><span class="sxs-lookup"><span data-stu-id="14525-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="14525-103">Administratori [var skatīt, izlaist vai dzēst šos ziņojumus.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="14525-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="14525-104">Lai atvērtu drošības & centru, dodieties uz [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="14525-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="14525-105">Lai tieši atvērtu lapu Karantīnā, dodieties uz [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="14525-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="14525-106">Varat meklēt pēc šādām vērtībām:</span><span class="sxs-lookup"><span data-stu-id="14525-106">You can search by the following values:</span></span>  

- <span data-ttu-id="14525-107">**Ziņojuma ID:** ziņojuma globāli unikāls identifikators.</span><span class="sxs-lookup"><span data-stu-id="14525-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="14525-108">Ja sarakstā atlasāt ziņojumu, izlidošanas rūtī  Detalizēti tiek rādīta vērtība Ziņojuma **ID.**</span><span class="sxs-lookup"><span data-stu-id="14525-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="14525-109">Administratori var izmantot ziņojumu [izsekošanu,](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) lai atrastu ziņojumus un to atbilstošās vērtības Ziņojuma ID.</span><span class="sxs-lookup"><span data-stu-id="14525-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="14525-110">**Sūtītāja e-pasta** adrese: viena sūtītāja e-pasta adrese.</span><span class="sxs-lookup"><span data-stu-id="14525-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="14525-111">**Adresāta e-pasta** adrese: viena adresāta e-pasta adrese.</span><span class="sxs-lookup"><span data-stu-id="14525-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="14525-112">**Tēma:** izmantojiet visu ziņojuma tēmu.</span><span class="sxs-lookup"><span data-stu-id="14525-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="14525-113">Meklēšana nav reģistrjutīga.</span><span class="sxs-lookup"><span data-stu-id="14525-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="14525-114">Kad esat ievadījis meklēšanas kritērijus, noklikšķiniet uz ![ Atsvaidzināt pogas ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Atsvaidzināt,** lai filtrētu rezultātus.  </span><span class="sxs-lookup"><span data-stu-id="14525-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="14525-115">Cmdlet, kuras izmantojat ziņojumu un failu skatīšanai un pārvaldīšanai karantīnā, ir:</span><span class="sxs-lookup"><span data-stu-id="14525-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="14525-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="14525-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="14525-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="14525-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="14525-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="14525-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="14525-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Ņemiet vērā, ka šī cmdlet ir pieejama tikai ziņojumiem, nevis ļaunprogrammatūras failiem no ATP pakalpojumā SharePoint Online, OneDrive darbam vai Teams.</span><span class="sxs-lookup"><span data-stu-id="14525-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="14525-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="14525-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)