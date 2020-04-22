---
title: Outlook darbvirsmas atsaukšana vai aizstājiet e-pasta ziņojumu
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687517"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="d0358-102">Outlook e-pasta ziņojuma atsaukšana vai aizstāšana</span><span class="sxs-lookup"><span data-stu-id="d0358-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="d0358-103">Kā admin, jūs varat **Atsaukt ziņojumus vārdā lietotājiem, izmantojot PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="d0358-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="d0358-104">Ziņojumus nevar atsaukt administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="d0358-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="d0358-105">Varat **atsaukt tikai tos ziņojumus, kas nosūtīti personām jūsu organizācijā**.</span><span class="sxs-lookup"><span data-stu-id="d0358-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="d0358-106">Piemēram, ja ziņojums ir nosūtīts uz Gmail adresi, to nevar atsaukt.</span><span class="sxs-lookup"><span data-stu-id="d0358-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="d0358-107">**No datora var tikai atsaukt ziņojumus, kas nosūtīti no programmas Outlook 2016**.</span><span class="sxs-lookup"><span data-stu-id="d0358-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="d0358-108">Ja lietotājs nosūta ziņojumu, izmantojot Outlook Mac vai Outlook Web, to nevar atsaukt.</span><span class="sxs-lookup"><span data-stu-id="d0358-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="d0358-109">Lai atsauktu vai aizstātu e-pasta ziņojumu:</span><span class="sxs-lookup"><span data-stu-id="d0358-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="d0358-110">Mapju rūtī, kas atrodas Outlook loga kreisajā pusē, atlasiet mapi Nosūtītie vienumi.</span><span class="sxs-lookup"><span data-stu-id="d0358-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="d0358-111">Veiciet dubultklikšķi uz ziņojuma, kuru vēlaties atsaukt, lai to atvērtu.</span><span class="sxs-lookup"><span data-stu-id="d0358-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="d0358-112">Atlasiet cilni **ziņojums** un pēc tam atlasiet **darbības** > **Atsaukt šo ziņojumu**.</span><span class="sxs-lookup"><span data-stu-id="d0358-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="d0358-113">Atlasiet **Dzēst šī ziņojuma nelasītās kopijas** vai **Dzēst nelasītās kopijas un aizstāt ar jaunu ziņojumu**un pēc tam atlasiet **Labi**.</span><span class="sxs-lookup"><span data-stu-id="d0358-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="d0358-114">Ja sūtāt ziņojumu ar aizstājējziņu, Sastādiet ziņojumu un pēc tam atlasiet **Sūtīt**.</span><span class="sxs-lookup"><span data-stu-id="d0358-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="d0358-115">Ziņojumu atsaukšanas izdošanās vai neveiksme ir atkarīga no adresāta iestatījumiem programmā Outlook.</span><span class="sxs-lookup"><span data-stu-id="d0358-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="d0358-116">Lai pārbaudītu atsaukuma darbības, skatiet [šo rakstu](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="d0358-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="d0358-117">E-pasta ziņojumu meklēšana un dzēšana organizācijā</span><span class="sxs-lookup"><span data-stu-id="d0358-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="d0358-118">Ja neesat globālais administrators, jūsu konts ir jāpievieno lomai eDiscovery Manager loma vai atbilstības meklēšanas pārvaldība, lai meklētu ziņojumus.</span><span class="sxs-lookup"><span data-stu-id="d0358-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="d0358-119">Lai dzēstu ziņojumus, ir jāpievienojas organizācijas pārvaldības lomu grupai vai lomai meklēšanas un tīrīšanas pārvaldība.</span><span class="sxs-lookup"><span data-stu-id="d0358-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="d0358-120">Šo lomu atļaujas tiek piešķirtas [drošības un atbilstības centrā](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="d0358-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="d0358-121">[Izveidojiet satura meklēšanu](https://docs.microsoft.com/office365/securitycompliance/content-search) , lai atrastu dzēšamo ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="d0358-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="d0358-122">[Izveidot savienojumu ar drošības un atbilstības centra PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d0358-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="d0358-123">Ja izmantojat vairāku faktoru autentifikāciju, skatiet [izveidot savienojumu ar Microsoft 365 drošības un atbilstības centrs PowerShell, izmantojot vairāku faktoru autentifikācija](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d0358-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>