---
title: Problēmu risināšana Teams pierakstīšanās kļūda AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357877"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="5913f-102">Problēmu risināšana Teams pierakstīšanās kļūda AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="5913f-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="5913f-103">Pierakstoties Microsoft Teams, var tikt parādīts kļūdas ziņojums: **Atvainojiet, bet mums ir problēmas ar PIERAKSTĪŠANOS AADSTS9000411: pieprasījums nav pareizi formatēts. Tiek dublēts parametrs "login_hint".**</span><span class="sxs-lookup"><span data-stu-id="5913f-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="5913f-104">Lai risinātu šo problēmu, lūdzu, pārliecinieties, vai jūsu Microsoft Teams klienti tiek atjaunināti.</span><span class="sxs-lookup"><span data-stu-id="5913f-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="5913f-105">Papildinformāciju par klienta atjaunināšanu skatiet sadaļā [Microsoft Teams atjaunināšana](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="5913f-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="5913f-106">Ja nevarat atjaunināt savu klientu kādu iemeslu dēļ, atteikšanās klients būs skaidrs visvairāk kešatmiņā datus.</span><span class="sxs-lookup"><span data-stu-id="5913f-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="5913f-107">Tomēr, ja jums joprojām ir problēmas pēc atteikšanās/pieteikšanās, beidziet darbu ar komandām un, lūdzu, iztīriet klienta kešatmiņu, rīkojoties šādi:</span><span class="sxs-lookup"><span data-stu-id="5913f-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="5913f-108">Aizveriet Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5913f-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="5913f-109">Dodieties uz:%AppData%\microsoft\teams un izdzēsiet visus failus.</span><span class="sxs-lookup"><span data-stu-id="5913f-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="5913f-110">Atkārtoti atveriet Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5913f-110">Reopen Microsoft Teams.</span></span>
