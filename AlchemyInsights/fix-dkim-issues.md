---
title: DKIM iestatīšanas problēmu novēršana
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744957"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="5932a-102">DKIM iestatīšanas problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="5932a-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="5932a-103">Ja rodas problēmas, kas sniedz DKIM savam pielāgotajam domēnam, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="5932a-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="5932a-104">Lielākā daļa DKIM iestatīšanas problēmu attiecas uz nepareiziem DNS ierakstiem.</span><span class="sxs-lookup"><span data-stu-id="5932a-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="5932a-105">Pārbaudiet, vai DKIM CNAME ieraksts (**nevis** txt ieraksts) ir pareizi formatēts.</span><span class="sxs-lookup"><span data-stu-id="5932a-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="5932a-106">Papildinformāciju skatiet šajā [tēmā](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="5932a-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="5932a-107">Pēc tam, kad esat izveidojis vai atjauninājis savus DKIM DNS ierakstus sava domēna DNS viesošanas pakalpojumā (parasti jūsu domēnu reģistrētājs), uzgaidiet, līdz tiek izplatīti DNS ieraksti.</span><span class="sxs-lookup"><span data-stu-id="5932a-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="5932a-108">Ja nevarat izveidot DKIM DNS ierakstus administrēšanas centrā, varat aizstāt \<CustomDomain\> ar savu pielāgoto domēnu (piemēram, contoso.com) un izpildīt šo komandu pakalpojumā [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="5932a-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
