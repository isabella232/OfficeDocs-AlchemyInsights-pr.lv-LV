---
title: Izdzēstas pastkastes atjaunošana
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "360"
- "3500005"
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 14d2c9b1fe6764f5cd3a5a968586a19a03b62694
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641525"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="2952d-102">Izdzēstas pastkastes atjaunošana</span><span class="sxs-lookup"><span data-stu-id="2952d-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="2952d-103">Kad lietotājs zaudē Exchange Online licenci, to pastkaste tiek saglabāta 30 dienas, un to var atkopt, vienkārši atkārtoti piešķirot licenci lietotājam.</span><span class="sxs-lookup"><span data-stu-id="2952d-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
1. <span data-ttu-id="2952d-104">Microsoft 365 administrēšanas centrā dodieties uz lapu **lietotāji** \> **Aktīvie lietotāji** .</span><span class="sxs-lookup"><span data-stu-id="2952d-104">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="2952d-105">Atlasiet attiecīgo lietotāju.</span><span class="sxs-lookup"><span data-stu-id="2952d-105">Select the user in question.</span></span>

2. <span data-ttu-id="2952d-106">Cilnē **licences un lietojumprogrammas** piešķiriet Exchange Online licenci un atlasiet **Saglabāt izmaiņas**.</span><span class="sxs-lookup"><span data-stu-id="2952d-106">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="2952d-107">Ja mēģināt atkopt koplietotu pastkasti vai dzēstu lietotāju, tas ir arī atkopjams 30 dienu laikā.</span><span class="sxs-lookup"><span data-stu-id="2952d-107">If you are trying to recover a shared mailbox or a user that was deleted, it is also recoverable for 30 days.</span></span> <span data-ttu-id="2952d-108">Tās var atrast sadaļā **lietotāji** \> **Izdzēstie lietotāji**; koplietojamām pastkastēm nav nepieciešama licence.</span><span class="sxs-lookup"><span data-stu-id="2952d-108">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="2952d-109">Lūdzu, skatiet sadaļu [lietotāja atjaunošana](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="2952d-109">Please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="2952d-110">E-pasta atkopšanu no lietotāja pastkastes var veikt administratori, apmeklējot [jauno Exchange administrēšanas centru](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353).</span><span class="sxs-lookup"><span data-stu-id="2952d-110">Recovery of email from user's mailbox can be done by admins by going to the [new Exchange Admin Center](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353).</span></span>

<span data-ttu-id="2952d-111">Visbeidzot, ja mēģināt atkopt neaktīvu pastkasti, [izpildiet norādījumus, kas sniegti šeit](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox).</span><span class="sxs-lookup"><span data-stu-id="2952d-111">Finally, if you are trying to recover an Inactive mailbox, [follow the instructions here](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox).</span></span>
  
