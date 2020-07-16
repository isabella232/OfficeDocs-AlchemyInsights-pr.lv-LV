---
title: Failu atvēršanas vai lejupielādes problēmu yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148333"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Failu atvēršanas vai lejupielādes problēmu yammer

Klasiskais Yammer atbalsta vairākas opcijas failu augšupielādei ziņojumos un grupās. Atkarībā no tīkla konfigurācijas faili pēc noklusējuma tiek lietoti krātuvē koplietošanas vidē SharePoint.

Failu izvēle jaunā Yammer vēl neatbalsta visas opcijas, kas pieejamas klasiskajā Yammer. Nākamajā atjauninājumā tiks pievienoti papildu līdzekļi. Papildinformāciju skatiet rakstā [Faila vai attēla pievienošana Yammer sarunas ziņai](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Nevar atvērt vai lejupielādēt failu**  

Fails var augšupielādēt Yammer, bet arī saites uz failu SharePoint Online. Lai novērstu problēmas, vispirms ir jānosaka faila atrašanās vieta. Ja fails ir augšupielādēts Yammer, tam būs *.yammer.com URL. Pārliecinieties, vai nepieciešamie vietrāži URL un IP adreses tiek atbloķēti. Lai iegūtu papildinformāciju, skatiet emuāra [ziņu Izmantojot grūti kodēta IP adreses Yammer nav ieteicams](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Pārbaudiet, vai lietotājs, kurš ir arī globālais administrators, var lejupielādēt failu. Ja fails ir privāts, iespējams, ir jāizmanto privātā satura režīms. Papildinformāciju skatiet rakstā Privātā [satura pārraudzība pakalpojumā Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Yammer tīkla līmeņa viesi un faili pakalpojumā SharePoint Online**  

[Tīkla līmeņa viesi Yammer neizmanto](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) Azure AD B2B un ir iekšējā Yammer pakalpojumu, lai viņi nevar piekļūt Yammer failus, kas saglabāti SharePoint. Izveidojiet ārēju AAD B2B lietotāju, kurš var piekļūt dokumentu bibliotēkām pakalpojumā SharePoint Online, izmantojot šo identitāti. Informāciju par turpmāko Azure AD B2B viesu atbalstu pakalpojumā Yammer skatiet rakstā [Biznesa-to-business (B2B) viesu atbalsts pakalpojumā Yammer Preview — klientu nosacījumi un bieži uzdotie jautājumi](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).