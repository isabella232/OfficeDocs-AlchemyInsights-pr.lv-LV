---
title: Izveidot e-pasta catch visu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286199"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="e248d-102">Izveidot e-pasta catch visu</span><span class="sxs-lookup"><span data-stu-id="e248d-102">Create an email catch all</span></span>

<span data-ttu-id="e248d-103">Visas nozvejas izmantošana tiek stingri kavēti.</span><span class="sxs-lookup"><span data-stu-id="e248d-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="e248d-104">Tas ir labāk, lai nodrošinātu piepeši atpakaļ sūtītājam izīrēšanas sūtītājiem zināt viņu ziņu nevar piegādāt kā adresēts, lai viņi varētu rīkoties.</span><span class="sxs-lookup"><span data-stu-id="e248d-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="e248d-105">Varat arī ierobežot pārraudzītas pastkastes tikai catch iepriekš derīgu e-pasta adreses.</span><span class="sxs-lookup"><span data-stu-id="e248d-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="e248d-106">Jebkurš nozvejas visas pastkastes saņems daudz surogātpasta un galu galā var aizpildīt, ja nav cieši jāuzrauga.</span><span class="sxs-lookup"><span data-stu-id="e248d-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="e248d-107">(Ir saņemšanas ierobežojumi.)</span><span class="sxs-lookup"><span data-stu-id="e248d-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="e248d-108">Ja nolemjat turpināt, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="e248d-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="e248d-109">Dinamiskās adresātu grupas izveide & iekļaut "visi adresātu tipi".</span><span class="sxs-lookup"><span data-stu-id="e248d-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="e248d-110">Izveidojiet speciālu pastkasti, lai noķertu e-pastus, piemēram, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="e248d-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="e248d-111">Konkrētu domēna, iestatiet DomainType "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="e248d-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="e248d-112">Ja jūs vēlāk izņemt nozvejas visiem, pārliecinieties, lai uzstādītu domēna atpakaļ autoritatīvu.</span><span class="sxs-lookup"><span data-stu-id="e248d-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="e248d-113">Izveidojiet šādu Mailflow transporta kārtulu:</span><span class="sxs-lookup"><span data-stu-id="e248d-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="e248d-114">Ja sūtītājs ir "ārpus organizācijas"</span><span class="sxs-lookup"><span data-stu-id="e248d-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="e248d-115">Novirzīt ziņojumu uz Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="e248d-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="e248d-116">Izņemot, ja saņēmējs ir biedrs allusers@domain.com (adresātu grupa ir visi dalībnieki)</span><span class="sxs-lookup"><span data-stu-id="e248d-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="e248d-117">Pārliecinieties, lai apstiprinātu, ka jaunās pastkastes tiek pievienotas dinamiskā adresātu grupa</span><span class="sxs-lookup"><span data-stu-id="e248d-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
