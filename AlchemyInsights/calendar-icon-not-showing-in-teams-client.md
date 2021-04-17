---
title: Kalendāra ikona netiek rādīta Teams klientā
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
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819960"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="68d73-102">Kalendāra ikona netiek rādīta Teams klientā</span><span class="sxs-lookup"><span data-stu-id="68d73-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="68d73-103">Cilnei Kalendārs pakalpojumā Teams ir nepieciešama piekļuve Exchange pastkastei, izmantojot Exchange tīmekļa pakalpojumus.</span><span class="sxs-lookup"><span data-stu-id="68d73-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="68d73-104">Exchange pastkaste var būt tiešsaistē vai lokāli.</span><span class="sxs-lookup"><span data-stu-id="68d73-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="68d73-105">Tiešsaistes lietotājiem, kuri neredz cilni Kalendārs, jāpārliecinās, vai viņiem [ir Exchange Online pastkastes licence un vai pastkaste ir iespējota](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="68d73-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="68d73-106">Ja lietotājam ir derīga pastkaste pakalpojumā Exchange Online, bet viņš joprojām neredz cilni Kalendārs, iespējams, radušās tīkla problēmas.</span><span class="sxs-lookup"><span data-stu-id="68d73-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="68d73-107">Izmantojiet [Microsoft attālās savienojamības analizētāju](https://testconnectivity.microsoft.com/) un palaidiet ietekmētajam lietotājam paredzētās **Microsoft Exchange tīmekļa pakalpojumu savienojamības pārbaudes**.</span><span class="sxs-lookup"><span data-stu-id="68d73-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="68d73-108">Visbeidzot pārbaudiet [Teams programmas — programmu iestatīšanas politikas](https://admin.teams.microsoft.com/policies/app-setup), lai nodrošinātu, ka programma Kalendārs nav noņemta no lietotājam piemērotās politikas (visdrīzāk **Globālā (organizācijas līmeņa noklusējums)**).</span><span class="sxs-lookup"><span data-stu-id="68d73-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="68d73-109">Ja jūsu lietotāji izmanto lokālo versiju, jums jāpārliecinās, vai hibrīdā konfigurācija ir darbspējīga.</span><span class="sxs-lookup"><span data-stu-id="68d73-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="68d73-110">Izmantojiet [hibrīdās konfigurācijas vedni](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent), lai novērstu problēmas.</span><span class="sxs-lookup"><span data-stu-id="68d73-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="68d73-111">Ņemiet vērā, ka [pakalpojumam Teams nepieciešams Exchange 2016 CU3 vai jaunāka tā versija](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="68d73-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
