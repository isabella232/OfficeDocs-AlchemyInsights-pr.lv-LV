---
title: Problēma ar vienu lietotāju
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430199"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="57dfa-102">Problēma ar vienu lietotāju</span><span class="sxs-lookup"><span data-stu-id="57dfa-102">Problem with single user</span></span>

- <span data-ttu-id="57dfa-103">Lietotājs, iespējams, nav nodrošināts, jo pakalpojums vēl nav bijis izdevies novērtēt lietotāju.</span><span class="sxs-lookup"><span data-stu-id="57dfa-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="57dfa-104">Pārskatiet norādījumus par to, kā ilgtermiņā tiek nodrošināts, kā arī norises josla lapā nodrošināšanas konfigurācija.</span><span class="sxs-lookup"><span data-stu-id="57dfa-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="57dfa-105">Ja sadaļā Papildu dati norādītā stabilā stāvokļa vērtība ir pirms lietotāja izveides/atjaunināšanas/dzēšanas, tas nozīmē, ka vēl neesat izvērtējis lietotāju.</span><span class="sxs-lookup"><span data-stu-id="57dfa-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="57dfa-106">Šajā scenārijā vislabākā darbība ir gaidīt, līdz tiek pabeigts nodrošināšanas pakalpojums.</span><span class="sxs-lookup"><span data-stu-id="57dfa-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="57dfa-107">Ņemiet vērā, ka mūsu pakalpojumi ir tikai informēti par izmaiņām lietotāja avota sistēmā (mākoņa stundā).</span><span class="sxs-lookup"><span data-stu-id="57dfa-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="57dfa-108">Azure AD avota sistēmā ir jābūt derīgām izmaiņām, lai noteiktu izmaiņas un to ieplūstošu Active Directory.</span><span class="sxs-lookup"><span data-stu-id="57dfa-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="57dfa-109">Nodrošināšanas pakalpojums novērtēja lietotāju un noteica, ka tas nav nodrošināts:</span><span class="sxs-lookup"><span data-stu-id="57dfa-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="57dfa-110">Ja esat iestatījis atribūtu, kura pamatā ir tvērums, pārliecinieties, vai lietotājs atbilst norādītajiem kritērijiem.</span><span class="sxs-lookup"><span data-stu-id="57dfa-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="57dfa-111">Ja lietotāji jau ir mērķa sistēmā un lietotāja stāvoklis avota un mērķa atbilstībā, mēs neveicam nekādas papildu darbības.</span><span class="sxs-lookup"><span data-stu-id="57dfa-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="57dfa-112">Nodrošināšanas pakalpojums mēģināja nodrošināt lietotāju un tas neizdevās.</span><span class="sxs-lookup"><span data-stu-id="57dfa-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="57dfa-113">Šos scenārijus skatiet nodrošināšanas žurnālu cilne problēmu novēršana un ieteikumi.</span><span class="sxs-lookup"><span data-stu-id="57dfa-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="57dfa-114">Lokālā Active Directory vai Azure AD, iespējams, trūkst nepieciešama lietotāja atribūta.</span><span class="sxs-lookup"><span data-stu-id="57dfa-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="57dfa-115">Piemēram, userPrincipalName vai sAMAccountName ģenerēšanas kārtulas nerada pareizo vērtību.</span><span class="sxs-lookup"><span data-stu-id="57dfa-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="57dfa-116">Atbilstošais atribūts (parasti employeeId) nav atrisināts ar unikālu lietotāju lokālajā Active Directory vai Azure AD.</span><span class="sxs-lookup"><span data-stu-id="57dfa-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="57dfa-117">Piemēram, ir divi lietotāji ar vienu un to pašu employeeId AD un pakalpojums atgriež kļūdas kodu, kas norāda tā paša avota ieraksta dublikātus.</span><span class="sxs-lookup"><span data-stu-id="57dfa-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="57dfa-118">Lai pārskatītu viena lietotāja un grupu žurnālus, skatiet rakstu [nodrošināšanas žurnālu pārskatīšana, lai iegūtu problēmu ar konkrētu lietotāju](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="57dfa-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
