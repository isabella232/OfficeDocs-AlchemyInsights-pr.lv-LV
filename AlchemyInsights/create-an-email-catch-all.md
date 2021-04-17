---
title: E-pasta tvert visu izveide
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816207"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="149e9-102">E-pasta tvert visu izveide</span><span class="sxs-lookup"><span data-stu-id="149e9-102">Create an email catch all</span></span>

<span data-ttu-id="149e9-103">Tvert visu izmantošana ir ļoti neiesarunāta.</span><span class="sxs-lookup"><span data-stu-id="149e9-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="149e9-104">Ir labāk nodrošināt atsišanu atpakaļ uz sūtītāju, kas informēja sūtītājus par to, ka viņu ziņojumus nevarēja piegādāt, lai viņi varētu rīkoties.</span><span class="sxs-lookup"><span data-stu-id="149e9-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="149e9-105">Varat arī ierobežot pārraudzīto pastkasti, lai tā tvertu tikai iepriekš derīgas e-pasta adreses.</span><span class="sxs-lookup"><span data-stu-id="149e9-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="149e9-106">Jebkura tvērēja no visām pastkastēm saņems daudz surogātpasta, un tas var tikt aizpildīts, ja netiks rūpīgi pārraudzīts.</span><span class="sxs-lookup"><span data-stu-id="149e9-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="149e9-107">(Pastāv saņemšanas ierobežojumi.)</span><span class="sxs-lookup"><span data-stu-id="149e9-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="149e9-108">Ja izlemjat turpināt, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="149e9-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="149e9-109">Izveidojiet dinamisko adresātu grupu, & ietvert "Visi adresātu tipi".</span><span class="sxs-lookup"><span data-stu-id="149e9-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="149e9-110">Izveidojiet atvēlētu pastkasti, lai tvertu e-pasta ziņojumus, piemēram, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="149e9-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="149e9-111">Konkrētam domēnam iestatiet DomainType vērtību "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="149e9-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="149e9-112">Ja vēlāk noņemsit visu lomu, iestatiet domēnu atpakaļ uz Autoritatīvs.</span><span class="sxs-lookup"><span data-stu-id="149e9-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="149e9-113">Izveidojiet pasta plūsmas transporta kārtulu, kā norādīts tālāk.</span><span class="sxs-lookup"><span data-stu-id="149e9-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="149e9-114">Ja sūtītājs ir ārpus organizācijas</span><span class="sxs-lookup"><span data-stu-id="149e9-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="149e9-115">Novirzīt ziņojumu uz Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="149e9-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="149e9-116">Izņemot to, ka adresāts ir grupas allusers@domain.com (Adresātu grupā ir visi dalībnieki)</span><span class="sxs-lookup"><span data-stu-id="149e9-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="149e9-117">Kā pārliecināties, vai jaunās pastkastes tiek pievienotas dinamisko adresātu grupai</span><span class="sxs-lookup"><span data-stu-id="149e9-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
