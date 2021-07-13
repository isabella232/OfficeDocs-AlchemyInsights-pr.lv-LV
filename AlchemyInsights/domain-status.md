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
ms.openlocfilehash: 66fae5b5602dd67954ac9208b26bc2005adda0e3
ms.sourcegitcommit: 56650eb9af437ff97e4f4d9ca5a2f53ad5bb990e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/12/2021
ms.locfileid: "53389188"
---
# <a name="domain-status---no-services-selected"></a>Domēna statuss — nav atlasīts neviens pakalpojums

**Neviens pakalpojums** nav atlasīts, tas nozīmē, ka neesat atlasījis nevienu Microsoft 365 pakalpojumu, piemēram, Exchange Online, Skype darbam vai Intune, kā arī mobilo ierīču pārvaldību ierīcei Microsoft 365 izmantošanai ar savu pielāgoto domēnu. Ja izmantojat Exchange hibrīdu (Exchange lokāli ar Exchange Online) vai ārēju surogātpasta filtrēšanu ar Exchange un nevienu citu Microsoft pakalpojumi, varat ignorēt šo ziņojumu. Domēna darbspējas statuss ir pieejams tikai domēniem, kas ir savienoti tieši ar pakalpojumu.

Lai atlasītu pakalpojumus savam domēnam:

1. No **Iestatījumi**  >  [**domēni**](https://admin.microsoft.com/Adminportal/Home)atzīmējiet izvēles rūtiņu blakus domēnam ar statusa ziņojumu **Nav atlasīts neviens pakalpojums.**
1. Atlasiet **Pārvaldīt DNS,** lai startētu domēna iestatīšanas vedni.
    - Ja **izvēlaties Pievienot savus DNS ierakstus**, noteikti atlasiet pakalpojumu, kad tas tiek piedāvāts. Papildu pakalpojumi var būt pieejami sadaļā **Papildu opcijas.**
    - Ja izvēlaties **Ļaut korporācijai Microsoft pievienot** jūsu DNS ierakstus vai Papildu opcijas Iestatīt manus tiešsaistes pakalpojumus, visi pieejamie pakalpojumi tiek ieteikti un   >   atlasīti automātiski.
1. Turpiniet ar vedņa starpniecību, lai pabeigtu DNS iestatīšanu un pakalpojumu izvēli.
 
Lai saņemtu papildu palīdzību saistībā ar domēna iestatīšanu, skatiet [rakstu DNS ierakstu pievienošana domēna pievienošanai.](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

