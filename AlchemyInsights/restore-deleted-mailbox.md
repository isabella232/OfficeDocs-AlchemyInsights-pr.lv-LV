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
ms.openlocfilehash: 899eb7e171d125c509871c219f99dfd1106b858a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728078"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="23d2b-102">Izdzēstas pastkastes atjaunošana</span><span class="sxs-lookup"><span data-stu-id="23d2b-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="23d2b-103">Kad lietotājs zaudē Exchange Online licenci, to pastkaste tiek saglabāta 30 dienas, un to var atkopt, vienkārši atkārtoti piešķirot licenci lietotājam.</span><span class="sxs-lookup"><span data-stu-id="23d2b-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="23d2b-104">*Tas darbosies tikai 30 dienu laikā.*</span><span class="sxs-lookup"><span data-stu-id="23d2b-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="23d2b-105">Microsoft 365 administrēšanas centrā dodieties uz lapu **lietotāji** \> **Aktīvie lietotāji** .</span><span class="sxs-lookup"><span data-stu-id="23d2b-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="23d2b-106">Atlasiet attiecīgo lietotāju.</span><span class="sxs-lookup"><span data-stu-id="23d2b-106">Select the user in question.</span></span>

2. <span data-ttu-id="23d2b-107">Cilnē **licences un lietojumprogrammas** piešķiriet Exchange Online licenci un atlasiet **Saglabāt izmaiņas**.</span><span class="sxs-lookup"><span data-stu-id="23d2b-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="23d2b-108">Ja mēģināt atkopt koplietotu pastkasti, tā ir atkopjama arī 30 dienu laikā.</span><span class="sxs-lookup"><span data-stu-id="23d2b-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="23d2b-109">Tās var atrast sadaļā **lietotāji** \> **Izdzēstie lietotāji**; koplietojamām pastkastēm nav nepieciešama licence.</span><span class="sxs-lookup"><span data-stu-id="23d2b-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="23d2b-110">Ja konstatējat, ka ir jāatjauno izdzēsts lietotājs, skatiet rakstu [lietotāja atjaunošana](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="23d2b-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
  