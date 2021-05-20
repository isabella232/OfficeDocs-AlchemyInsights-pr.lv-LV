---
title: Drošības centrā netiek atrasts ziņojums par to, ka abonementi nav atrasti
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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544115"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="08820-102">Drošības centrā netiek atrasts ziņojums par to, ka abonementi nav atrasti</span><span class="sxs-lookup"><span data-stu-id="08820-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="08820-103">Ja, piekļūstot Microsoft Defender drošības centrs tiek parādīts ziņojums "Nav atrasts neviens abonements", tas nozīmē, ka Azure Active Directory (AAD), kas tiek izmantots, lai pieteiktos portālā, nav Microsoft Defender ATP licence.</span><span class="sxs-lookup"><span data-stu-id="08820-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="08820-104">E5 Windows E5 Office E5 licences ir atsevišķas licences.</span><span class="sxs-lookup"><span data-stu-id="08820-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="08820-105">Atveriet atbalsta gadījumu, ja licence tika iegādāta, bet netiek nodrošināta šai AAD instancei.</span><span class="sxs-lookup"><span data-stu-id="08820-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="08820-106">Jums ir:</span><span class="sxs-lookup"><span data-stu-id="08820-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="08820-107">Iespējama licenču nodrošināšanas problēma.</span><span class="sxs-lookup"><span data-stu-id="08820-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="08820-108">Jūs nejauši nodrošināt licenci citā Microsoft AAD, nevis tam, kas tika izmantots autentifikācijai pakalpojumā.</span><span class="sxs-lookup"><span data-stu-id="08820-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>