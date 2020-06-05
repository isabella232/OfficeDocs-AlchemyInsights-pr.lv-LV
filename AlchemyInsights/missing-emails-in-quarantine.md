---
title: Trūkst e-pasta karantīnā
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569233"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="5a0a6-102">Trūkst e-pasta ziņojumu karantīnā "</span><span class="sxs-lookup"><span data-stu-id="5a0a6-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="5a0a6-103">Administratori var [Skatīt, izlaist vai dzēst šos ziņojumus.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="5a0a6-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="5a0a6-104">Lai atvērtu drošības & atbilstības centru, dodieties uz [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="5a0a6-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="5a0a6-105">Lai tieši atvērtu karantīnas lapu, dodieties uz [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="5a0a6-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="5a0a6-106">Jūs varat meklēt pēc šādām vērtībām:</span><span class="sxs-lookup"><span data-stu-id="5a0a6-106">You can search by the following values:</span></span>  

- <span data-ttu-id="5a0a6-107">**Ziņojuma ID**: ziņojuma vispārēji unikālais identifikators.</span><span class="sxs-lookup"><span data-stu-id="5a0a6-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="5a0a6-108">Ja sarakstā atlasāt ziņojumu, **ziņojuma ID** vērtība tiek parādīta **informācijas** izlidošanas rūtī, kas tiek parādīta.</span><span class="sxs-lookup"><span data-stu-id="5a0a6-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="5a0a6-109">Administratori var izmantot [ziņojumu trasēšanas](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) atrast ziņojumus un to atbilstošo ziņojumu ID vērtības.</span><span class="sxs-lookup"><span data-stu-id="5a0a6-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="5a0a6-110">**Sūtītāja e-pasta adrese**: viena sūtītāja e-pasta adrese.</span><span class="sxs-lookup"><span data-stu-id="5a0a6-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="5a0a6-111">**Adresāta e-pasta adrese**: viena adresāta e-pasta adrese.</span><span class="sxs-lookup"><span data-stu-id="5a0a6-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="5a0a6-112">**Tēma**: izmantojiet visu ziņojuma tēmu.</span><span class="sxs-lookup"><span data-stu-id="5a0a6-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="5a0a6-113">Meklēšana nav reģistrjutīga.</span><span class="sxs-lookup"><span data-stu-id="5a0a6-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="5a0a6-114">Pēc meklēšanas kritēriju ievadīšanas noklikšķiniet uz ![ Atsvaidzināt atsvaidzināšanas pogas, ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** lai filtrētu rezultātus.  </span><span class="sxs-lookup"><span data-stu-id="5a0a6-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="5a0a6-115">Cmdlet, ko izmanto, lai skatītu un pārvaldīt ziņojumus un failus karantīnā, ir šādi:</span><span class="sxs-lookup"><span data-stu-id="5a0a6-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="5a0a6-116">Izdzēst-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="5a0a6-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="5a0a6-117">Eksports-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="5a0a6-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="5a0a6-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="5a0a6-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="5a0a6-119">[Priekšapskate-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Ņemiet vērā, ka šī cmdlet ir tikai ziņojumi, nevis Malware failus no ATP SharePoint Online, OneDrive uzņēmumiem vai darba grupas.</span><span class="sxs-lookup"><span data-stu-id="5a0a6-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="5a0a6-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="5a0a6-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)