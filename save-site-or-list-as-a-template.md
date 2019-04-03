---
title: Vietni vai sarakstu saglabātu kā veidni
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 56c52c73e752414d66785f175c3a0e2925ad41c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/02/2019
ms.locfileid: "31044011"
---
# <a name="save-site-or-list-as-a-template"></a>Vietni vai sarakstu saglabātu kā veidni

SharePoint vietņu veidnes ir iebūvētām definīcijas, kas paredzēta ap konkrētu biznesa vajadzību. Plašāku informāciju skatiet [izmantojot veidnes, lai radītu dažādu veidu SharePoint vietnēs](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Šeit ir dažas kopējas problēmas/risinājumi attiecībā uz saglabāšanas vietu vai sarakstu kā veidni SharePoint Online.

**Saglabāt sarakstā un vietnes veidnes poga ir nav pieejama vai tās trūkst**. 

- Administratoriem būs nepieciešams pielāgots skripts ļauj iespējot veidnes līdzekļi. Detalizētām darbībām, piemērus un apsvērumi sk [Atļaut vai aizliegt pielāgotu skriptu](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).


- Saglabāt vietni kā veidni komanda netiek atbalstīta, un var radīt problēmas uz vietām, kas izmanto SharePoint Server publicēšanas infrastruktūru.


**Vietnes veidne nevar izveidot vai nedarbojas pareizi**

- Veidni var trūkt [līdzekli](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) un nevar aktivizēt. Ja šī funkcija nav pieejama, lai aktivizētu vietņu kolekcijā, vietnes veidne nevar izmantot, lai izveidotu vietni.


- Pārbaudiet, lai redzētu, ja nevienu sarakstu vai bibliotēku pārsniegt 5000 vienumus [Saraksta skats ierobežojuma slieksni](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , jo tas var bloķēt vietnes veidnes izveide.


- Vietne, iespējams, izmanto pārāk daudz resursu un tādēļ vietņu veidņu pārsniedz 50 megabaitu (MB) robežu.


- Pastāv problēmas attēlot datus no saraksta, kas izmanto uzmeklēšanas kolonnu. Papildinformāciju skatiet sadaļā [veidnes ģenerēts saraksts neparādās dati no SharePoint Online pareizo meklēšanas sarakstā](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).


Sīkāka informācija par bieži sastopamām problēmām un risinājumiem, lūdzu atsauci, [vietņu veidņu izveidošana un izmantošana](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

