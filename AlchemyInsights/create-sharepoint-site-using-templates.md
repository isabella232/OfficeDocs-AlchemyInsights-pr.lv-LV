---
title: Vietnes izveide programmā SharePoint Online
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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057973"
---
# <a name="create-sharepoint-sites-using-templates"></a>Vietņu SharePoint, izmantojot veidnes

Modernās saziņas un darba grupas vietnēs iespēja saglabāt vietni kā veidni netiek atbalstīta. Papildinformāciju par vietņu veidņu izmantošanu skatiet rakstā [SharePoint vietnes saglabāšana, lejupielāde un augšupielāde veidnes veidā](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Tālāk ir uzskaitītas dažas bieži sastopamas problēmas/risinājumi saistībā ar vietnes vai saraksta saglabāšanu veidnes formātā lietojumprogrammā Sharepoint Online. 

**Poga Saglabāt vietnes/saraksta veidni nav pieejama vai nav pieejama**

Lai iespējotu veidņu līdzekļus, administratoriem būs jāiespējo opcija Atļaut pielāgotu skriptu. Detalizētus soļus, piemērus un apsvērumus skatiet sadaļā 

- [Pielāgota skripta atļaušana vai nepieļaušana](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Komanda Saglabāt vietni kā veidni netiek atbalstīta un var izraisīt problēmas vietnēs, kas izmanto SharePoint Server publicēšanas infrastruktūru.

**Vietnes veidni nevar izveidot vai tā nedarbojas pareizi**

Iespējams, veidnē trūkst [līdzekļa](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) un tā netiks aktivizēta. Ja līdzeklis nav pieejams aktivizēšanai pašreizējā vietņu kolekcijā, nevarat izmantot vietnes veidni, lai izveidotu vietni.

- Pārbaudiet, vai kāds saraksts vai bibliotēka nepārsniedz 5000 vienumu [saraksta skata ierobežojuma slieksni](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59), jo tas var neļaut izveidot vietnes veidni.

- Vietne, iespējams, izmanto pārāk daudz resursu, tāpēc vietnes veidne pārsniedz 50 MB ierobežojumu.


- Rādot datus no saraksta, kas izmanto uzmeklēšanas kolonnu, rodas problēmas. Papildinformāciju skatiet rakstā [Veidnes ģenerētajā sarakstā netiek rādīti dati no pareizā uzmeklēšanas saraksta pakalpojumā SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Lai iegūtu detalizētāku informāciju par bieži sastopamām problēmām un risinājumiem, lūdzu, [skatiet vietni veidņu izveide un izmantošana.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



