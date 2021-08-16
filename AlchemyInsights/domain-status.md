---
title: Domēna statuss — nav atlasīts neviens pakalpojums
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 1476a88c7b974a9e6cfe443f6842df8cdc3d7073a73c0add7e6f183dd0528de1
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2021
ms.locfileid: "57874402"
---
# <a name="domain-status---no-services-selected"></a>Domēna statuss — nav atlasīts neviens pakalpojums

**Neviens pakalpojums nav** atlasīts, tas nozīmē, ka neesat atlasījis nevienu Microsoft 365, piemēram, Exchange Online, Skype darbam vai Intune, kā arī mobilo ierīču pārvaldību, ko izmantot Microsoft 365 izmantot ar savu pielāgoto domēnu. Ja izmantojat Exchange hibrīdu (Exchange lokāli ar Exchange Online) vai ārēju surogātpasta filtrēšanu ar Exchange un nevienu citu Microsoft pakalpojumi, varat ignorēt šo ziņojumu. Domēna darbspējas statuss ir pieejams tikai domēniem, kas ir savienoti tieši ar pakalpojumu.

Lai atlasītu pakalpojumus savam domēnam:

1. No **Iestatījumi**  >  [**domēnos**](https://admin.microsoft.com/Adminportal/Home)atzīmējiet izvēles rūtiņu blakus domēnam ar statusa ziņojumu **Nav atlasīts neviens pakalpojums.**
1. Atlasiet **Pārvaldīt DNS,** lai startētu domēna iestatīšanas vedni.
    - Ja **izvēlaties Pievienot savus DNS ierakstus**, noteikti atlasiet pakalpojumu, kad tas tiek piedāvāts. Papildu pakalpojumi var būt pieejami sadaļā **Papildu opcijas.**
    - Ja izvēlaties **Ļaut korporācijai Microsoft pievienot** jūsu DNS ierakstus vai Papildu opcijas Iestatīt manus tiešsaistes pakalpojumus, visi pieejamie pakalpojumi tiek ieteikti un   >   atlasīti automātiski.
1. Turpiniet ar vedņa starpniecību, lai pabeigtu DNS iestatīšanu un pakalpojumu izvēli.
 
Lai saņemtu papildu palīdzību saistībā ar domēna iestatīšanu, skatiet [rakstu DNS ierakstu pievienošana domēna pievienošanai.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

