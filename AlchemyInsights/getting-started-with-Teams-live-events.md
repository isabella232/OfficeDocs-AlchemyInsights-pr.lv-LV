---
title: Darba sākšana ar Teams tiešraides pasākumiem
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
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811967"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="084dc-102">Darba sākšana ar Teams tiešraides pasākumiem</span><span class="sxs-lookup"><span data-stu-id="084dc-102">Getting started with Teams live events</span></span>

<span data-ttu-id="084dc-103">Microsoft Teams tiešraides pasākumi ir Teams sapulču paplašinājums, kas ļauj plānot un izveidot pasākumus, kas tiek pārraidīti lielām tiešsaistes auditorijām.</span><span class="sxs-lookup"><span data-stu-id="084dc-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="084dc-104">Lai izveidotu tiešraides pasākumu, jums būs nepieciešams tālāk norādītās lietas:</span><span class="sxs-lookup"><span data-stu-id="084dc-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="084dc-105">Vispirms pārliecinieties, vai Teams tiešraides pasākumi ir [pieejami jūsu valstī un reģionā,](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); tiešraides pasākumi dažās valstīs vēl netiek atbalstīti.</span><span class="sxs-lookup"><span data-stu-id="084dc-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="084dc-106">Ja esat piešķīris licences un iestatījis politikas, bet joprojām nevarat izveidot Teams tiešraides pasākumu, visticamāk, ka atrodaties valstī vai reģionā, kur tiešraides pasākumi vēl nav pieejami.</span><span class="sxs-lookup"><span data-stu-id="084dc-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="084dc-107">[Office 365 Enterprise E1, E3 vai E5 licence, vai Office 365 a3 vai A5 licences](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="084dc-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="084dc-108">**Piezīme**. Nesenā Teams lietojuma palielināšanās dēļ, kad piešķirat Teams licenci lietotājam, var paiet 24 stundas, pirms lietotājs tiks pilnībā iestatīts.</span><span class="sxs-lookup"><span data-stu-id="084dc-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="084dc-109">Līdz tam jūs nevarēsiet piešķirt Teams politikas, un viņiem, iespējams, nebūs piekļuves dažiem Teams līdzekļiem, piemēram, zvanīšanai un audiokonferencēm.</span><span class="sxs-lookup"><span data-stu-id="084dc-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="084dc-110">Atļauja [izveidot tiešraides pasākumus Microsoft Teams administrēšanas centrā](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="084dc-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="084dc-111">Atļauja [izveidot tiešraides pasākumus pakalpojumā Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (pasākumiem, kas veidoti, izmantojot ārēju apraides programmu vai ierīci).</span><span class="sxs-lookup"><span data-stu-id="084dc-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="084dc-112">Pilna darba grupas dalība organizācijā (nevarat būt viesis vai no citas organizācijas).</span><span class="sxs-lookup"><span data-stu-id="084dc-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="084dc-113">Privāta sapulču plānošana, ekrāna koplietošana un IP video koplietošana ieslēgta sadaļā Teams sapulces politika.</span><span class="sxs-lookup"><span data-stu-id="084dc-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="084dc-114">Teams tiešraides pasākumu lietošanas[Paraugprakse](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42).</span><span class="sxs-lookup"><span data-stu-id="084dc-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="084dc-115">Lai iegūtu papildinformāciju, lūdzu, skatiet rakstu [Darba sākšana ar Microsoft Teams tiešraides pasākumiem](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="084dc-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>