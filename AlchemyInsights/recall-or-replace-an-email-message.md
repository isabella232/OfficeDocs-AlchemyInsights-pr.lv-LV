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
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799211"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="679d0-102">E-pasta ziņojuma atsaukšana vai aizstāšana programmā Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="679d0-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="679d0-103">Varat **tikai atsaukt ziņojumus, kas tiek nosūtīti lietotājiem jūsu organizācijā**.</span><span class="sxs-lookup"><span data-stu-id="679d0-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="679d0-104">Ja ziņojums tika nosūtīts uz Gmail adresi, piemēram, varat to atsaukt.</span><span class="sxs-lookup"><span data-stu-id="679d0-104">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="679d0-105">Varat **atsaukt no programmas Outlook 2016 sūtītos ZIŅOJUMUS datorā**.</span><span class="sxs-lookup"><span data-stu-id="679d0-105">You can **only recall messages sent from Outlook 2016 for the PC**.</span></span> <span data-ttu-id="679d0-106">Ja lietotājs nosūta ziņojumu, izmantojot programmu Outlook darbam ar Mac vai Outlook tīmeklī, to nevar atsaukt.</span><span class="sxs-lookup"><span data-stu-id="679d0-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="679d0-107">Ja esat administrators, varat **Atsaukt ziņojumus lietotāju vārdā, izmantojot PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="679d0-107">If you're an admin, you can **recall messages on behalf of users by using PowerShell**.</span></span> <span data-ttu-id="679d0-108">Jūs nevarat atsaukt ziņojumus no administrēšanas centra.</span><span class="sxs-lookup"><span data-stu-id="679d0-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="679d0-109">Lai iegūtu papildinformāciju, ritiniet uz leju līdz opcijai meklēt un izdzēst e-pasta ziņojumus jūsu organizācijā.</span><span class="sxs-lookup"><span data-stu-id="679d0-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="679d0-110">**Nosūtīta e-pasta ziņojuma atsaukšana vai aizstāšana**</span><span class="sxs-lookup"><span data-stu-id="679d0-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="679d0-111">Mapju rūtī, kas atrodas pa kreisi no Outlook loga, izvēlieties mapi Nosūtītie vienumi.</span><span class="sxs-lookup"><span data-stu-id="679d0-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="679d0-112">Atveriet ziņojumu, kuru vēlaties atsaukt.</span><span class="sxs-lookup"><span data-stu-id="679d0-112">Open the message that you want to recall.</span></span> <span data-ttu-id="679d0-113">Lai atvērtu ziņojumu, veiciet uz tā dubultklikšķi.</span><span class="sxs-lookup"><span data-stu-id="679d0-113">You must double-click to open the message.</span></span> <span data-ttu-id="679d0-114">Atlasiet ziņojumu, lai tas tiktu parādīts lasīšanas rūtī, Neļaujiet atsaukt ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="679d0-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="679d0-115">Cilnē ziņojums atlasiet **darbības**  >  **Šī ziņojuma atsaukšana**.</span><span class="sxs-lookup"><span data-stu-id="679d0-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="679d0-116">Izvēlieties **Dzēst šī ziņojuma nelasītās kopijas** vai **Dzēst nelasītās kopijas un aizstāt ar jaunu ziņojumu un**pēc tam atlasiet **Labi**.</span><span class="sxs-lookup"><span data-stu-id="679d0-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="679d0-117">Ja sūtāt aizstāšanas ziņojumu, izveidojiet ziņojumu un pēc tam atlasiet **Sūtīt**.</span><span class="sxs-lookup"><span data-stu-id="679d0-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="679d0-118">Ziņojuma atsaukšanas sekmīgs vai neizdošanās ir atkarīgs no adresātu iestatījumiem programmā Outlook.</span><span class="sxs-lookup"><span data-stu-id="679d0-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="679d0-119">Papildinformāciju par atsaukšanu skatiet rakstā [e-pasta ziņojuma atsaukšana vai aizstāšana](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="679d0-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="679d0-120">***E-pasta ziņojumu meklēšana un dzēšana savā organizācijā*** Lai meklētu un izdzēstu e-pasta ziņojumus savā organizācijā, ir vienkāršāk, ja esat globālais administrators. Ja neesat globālais administrators, jūsu konts ir jāpievieno e-datu atklāšanas pārvaldnieka lomu grupai vai atbilstības meklēšanas pārvaldības lomai.</span><span class="sxs-lookup"><span data-stu-id="679d0-120">***Search for and delete email messages in your organization*** To search for and delete email messages in your organization, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="679d0-121">Lai izdzēstu ziņojumus, ir jāpievienojas organizācijas pārvaldības lomu grupai vai meklēšanas un iztīrīšanas pārvaldības lomai.</span><span class="sxs-lookup"><span data-stu-id="679d0-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="679d0-122">Atļaujas šīm lomām tiek piešķirtas [drošības & atbilstības centrā](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="679d0-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="679d0-123">[Izveidojiet satura meklēšanu](https://docs.microsoft.com/microsoft-365/compliance/content-search) , lai atrastu dzēšamo ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="679d0-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="679d0-124">[Savienojuma izveide ar drošības & atbilstības centra PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="679d0-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span> 

<span data-ttu-id="679d0-125">Ja izmantojat MFA, skatiet rakstu [savienojuma izveide ar Microsoft 365 security & atbilstības centra PowerShell, izmantojot daudzfaktoru autentifikāciju](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="679d0-125">If you're using MFA, see [Connect to Microsoft 365 security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span> 
