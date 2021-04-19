---
title: Teams pierakstīšanās kļūdas AADSTS9000411 adresēšana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821994"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="1a6a6-102">Teams pierakstīšanās kļūdas AADSTS9000411 adresēšana</span><span class="sxs-lookup"><span data-stu-id="1a6a6-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="1a6a6-103">Pierakstoties Microsoft Teams, iespējams, tiks parādīta kļūda: Diemžēl radās problēmas ar pierakstīšanos **AADSTS9000411: Pieprasījums nav pareizi formatēts. Parametra "login_hint" dublikāts.**</span><span class="sxs-lookup"><span data-stu-id="1a6a6-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="1a6a6-104">Lai novērstu šo problēmu, lūdzu, pārliecinieties, vai jūsu Microsoft Teams klienti tiek atjaunināti.</span><span class="sxs-lookup"><span data-stu-id="1a6a6-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="1a6a6-105">Papildinformāciju par klienta atjaunināšanu skatiet rakstā [Microsoft Teams atjaunināšana.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="1a6a6-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="1a6a6-106">Ja kāda iemesla dēļ nevarat atjaunināt savu klientu, piesakoties klientam, tiks notīrīta lielākā daļa kešoto datu.</span><span class="sxs-lookup"><span data-stu-id="1a6a6-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="1a6a6-107">Tomēr, ja problēmas joprojām pastāv pēc pieteikšanās/logotipa pievienošanas, aizveriet programmu Teams un, lūdzu, notīriet klienta kešatmiņu, rīkojoties šādi:</span><span class="sxs-lookup"><span data-stu-id="1a6a6-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="1a6a6-108">Aizveriet Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1a6a6-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="1a6a6-109">Dodieties uz: %appdata%\microsoft\teams un izdzēsiet visus failus.</span><span class="sxs-lookup"><span data-stu-id="1a6a6-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="1a6a6-110">Atkārtoti atveriet pakalpojumu Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1a6a6-110">Reopen Microsoft Teams.</span></span>
