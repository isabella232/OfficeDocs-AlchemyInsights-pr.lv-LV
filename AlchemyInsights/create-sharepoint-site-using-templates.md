---
title: Vietnes izveide pakalpojumā SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732238"
---
# <a name="create-sharepoint-sites-using-templates"></a>SharePoint vietņu izveide, izmantojot veidnes

Iespēja saglabāt vietni kā veidni netiek atbalstīta modernās saziņas vai grupas vietnēs. Papildinformāciju par veidņu izmantošanu skatiet rakstā [SharePoint vietnes saglabāšana, lejupielāde un augšupielāde veidnes](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)formātā.

Tālāk ir sniegtas dažas bieži sastopamas problēmas/risinājumi attiecībā uz vietnes vai saraksta saglabāšanu veidnes formātā pakalpojumā SharePoint Online. 

**Poga saglabāt vietnes/saraksta veidni nav pieejama vai trūkst**

Administratoriem ir jāatļauj pielāgot skriptu, lai iespējotu veidnes līdzekļus. Detalizētus norādījumus par piemēriem un apsvērumiem skatiet rakstā 

- [Pielāgota skripta atļaušana vai aizliegšana](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Komanda Saglabāt vietni kā veidni netiek atbalstīta, un tā var izraisīt problēmas vietnēs, kurās tiek izmantota SharePoint Server publicēšanas infrastruktūra.

**Vietnes veidni nevar izveidot vai tā nedarbojas pareizi**

Veidnei, iespējams, trūkst [līdzekļa](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , un tā netiek aktivizēta. Ja šis līdzeklis nav pieejams aktivizēšanai pašreizējā vietņu kolekcijā, vietnes veidni nevar izmantot, lai izveidotu vietni.

- Pārbaudiet, vai kāds saraksts vai bibliotēka pārsniedz [saraksta skata ierobežojuma slieksni](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 vienumiem, jo tas var bloķēt vietnes veidnes izveidi.

- Vietne, iespējams, izmanto pārāk daudz resursu, tāpēc vietnes veidne pārsniedz 50 MB ierobežojumu.


- Pastāv problēmas, kas rāda datus no saraksta, kas izmanto uzmeklēšanas kolonnu. Lai iegūtu papildinformāciju, skatiet rakstu [veidnes ģenerētie saraksti nerāda datus no pareiza uzmeklēšanas saraksta pakalpojumā SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Lai iegūtu detalizētāku informāciju par biežāk sastopamajām problēmām un risinājumiem, skatiet [lapu veidņu izveide un lietošana](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



