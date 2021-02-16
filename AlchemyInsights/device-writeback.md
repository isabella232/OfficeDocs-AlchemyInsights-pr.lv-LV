---
title: Ierīces arī atpakaļrakstīšanas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256854"
---
# <a name="device-writeback"></a><span data-ttu-id="d9299-102">Ierīces arī atpakaļrakstīšanas</span><span class="sxs-lookup"><span data-stu-id="d9299-102">Device Writeback</span></span>

<span data-ttu-id="d9299-103">Ierīces arī atpakaļrakstīšanas tiek izmantota šādos scenārijos:</span><span class="sxs-lookup"><span data-stu-id="d9299-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="d9299-104">[Windows Hello darbam iespējošana uzņēmumiem, izmantojot hibrīda sertifikāta uzticamības izvietošanu](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="d9299-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="d9299-105">Iespējot piekļuvi nosacījumam, pamatojoties uz ADFS (2012 R2 vai jaunākas versijas) aizsargātām lietojumprogrammām (paļaujoties uz pušu uzticamību)</span><span class="sxs-lookup"><span data-stu-id="d9299-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="d9299-106">Azure AD Premium abonements ir nepieciešams ierīču arī atpakaļrakstīšanas.</span><span class="sxs-lookup"><span data-stu-id="d9299-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="d9299-107">Tas nodrošina papildu drošību un pārliecību par to, ka piekļuve lietojumprogrammām tiek piešķirta tikai uzticamām ierīcēm.</span><span class="sxs-lookup"><span data-stu-id="d9299-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="d9299-108">Papildinformāciju par ierobežotu piekļuvi skatiet rakstā [riska pārvaldība ar ierobežotu piekļuvi](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) un lokālās piekļuves [iestatīšana, izmantojot Azure Active Directory ierīces reģistrāciju](https://docs.microsoft.com/azure/active-directory/devices/overview).</span><span class="sxs-lookup"><span data-stu-id="d9299-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="d9299-109">Papildinformāciju par ierīču arī atpakaļrakstīšanas ierīcēm skatiet rakstā ierīces [arī atpakaļrakstīšanas iespējošana](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span><span class="sxs-lookup"><span data-stu-id="d9299-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
