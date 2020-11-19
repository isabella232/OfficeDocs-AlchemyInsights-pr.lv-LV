---
title: E-pasta ziņojuma atsaukšana vai aizstāšana
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353513"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="9eed0-102">E-pasta ziņojuma atsaukšana vai aizstāšana programmā Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9eed0-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="9eed0-103">Varat **tikai atsaukt ziņojumus, kas tiek nosūtīti lietotājiem jūsu organizācijā**.</span><span class="sxs-lookup"><span data-stu-id="9eed0-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="9eed0-104">Piemēram, ja ziņojums tika nosūtīts uz Gmail adresi, to nevar atsaukt.</span><span class="sxs-lookup"><span data-stu-id="9eed0-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="9eed0-105">**No datora Outlook sūtītos ziņojumus varat atsaukt**.</span><span class="sxs-lookup"><span data-stu-id="9eed0-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="9eed0-106">Ja lietotājs nosūta ziņojumu, izmantojot programmu Outlook darbam ar Mac vai Outlook tīmeklī, to nevar atsaukt.</span><span class="sxs-lookup"><span data-stu-id="9eed0-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="9eed0-107">Kā nomnieka administrators varat **Atsaukt ziņojumus lietotāju vārdā, izmantojot PowerShell** (Papildinformācija atrodama rakstā [e-pasta ziņojumu meklēšana un dzēšana](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="9eed0-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="9eed0-108">Jūs nevarat atsaukt ziņojumus no administrēšanas centra.</span><span class="sxs-lookup"><span data-stu-id="9eed0-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="9eed0-109">Lai iegūtu papildinformāciju, ritiniet uz leju līdz opcijai meklēt un izdzēst e-pasta ziņojumus jūsu organizācijā.</span><span class="sxs-lookup"><span data-stu-id="9eed0-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="9eed0-110">**Nosūtīta e-pasta ziņojuma atsaukšana vai aizstāšana**</span><span class="sxs-lookup"><span data-stu-id="9eed0-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="9eed0-111">Mapju rūtī, kas atrodas pa kreisi no Outlook loga, izvēlieties mapi Nosūtītie vienumi.</span><span class="sxs-lookup"><span data-stu-id="9eed0-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="9eed0-112">Atveriet ziņojumu, kuru vēlaties atsaukt.</span><span class="sxs-lookup"><span data-stu-id="9eed0-112">Open the message that you want to recall.</span></span> <span data-ttu-id="9eed0-113">Lai atvērtu ziņojumu, veiciet uz tā dubultklikšķi.</span><span class="sxs-lookup"><span data-stu-id="9eed0-113">You must double-click to open the message.</span></span> <span data-ttu-id="9eed0-114">Atlasiet ziņojumu, lai tas tiktu parādīts lasīšanas rūtī, Neļaujiet atsaukt ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="9eed0-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="9eed0-115">Cilnē ziņojums atlasiet **darbības**  >  **Šī ziņojuma atsaukšana**.</span><span class="sxs-lookup"><span data-stu-id="9eed0-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="9eed0-116">Izvēlieties **Dzēst šī ziņojuma nelasītās kopijas** vai **Dzēst nelasītās kopijas un aizstāt ar jaunu ziņojumu un** pēc tam atlasiet **Labi**.</span><span class="sxs-lookup"><span data-stu-id="9eed0-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="9eed0-117">Ja sūtāt aizstāšanas ziņojumu, izveidojiet ziņojumu un pēc tam atlasiet **Sūtīt**.</span><span class="sxs-lookup"><span data-stu-id="9eed0-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="9eed0-118">Ziņojuma atsaukšanas sekmīgs vai neizdošanās ir atkarīgs no adresātu iestatījumiem programmā Outlook.</span><span class="sxs-lookup"><span data-stu-id="9eed0-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="9eed0-119">Papildinformāciju par atsaukšanu skatiet rakstā [e-pasta ziņojuma atsaukšana vai aizstāšana](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="9eed0-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="9eed0-120">**_Lai meklētu un izdzēstu e-pasta ziņojumus savā organizācijā_**, ir vienkāršāk, ja esat globālais administrators. Ja neesat globālais administrators, jūsu konts ir jāpievieno e-datu atklāšanas pārvaldnieka lomu grupai vai atbilstības meklēšanas pārvaldības lomai.</span><span class="sxs-lookup"><span data-stu-id="9eed0-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="9eed0-121">Lai izdzēstu ziņojumus, ir jāpievienojas organizācijas pārvaldības lomu grupai vai meklēšanas un iztīrīšanas pārvaldības lomai.</span><span class="sxs-lookup"><span data-stu-id="9eed0-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="9eed0-122">Atļaujas šīm lomām tiek piešķirtas [drošības & atbilstības centrā](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="9eed0-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="9eed0-123">[Izveidojiet satura meklēšanu](https://docs.microsoft.com/microsoft-365/compliance/content-search) , lai atrastu dzēšamo ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="9eed0-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="9eed0-124">[Savienojuma izveide ar drošības & atbilstības centra PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="9eed0-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="9eed0-125">Ja izmantojat MFA (daudzfaktoru autentifikācija), skatiet rakstu [savienojuma izveide ar Microsoft 365 Security & atbilstības centra PowerShell, izmantojot daudzfaktoru autentifikāciju](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="9eed0-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
