---
title: Programma Outlook darbvirsmas atcerēties vai aizstāt e-pasta ziņojumu
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389731"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="b38e8-102">Atsauktu vai aizstātu e-pasta ziņojumu</span><span class="sxs-lookup"><span data-stu-id="b38e8-102">Recall or replace an email message</span></span>

- <span data-ttu-id="b38e8-103">Kā administrators, varat **Atsaukt ziņojumus, izmantojot programmu PowerShell lietotāju vārdā**.</span><span class="sxs-lookup"><span data-stu-id="b38e8-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="b38e8-104">Ziņas no admin center nevar atsaukt.</span><span class="sxs-lookup"><span data-stu-id="b38e8-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="b38e8-105">Jūs varat **tikai atsaukt ziņojumus, kas nosūtīti cilvēkiem jūsu organizācijā**.</span><span class="sxs-lookup"><span data-stu-id="b38e8-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="b38e8-106">Ja ziņojums tika nosūtīts Gmail adresi, piemēram, nevaru atcerēties to.</span><span class="sxs-lookup"><span data-stu-id="b38e8-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="b38e8-107">Jūs varat **tikai atsaukt ziņojumus, kas nosūtīti no Outlook 2016 uz PC**.</span><span class="sxs-lookup"><span data-stu-id="b38e8-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="b38e8-108">Ja lietotājs nosūta īsziņu, izmantojot Mac programmu Outlook vai Outlook Web, to nevar atsaukt.</span><span class="sxs-lookup"><span data-stu-id="b38e8-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="b38e8-109">Lai atsauktu vai aizstātu e-pasta ziņojumu:</span><span class="sxs-lookup"><span data-stu-id="b38e8-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="b38e8-110">Mapju rūtī Outlook loga kreisajā pusē, izvēlieties mapi Nosūtītie vienumi.</span><span class="sxs-lookup"><span data-stu-id="b38e8-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="b38e8-111">Veiciet dubultklikšķi uz ziņojuma, kuru vēlaties atsaukt, lai to atvērtu.</span><span class="sxs-lookup"><span data-stu-id="b38e8-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="b38e8-112">Atlasiet cilni **ziņojums** un pēc tam atlasiet **darbību** > **Atsaukt šo ziņojumu**.</span><span class="sxs-lookup"><span data-stu-id="b38e8-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="b38e8-113">Atlasiet **Dzēst šī ziņojuma nelasītās kopijas** vai **Dzēst nelasītās kopijas un aizstāt ar jaunu ziņojumu**un pēc tam **Labi**.</span><span class="sxs-lookup"><span data-stu-id="b38e8-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="b38e8-114">Ja sūtāt ziņojumu Nomaiņa, sastādīt ziņojumu un pēc tam atlasiet **nosūtīt**.</span><span class="sxs-lookup"><span data-stu-id="b38e8-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="b38e8-115">Ziņojuma atsaukšanas izdošanās vai neizdošanās ir atkarīga no adresāta iestatījumus programmā Outlook.</span><span class="sxs-lookup"><span data-stu-id="b38e8-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="b38e8-116">Darbības, lai pārbaudītu par atsaukšanu, skatiet [šajā rakstā](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="b38e8-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="b38e8-117">Meklēt un dzēst e-pasta ziņojumus savā uzņēmumā</span><span class="sxs-lookup"><span data-stu-id="b38e8-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="b38e8-118">Ja jūs neesat globālās administrēšanas, jūsu kontā jābūt pievienotiem eDiscovery Manager lomu vai atbilstības meklēšanas pārvaldības loma, lai meklētu ziņojumus.</span><span class="sxs-lookup"><span data-stu-id="b38e8-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="b38e8-119">Lai izdzēstu ziņas, jums pievienoties uzņēmuma pārvaldības lomu grupas vai meklēšanas un iztīrīs pārvaldības lomu.</span><span class="sxs-lookup"><span data-stu-id="b38e8-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="b38e8-120">Atļaujas šīs lomas tiek piešķirtas [drošības un saskaņotības centrs](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="b38e8-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="b38e8-121">[Izveidošana satura meklēšanu](https://docs.microsoft.com/office365/securitycompliance/content-search) , lai atrastu ziņai un izdzēsiet.</span><span class="sxs-lookup"><span data-stu-id="b38e8-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="b38e8-122">[Drošības un atbilstības centrā PowerShell savienojumu](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="b38e8-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="b38e8-123">Ja jūs izmantojat vairāku faktoru autentifikaciju, skatiet [Office 365 drošību un atbilstību centra PowerShell savienojuma izveide, izmantojot vairāku faktoru autentifikaciju](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="b38e8-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>