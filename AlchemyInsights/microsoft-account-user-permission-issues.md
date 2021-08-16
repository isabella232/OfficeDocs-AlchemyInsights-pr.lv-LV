---
title: Problēmu novēršana — lietotājs direktorijā nav atrasts
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098177"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Problēmu novēršana — lietotājs direktorijā nav atrasts

Ja lietotāji direktorijā saņem kļūdas ziņojumu "nevar atrast lietotāju", mēģiniet vēlreiz, kur problēmas tips ir Lietotājs nav direktorijā.

Lai novērstu problēmu, varat veikt tālāk norādītās darbības.

- Pārliecinieties, vai kontam, kas akceptējis uzaicinājumu pa e-pastu, ir tas pats konts, kas tiek izmantots, lai pierakstītos vēlāk. Pārliecinieties, vai lietotājs izmanto to pašu kontu, lai pieņemtu uzaicinājumu un pierakstītos vietnē. 

Papildinformāciju skatiet rakstā [Kā pārvaldīt aizstājvārdu savam Microsoft kontam, </a> lai pārvaldītu Microsoft 365 pieteikšanos.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Pārlūkojiet līdz katrai(-ām) vietnei(-ām), kurā lietotājs saņem kļūdu. 

Vietnes vietrāža URL beigās pievienojiet "/_layouts/15/people.aspx/membershipgroupid=0" (dubultpēdiņās). 

Piemērs: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Sarakstā atlasiet lietotāju.

- Lentē **noklikšķiniet uz** Noņemt lietotāja atļaujas. 
-  Pievienojiet lietotāju atpakaļ un atkārtoti nosūtīt uzaicinājumu lietotājam.

