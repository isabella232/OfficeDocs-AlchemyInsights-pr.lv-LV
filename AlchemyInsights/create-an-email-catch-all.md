---
title: E-pasta nozvejas izveide visiem
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
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712993"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="e1470-102">E-pasta nozvejas izveide visiem</span><span class="sxs-lookup"><span data-stu-id="e1470-102">Create an email catch all</span></span>

<span data-ttu-id="e1470-103">Ir stingri kavēta nozvejas lietošana.</span><span class="sxs-lookup"><span data-stu-id="e1470-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="e1470-104">Labāk ir nodrošināt atlēcienu sūtītājam, kas nosūta sūtītājus par to, ka viņu ziņojumu nevarēja nosūtīt kā adresētu, lai viņi varētu rīkoties.</span><span class="sxs-lookup"><span data-stu-id="e1470-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="e1470-105">Varat arī ierobežot monitorētās pastkastes tikai iepriekš derīgās e-pasta adreses.</span><span class="sxs-lookup"><span data-stu-id="e1470-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="e1470-106">Visas nozvejas visas pastkastes saņems lielu surogātpasta daudzumu, un tā, iespējams, tiks aizpildīta, ja netiek stingri pārraudzīta.</span><span class="sxs-lookup"><span data-stu-id="e1470-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="e1470-107">(Ir saņemti ierobežojumi.)</span><span class="sxs-lookup"><span data-stu-id="e1470-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="e1470-108">Ja izlemjat turpināt, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="e1470-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="e1470-109">Izveidojiet dinamisku adresātu grupu & iekļaujiet visus adresātu tipus.</span><span class="sxs-lookup"><span data-stu-id="e1470-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="e1470-110">Izveidojiet atvēlētu pastkasti e-pasta ziņojumu nozvejai, piemēram, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="e1470-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="e1470-111">Konkrētajā domēnā iestatiet DomainType uz "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="e1470-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="e1470-112">Ja vēlāk noņemat catch all, noteikti iestatiet domēnu atpakaļ uz autoritatīvo.</span><span class="sxs-lookup"><span data-stu-id="e1470-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="e1470-113">Izveidojiet pasta risinātājahttps://Configure.Office.com/Scenario.aspx?SID=12 transporta kārtulu šādi:</span><span class="sxs-lookup"><span data-stu-id="e1470-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="e1470-114">Ja sūtītājs ir ārpus organizācijas</span><span class="sxs-lookup"><span data-stu-id="e1470-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="e1470-115">Ziņojuma novirzīšana uz Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="e1470-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="e1470-116">Izņemot gadījumus, kad adresāts ir allusers@domain.com dalībnieks (adresātu grupā ir visi dalībnieki)</span><span class="sxs-lookup"><span data-stu-id="e1470-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="e1470-117">Nodrošiniet, lai validētu, ka jaunās pastkastes tiek pievienotas dinamiskās adresātu grupai</span><span class="sxs-lookup"><span data-stu-id="e1470-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
