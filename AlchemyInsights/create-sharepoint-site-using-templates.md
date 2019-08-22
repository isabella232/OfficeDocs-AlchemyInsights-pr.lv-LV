---
title: Izveidot vietni, SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 7c24a0cf3bcae0f2780c1cb33c911cb38c1ca5cb
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515005"
---
# <a name="create-sharepoint-sites-using-templates"></a>Izveidojiet SharePoint vietnes, izmantojot veidnes

SharePoint vietņu veidnes ir iebūvētām definīcijas, kas paredzēta ap konkrētu biznesa vajadzību. Plašāku informāciju skatiet [izmantojot veidnes, lai radītu dažādu veidu SharePoint vietnēs](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Šeit ir dažas kopējas problēmas/risinājumi attiecībā uz saglabāšanas vietu vai sarakstu kā veidni Sharepoint Online. 

**Saglabāt sarakstā un vietnes veidnes poga nav pieejama vai trūkst**

Administratoriem būs nepieciešams pielāgots skripts ļauj iespējot veidnes līdzekļi. Detalizēts darbības piemērus un apsvērumi skatiet 

- [Atļautu vai aizliegtu pielāgots skripts](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Saglabāt vietni kā veidni komanda netiek atbalstīta, un var radīt problēmas uz vietām, kas izmanto SharePoint Server publicēšanas infrastruktūru.

**Vietnes veidne nevar izveidot vai nedarbojas pareizi**

Veidni var trūkt [līdzekli](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) un nevar aktivizēt. Ja šī funkcija nav pieejama, lai aktivizētu vietņu kolekcijā, vietnes veidne nevar izmantot, lai izveidotu vietni.

- Pārbaudiet, lai redzētu, ja nevienu sarakstu vai bibliotēku pārsniegt 5000 vienumus [Saraksta skats ierobežojuma slieksni](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , jo tas var bloķēt vietnes veidnes izveide.

- Vietne, iespējams, izmanto pārāk daudz resursu un tādēļ vietņu veidņu pārsniedz 50 MB.


- Pastāv problēmas attēlot datus no saraksta, kas izmanto uzmeklēšanas kolonnu. Papildinformāciju skatiet sadaļā [veidnes ģenerēts saraksts neparādās dati no SharePoint Online pareizo meklēšanas sarakstā](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).

Sīkāka informācija par kopīgu problēmu un risinājumu, lūdzu, pārbaudiet [vietnes veidņu izveidošana un izmantošana](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



