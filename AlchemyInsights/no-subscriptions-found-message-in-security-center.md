---
title: Nav atrasts neviens abonements drošības centrā
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713958"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="bd38a-102">Nav atrasts neviens abonements drošības centrā</span><span class="sxs-lookup"><span data-stu-id="bd38a-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="bd38a-103">Ja, piekļūstot Microsoft Defender drošības centram, tiek parādīts ziņojums "bez abonementiem", tas nozīmē, ka Azure Active Directory (AAD), ko izmanto, lai pieteiktos lietotājam portālā, nav Microsoft Defender ATP licences.</span><span class="sxs-lookup"><span data-stu-id="bd38a-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="bd38a-104">Windows E5 un Office E5 licences ir atsevišķas licences.</span><span class="sxs-lookup"><span data-stu-id="bd38a-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="bd38a-105">Atveriet atbalsta gadījumu, ja licence ir iegādāta, bet netika nodrošināta šai AAD instancei.</span><span class="sxs-lookup"><span data-stu-id="bd38a-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="bd38a-106">Jums ir:</span><span class="sxs-lookup"><span data-stu-id="bd38a-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="bd38a-107">Iespējamu licenču nodrošināšanas problēmu.</span><span class="sxs-lookup"><span data-stu-id="bd38a-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="bd38a-108">Jūs nejauši esat licencējis licenci uz citu Microsoft AAD, nevis to, ko izmanto autentifikācijai pakalpojumā.</span><span class="sxs-lookup"><span data-stu-id="bd38a-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>