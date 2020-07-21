---
title: Konflikti ar SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198178"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="95744-102">Konflikti ar SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="95744-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="95744-103">Ja sinhronizācijas laikā saņemat kļūdas, piemēram, "Jūsu direktorijā pastāv sinhronizēts objekts ar to pašu ProxyAddress vai UserPrincipalName", skatiet sadaļu [Atribūtu sinhronizācijas dublikātu problēmu diagnosticēšana un labošana](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="95744-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="95744-104">Apsveriet arī iespēju iespējot dublikātu atribūtu elastību.</span><span class="sxs-lookup"><span data-stu-id="95744-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="95744-105">Papildinformāciju skatiet sadaļā [Identitātes sinhronizācija un atribūtu atspējošana.](https://aka.ms/duplicateattributeresiliency)</span><span class="sxs-lookup"><span data-stu-id="95744-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>