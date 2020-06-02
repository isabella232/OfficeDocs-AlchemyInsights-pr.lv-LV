---
title: DKIM uzstādīšanas problēmu labošana
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506781"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="7e844-102">DKIM uzstādīšanas problēmu labošana</span><span class="sxs-lookup"><span data-stu-id="7e844-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="7e844-103">Ja rodas problēmas, iespējojot DKIM pielāgotu domēnu, veiciet šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="7e844-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="7e844-104">Lielākā daļa DKIM uzstādīšanas problēmas ir saistītas ar nepareizu DNS ierakstus.</span><span class="sxs-lookup"><span data-stu-id="7e844-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="7e844-105">Pārbaudiet DKIM CNAME ieraksts (**nav** txt ieraksts) ir formatēts pareizi.</span><span class="sxs-lookup"><span data-stu-id="7e844-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="7e844-106">Lai iegūtu papildinformāciju, skatiet šo [tēmu](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="7e844-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="7e844-107">Pēc tam, kad izveidojat vai atjaunināt DKIM DNS ierakstu DNS viesošanas pakalpojumu domēna (parasti domēna reģistrētājs), uzgaidiet, kamēr tiek izplatīts DNS ierakstus.</span><span class="sxs-lookup"><span data-stu-id="7e844-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="7e844-108">Ja nevarat izveidot DKIM DNS ierakstus administrēšanas centrs, varat aizstāt \<CustomDomain\> ar savu pielāgoto domēnu (piemēram, contoso.com) un palaist šo komandu [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="7e844-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
