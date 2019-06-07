---
title: Novērsiet DKIM uzstādīšanas kļūdas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765219"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="dbe14-102">Novērsiet DKIM uzstādīšanas kļūdas</span><span class="sxs-lookup"><span data-stu-id="dbe14-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="dbe14-103">Ja jums rodas problēmas, ļaujot DKIM pielāgoto domēnu, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="dbe14-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="dbe14-104">Visvairāk DKIM uzstādīšanas jautājumi ir saistīti ar nepareizu DNS ierakstus.</span><span class="sxs-lookup"><span data-stu-id="dbe14-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="dbe14-105">Pārbaudiet, vai pareizi noformēta DKIM CNAME ieraksts (**nav** TXT ierakstu).</span><span class="sxs-lookup"><span data-stu-id="dbe14-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="dbe14-106">Lai iegūtu papildinformāciju, skatiet šajā [tēmā](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="dbe14-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="dbe14-107">Pēc tam, kad esat izveidot vai atjaunināt DKIM DNS ierakstu DNS viesošanas pakalpojumu savam domēnam (parasti, domēnu reģistrators), pagaidiet izplatīt DNS ierakstus.</span><span class="sxs-lookup"><span data-stu-id="dbe14-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="dbe14-108">Ja jūs nevarat izveidot DKIM DNS ieraksti administrēšanas centrā, jūs varat nomainīt \<CustomDomain\> ar pielāgoto domēnu (piemēram, contoso.com) un palaist šo komandu [Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)PowerShell: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="dbe14-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
