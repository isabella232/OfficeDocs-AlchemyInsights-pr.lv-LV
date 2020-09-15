---
title: 182 Lūdzu, palaidiet SaRA, lai diagnosticētu un novērstu Outlook autentifikācijas problēmas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "182"
- "1800012"
ms.assetid: a3a5ea91-6989-4616-9290-c7b24484e8c8
ms.openlocfilehash: aa1e831eac829f3bd35f34e2fbe34923c5af0d3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47802028"
---
# <a name="use-sara-to-diagnose-and-resolve-outlook-authentication-issues"></a><span data-ttu-id="d257d-102">SaRA izmantošana Outlook autentifikācijas problēmu diagnostikai un novēršanai</span><span class="sxs-lookup"><span data-stu-id="d257d-102">Use SaRA to diagnose and resolve Outlook authentication issues</span></span>

<span data-ttu-id="d257d-103">**Piezīme**. Lūdzu, pārbaudiet, vai jūsu organizācijai ir iespējoti [drošības noklusējumi](https://aka.ms/securitydefaults) .</span><span class="sxs-lookup"><span data-stu-id="d257d-103">**Note**: Please check to see whether [security defaults](https://aka.ms/securitydefaults) is enabled for your organization.</span></span> <span data-ttu-id="d257d-104">Ja jūsu nomnieks ir izveidots pēc 21. oktobra, 2019 un jūsu Outlook atkārtoti lūdz norādīt paroli, iespējams, jūsu nomniekā ir iespējoti **drošības noklusējumi** .</span><span class="sxs-lookup"><span data-stu-id="d257d-104">If your tenant was created after October 21st, 2019 and your Outlook is repeatedly asking you for a password, you may have **security defaults** enabled in your tenant.</span></span>

<span data-ttu-id="d257d-105">Mēs ļoti iesakām izmantot [Outlook joprojām lūdz manu paroļu](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) diagnostiku attiecīgajā datorā, lai novērstu problēmas, kad Outlook nepārtraukti lūdz paroli.</span><span class="sxs-lookup"><span data-stu-id="d257d-105">We highly recommend you use the [Outlook keeps asking for my password](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) diagnostic on the affected machine to troubleshoot issues where Outlook continually prompts for a password.</span></span> <span data-ttu-id="d257d-106">Šī [SaRA](https://diagnostics.office.com/#/) diagnostikas veic automatizētās pārbaudes un atgriež iespējamos risinājumus, ko varat izmantot, lai novērstu visas konstatētās problēmas.</span><span class="sxs-lookup"><span data-stu-id="d257d-106">This [SaRA](https://diagnostics.office.com/#/) diagnostic does automated checks and returns possible solutions for you to use to address any detected issues.</span></span>
