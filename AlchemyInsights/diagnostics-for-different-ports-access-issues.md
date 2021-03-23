---
title: Dažādu portu piekļuves problēmu diagnostika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035780"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="99b11-102">Dažādu portu piekļuves problēmu diagnostika</span><span class="sxs-lookup"><span data-stu-id="99b11-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="99b11-103">Lai atrisinātu dažādas portu piekļuves problēmas, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="99b11-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="99b11-104">Apturēt/depiešķirt virtuālo mašīnu (VM) no portāla, restartējiet VM un testējiet vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="99b11-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="99b11-105">Pārbaudiet sava VM tīkla iestatījumus, lai noteiktu, vai jums ir tīkla drošības grupu (NSGs) bloķēšanas trafiks.</span><span class="sxs-lookup"><span data-stu-id="99b11-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="99b11-106">Varat arī izmantot [tīkla uzrauga IP plūsmas pārbaudes rīku](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) , lai meklētu NSGs bloķēšanas trafiku, User-Defined maršrutus (UDRs) atkārtoti maršrutējiet savu trafiku atpakaļ uz lokālo ("noklusējuma maršruts" 0.0.0.0/0) vai uz tīkla ierīci.</span><span class="sxs-lookup"><span data-stu-id="99b11-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="99b11-107">Ja pēc šo darbību veikšanas joprojām rodas problēmas, lūdzu, norādiet VM nosaukumu un TCP portu, no kura mēģināt nosūtīt e-pasta ziņojumu, lai saņemtu turpmāku diagnozi.</span><span class="sxs-lookup"><span data-stu-id="99b11-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="99b11-108">**Ieteiktie dokumenti**</span><span class="sxs-lookup"><span data-stu-id="99b11-108">**Recommended Documents**</span></span>

[<span data-ttu-id="99b11-109">Ierobežojumi un ieteikumi par izejošā e-pasta nosūtīšanu, salīdzinot ar portu 25</span><span class="sxs-lookup"><span data-stu-id="99b11-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)