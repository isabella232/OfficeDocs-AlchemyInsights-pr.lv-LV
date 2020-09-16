---
title: Vietnes vai saraksta saglabāšana veidnes formātā
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727538"
---
# <a name="save-site-or-list-as-a-template"></a>Vietnes vai saraksta saglabāšana veidnes formātā

SharePoint vietnes veidnes ir iepriekš izveidotas definīcijas, kas paredzētas noteiktai biznesa nepieciešamībai. Papildinformāciju skatiet rakstā [veidņu izmantošana, lai izveidotu dažādu veidu SharePoint vietnes](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Tālāk ir sniegtas dažas bieži sastopamas problēmas/risinājumi attiecībā uz vietnes vai saraksta saglabāšanu veidnes formātā pakalpojumā SharePoint Online.

**Poga saglabāt vietnes/saraksta veidni nav pieejama vai trūkst**. 

- Administratoriem ir jāatļauj pielāgot skriptu, lai iespējotu veidnes līdzekļus. Detalizētus norādījumus par piemēriem un apsvērumiem skatiet rakstā [pielāgota skripta atļaušana vai novēršana](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Komanda Saglabāt vietni kā veidni netiek atbalstīta, un tā var izraisīt problēmas vietnēs, kurās tiek izmantota SharePoint Server publicēšanas infrastruktūra.


**Vietnes veidni nevar izveidot vai tā nedarbojas pareizi**

- Veidnei, iespējams, trūkst [līdzekļa](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , un tā netiek aktivizēta. Ja šis līdzeklis nav pieejams aktivizēšanai pašreizējā vietņu kolekcijā, vietnes veidni nevar izmantot, lai izveidotu vietni.


- Pārbaudiet, vai kāds saraksts vai bibliotēka pārsniedz [saraksta skata ierobežojuma slieksni](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 vienumiem, jo tas var bloķēt vietnes veidnes izveidi.


- Vietne, iespējams, izmanto pārāk daudz resursu, tāpēc vietnes veidne pārsniedz 50 megabaitu (MB) ierobežojumu.


- Pastāv problēmas, kas rāda datus no saraksta, kas izmanto uzmeklēšanas kolonnu. Lai iegūtu papildinformāciju, skatiet rakstu [veidnes ģenerētie saraksti nerāda datus no pareiza uzmeklēšanas saraksta pakalpojumā SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Detalizētāku informāciju par biežāk sastopamajām problēmām un risinājumiem skatiet sadaļā [vietņu veidņu izveide un lietošana](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

