---
title: Funkcija WORKDAY uz AD lietotāju nodrošināšanu nonāk karantīnas stāvoklī
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481878"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="97f2c-102">Funkcija WORKDAY uz AD lietotāju nodrošināšanu nonāk karantīnas stāvoklī</span><span class="sxs-lookup"><span data-stu-id="97f2c-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="97f2c-103">**Funkcija WORKDAY uz AD lietotāju nodrošināšanu tiek pārveidota par karantīnas stāvokli, bet REKLĀMā netiek izveidots neviens lietotājs**</span><span class="sxs-lookup"><span data-stu-id="97f2c-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="97f2c-104">Darba sākšana ar reklāmas lietotāju nodrošināšanas darbu ir izdevusies karantīnas stāvoklī, un audita žurnālos tiek rādīts kļūdas ziņojuma **kļūdas ziņojums: OperationsError-SvcErr: radās darbības kļūda. Nav konfigurēta neviena vadītāja atsauce direktoriju pakalpojumam. Direktoriju pakalpojums tāpēc nevar sniegt norādes objektiem ārpus šī meža**.</span><span class="sxs-lookup"><span data-stu-id="97f2c-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="97f2c-105">Šī kļūda parasti tiek rādīta, ja Active Directory konteiners OU nav iestatīts pareizi vai pastāv problēmas ar **ParentDistinguishedName** izteiksmju kartēšanu.</span><span class="sxs-lookup"><span data-stu-id="97f2c-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="97f2c-106">Pārbaudiet noklusējuma OU **jauniem lietotājiem** parametru typos.</span><span class="sxs-lookup"><span data-stu-id="97f2c-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="97f2c-107">Pārliecinieties, vai jūsu REKLĀMā jau ir norādīta norādītā OU.</span><span class="sxs-lookup"><span data-stu-id="97f2c-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="97f2c-108">Ja izmantojat **parentDistinguishedName** atribūtu kartē, pārliecinieties, vai tas vienmēr tiek novērtēts uz zināmo konteineru ad domēnā.</span><span class="sxs-lookup"><span data-stu-id="97f2c-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="97f2c-109">Pārbaudiet eksportēšanas notikumu audita žurnālos, lai redzētu ģenerēto vērtību.</span><span class="sxs-lookup"><span data-stu-id="97f2c-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="97f2c-110">Lai iegūtu papildinformāciju par to, kā konfigurēt darba dienu automatizētai konfigurēšanai, skatiet rakstu [apmācība: darbdienas konfigurēšana automātiskai lietotāju nodrošināšanai](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="97f2c-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

