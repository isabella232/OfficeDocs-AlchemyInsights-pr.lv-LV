---
title: Outlook datora atsaukšana vai aizstāšana e-pasta ziņojums
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663997"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="100a9-102">Outlook e-pasta ziņojuma atsaukšana vai aizstāšana</span><span class="sxs-lookup"><span data-stu-id="100a9-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="100a9-103">Kā administrators varat **Atsaukt ziņojumus lietotāju vārdā, izmantojot PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="100a9-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="100a9-104">Jūs nevarat atsaukt ziņojumus no administrēšanas centra.</span><span class="sxs-lookup"><span data-stu-id="100a9-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="100a9-105">Varat **tikai atsaukt ziņojumus, kas tiek nosūtīti lietotājiem jūsu organizācijā**.</span><span class="sxs-lookup"><span data-stu-id="100a9-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="100a9-106">Ja ziņojums tika nosūtīts uz Gmail adresi, piemēram, varat to atsaukt.</span><span class="sxs-lookup"><span data-stu-id="100a9-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="100a9-107">Jūs varat **no datora sūtīt ziņojumus tikai no Outlook 2016**.</span><span class="sxs-lookup"><span data-stu-id="100a9-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="100a9-108">Ja lietotājs nosūta ziņojumu, izmantojot programmu Outlook darbam ar Mac vai Outlook tīmeklī, to nevar atsaukt.</span><span class="sxs-lookup"><span data-stu-id="100a9-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="100a9-109">Lai atsauktu vai aizstātu e-pasta ziņojumu:</span><span class="sxs-lookup"><span data-stu-id="100a9-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="100a9-110">Mapju rūtī, kas atrodas pa kreisi no Outlook loga, atlasiet mapi Nosūtītie vienumi.</span><span class="sxs-lookup"><span data-stu-id="100a9-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="100a9-111">Veiciet dubultklikšķi uz ziņojuma, ko vēlaties atsaukt, lai to atvērtu.</span><span class="sxs-lookup"><span data-stu-id="100a9-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="100a9-112">Atlasiet cilni **ziņojums** un pēc tam atlasiet **darbības**, lai  >  **atsauktu šo ziņojumu**.</span><span class="sxs-lookup"><span data-stu-id="100a9-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="100a9-113">Atlasiet **Dzēst šī ziņojuma nelasītās kopijas** vai **Dzēst nelasītās kopijas un aizstāt ar jaunu ziņojumu**un pēc tam atlasiet **Labi**.</span><span class="sxs-lookup"><span data-stu-id="100a9-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="100a9-114">Ja sūtāt aizstāšanas ziņojumu, izveidojiet ziņojumu un pēc tam atlasiet **Sūtīt**.</span><span class="sxs-lookup"><span data-stu-id="100a9-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="100a9-115">Ziņojuma atsaukšanas sekmīgs vai neizdošanās ir atkarīgs no adresāta iestatījumiem programmā Outlook.</span><span class="sxs-lookup"><span data-stu-id="100a9-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="100a9-116">Lai uzzinātu, kādas darbības ir jāveic, skatiet [šo rakstu](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="100a9-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="100a9-117">E-pasta ziņojumu meklēšana un dzēšana savā organizācijā</span><span class="sxs-lookup"><span data-stu-id="100a9-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="100a9-118">Ja neesat globālais administrators, jūsu kontam jābūt pievienotai e-datu atklāšanas pārvaldnieka lomai vai atbilstības meklēšanas pārvaldības lomai, lai meklētu ziņojumus.</span><span class="sxs-lookup"><span data-stu-id="100a9-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="100a9-119">Lai izdzēstu ziņojumus, ir jāpievienojas organizācijas pārvaldības lomu grupai vai meklēšanas un iztīrīšanas pārvaldības lomai.</span><span class="sxs-lookup"><span data-stu-id="100a9-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="100a9-120">Šo lomu atļaujas ir piešķirtas [drošības un atbilstības centrā](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="100a9-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="100a9-121">[Izveidojiet satura meklēšanu](https://docs.microsoft.com/microsoft-365/compliance/content-search) , lai atrastu dzēšamo ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="100a9-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="100a9-122">[Savienojuma izveide ar drošības un atbilstības centra PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="100a9-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="100a9-123">Ja izmantojat daudzfaktoru autentifikāciju, skatiet rakstu [savienojuma izveide ar Microsoft 365 Security un Compliance Center PowerShell, izmantojot daudzfaktoru autentifikāciju](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="100a9-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>