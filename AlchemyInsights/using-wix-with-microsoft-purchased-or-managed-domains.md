---
title: Wix tīmekļa vietnes izmantošana kopā ar Microsoft iegādātajiem vai pārvaldītajiem domēniem
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: f6845c56f05e9cef11362ce601a974b73a154c9a
ms.sourcegitcommit: 28a319e482e6a8644e87726e1b0e599819df52d0
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2020
ms.locfileid: "46629668"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a><span data-ttu-id="c743e-102">Wix tīmekļa vietnes izmantošana kopā ar Microsoft iegādātajiem vai pārvaldītajiem domēniem</span><span class="sxs-lookup"><span data-stu-id="c743e-102">Using a Wix website with Microsoft purchased or managed domains</span></span>

<span data-ttu-id="c743e-103">Informāciju par to, kā izmantot Wix tīmekļa vietni ar Microsoft iegādātos vai pārvaldītu domēnu, skatiet rakstā [DNS ierakstu atjaunināšana, lai savu tīmekļa vietni uzturētu ar pašreizējo viesošanas pakalpojumu sniedzēju](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="c743e-103">For information about how to use a Wix website with a Microsoft purchased or managed domain, see [Update DNS records to keep your website with your current hosting provider](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span></span>

<span data-ttu-id="c743e-104">Detalizētu informāciju skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="c743e-104">For details, see:</span></span> 

- <span data-ttu-id="c743e-105">Wix rakstā "domēna savienošana ar Wix, izmantojot norādes metodi" iesaka pievienot DNS ierakstus, kā norādīts iepriekš norādītajā saitē, nevis mainīt nosaukumu serverus, ja izmantojat Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c743e-105">The Wix article, "Connecting a Domain to Wix Using the Pointing Method," recommends adding DNS records as outlined in the link above rather than changing names servers when you're using Microsoft 365.</span></span>

- <span data-ttu-id="c743e-106">Ja izvēlējāties mainīt nosaukumu serverus uz Wix, ir jāizveido DNS ieraksti vietnē Wix darbam ar Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c743e-106">If you choose to change name servers to Wix, you must create DNS records at Wix for Microsoft.</span></span> <span data-ttu-id="c743e-107">Papildinformāciju skatiet rakstā [DNS ierakstu izveide vietnē Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span><span class="sxs-lookup"><span data-stu-id="c743e-107">For more info, see [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span></span>

- <span data-ttu-id="c743e-108">Ja jūsu domēnu iegādājāties no Microsoft, nosaukumu serverus nevar mainīt.</span><span class="sxs-lookup"><span data-stu-id="c743e-108">If your domain was purchased from Microsoft the name servers can't be changed.</span></span> <span data-ttu-id="c743e-109">Ja ir jāmaina nosaukumu serveri, Microsoft iegādātais domēns ir jāpārsūta uz citu viesošanas pakalpojumu sniedzēju pēc 60 dienām.</span><span class="sxs-lookup"><span data-stu-id="c743e-109">If you must change names servers, the Microsoft purchased domain must be transferred to another hosting provider after 60 days.</span></span> <span data-ttu-id="c743e-110">Papildinformāciju skatiet rakstā [bieži uzdotie jautājumi par domēniem](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span><span class="sxs-lookup"><span data-stu-id="c743e-110">For more info, see the [Domains FAQ](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span></span>