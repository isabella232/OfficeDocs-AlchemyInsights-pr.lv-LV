---
title: Veicot darbvirsmas analīzes, radās kļūda, validējot piekļuves marķiera kļūdu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783558"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="596b3-102">Veicot darbvirsmas analīzes programmas versiju, radās kļūda, validējot piekļuves marķieri</span><span class="sxs-lookup"><span data-stu-id="596b3-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="596b3-103">Šī kļūda parasti tiek ievērota, kad beidzas autentifikācijas pilnvara.</span><span class="sxs-lookup"><span data-stu-id="596b3-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="596b3-104">Parasti, atsvaidzinot lapu, šī pilnvara tiek atsvaidzināta.</span><span class="sxs-lookup"><span data-stu-id="596b3-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="596b3-105">Tomēr šī problēma var turpināties, ja pastāv ierobežotas piekļuves politikas, kas attiecas uz kontu, kas tiek izmantots datora analīzes vajadzībām.</span><span class="sxs-lookup"><span data-stu-id="596b3-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="596b3-106">Azure portālā Azure AD pierakstīšanās žurnālu varat pārskatīt, lai noskaidrotu, vai pastāv kāda pierakstīšanās kļūmes kontam, kas tiek izmantots datora analīzes veikšanai.</span><span class="sxs-lookup"><span data-stu-id="596b3-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="596b3-107">Lai iegūtu papildinformāciju par ierobežotu piekļuvi, apmeklējiet vietni [ar nosacījuma piekļuves izvietošanas plānošanu](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="596b3-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>