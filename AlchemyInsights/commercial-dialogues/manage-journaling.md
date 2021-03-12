---
title: Žurnālu pārvaldīšana
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745733"
---
# <a name="manage-journaling"></a><span data-ttu-id="134c5-102">Žurnālu pārvaldīšana</span><span class="sxs-lookup"><span data-stu-id="134c5-102">Manage journaling</span></span>

<span data-ttu-id="134c5-103">Journaling var palīdzēt organizācijai atsaukties uz juridiskajām, regulatīvajām un organizācijas prasībām, ierakstot ienākošo un izejošo e-pasta saziņu.</span><span class="sxs-lookup"><span data-stu-id="134c5-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="134c5-104">Atcerieties:</span><span class="sxs-lookup"><span data-stu-id="134c5-104">Keep in mind:</span></span>

* <span data-ttu-id="134c5-105">Lai varētu pārvaldīt journaling, ir nepieciešamas [organizācijas pārvaldības](https://go.microsoft.com/fwlink/?linkid=2115259) un [ierakstu pārvaldības](https://go.microsoft.com/fwlink/?linkid=2115469) atļaujas.</span><span class="sxs-lookup"><span data-stu-id="134c5-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="134c5-106">Jums ir jābūt instalētai žurnāla pastkastei un (pēc izvēles) konfigurētai alternatīvai žurnāla pastkastei.</span><span class="sxs-lookup"><span data-stu-id="134c5-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="134c5-107">Papildinformāciju skatiet rakstā [žurnāla konfigurēšana pakalpojumā Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span><span class="sxs-lookup"><span data-stu-id="134c5-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="134c5-108">Pakalpojumā Exchange Online ir ierobežots to žurnāla kārtulu skaits, kuras varat izveidot.</span><span class="sxs-lookup"><span data-stu-id="134c5-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="134c5-109">Detalizētu informāciju skatiet rakstā [žurnālu, transporta un iesūtnes kārtulu ierobežojumi](https://go.microsoft.com/fwlink/?linkid=2115261).</span><span class="sxs-lookup"><span data-stu-id="134c5-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="134c5-110">Exchange Online neatbalsta žurnāla atskaišu piegādi Exchange Online pastkastei.</span><span class="sxs-lookup"><span data-stu-id="134c5-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="134c5-111">Ir jānorāda lokālās arhivēšanas sistēmas vai trešo pušu arhivēšanas pakalpojuma e-pasta adrese kā journaling pastkaste.</span><span class="sxs-lookup"><span data-stu-id="134c5-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
