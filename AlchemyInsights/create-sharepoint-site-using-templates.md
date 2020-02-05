---
title: Izveidot vietni SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770430"
---
# <a name="create-sharepoint-sites-using-templates"></a>SharePoint vietņu izveide, izmantojot veidnes

Iespēja saglabāt vietni kā veidni netiek atbalstīta mūsdienu saziņas vai grupas vietnēs. Lai iegūtu papildinformāciju par veidņu lietošanu, skatiet sadaļu [SharePoint vietnes kā veidnes saglabāšana, lejupielāde un augšupielāde](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Tālāk ir norādītas dažas bieži sastopamas problēmas/risinājumi attiecībā uz vietnes vai saraksta saglabāšanu kā veidni programmā SharePoint Online. 

**Poga saglabāt vietnes/saraksta veidni nav pieejama vai tās trūkst**

Administratoriem ir jāatļauj pielāgots skripts, lai iespējotu veidnes līdzekļus. Detalizētus soļus, piemērus un apsvērumus sk. 

- [Atļaut vai aizliegt pielāgotu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Saglabāt vietni kā veidni komanda netiek atbalstīta un var radīt problēmas vietnēs, kas izmanto SharePoint Server publicēšanas infrastruktūra.

**Vietnes veidni nevar izveidot vai tā nedarbojas pareizi**

Iespējams, ka veidnei trūkst [līdzekļa](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , un tā netiks aktivizēta. Ja līdzeklis nav pieejams, lai aktivizētu pašreizējā vietņu kolekcijā, vietnes veidni nevar izmantot, lai izveidotu vietni.

- Pārbaudiet, vai kādi saraksti vai bibliotēkas pārsniedz [saraksta skata ierobežojuma slieksnis](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 vienumus, jo tas var bloķēt vietnes veidnes izveide.

- Vietne var izmantot pārāk daudz resursu un tādēļ vietnes veidne pārsniedz 50 MB ierobežojumu.


- Ir problēmas, parādot datus no saraksta, kas izmanto uzmeklēšanas kolonnu. Lai iegūtu papildinformāciju, skatiet [veidne ģenerēts saraksts netiek parādīts datus no pareizā uzmeklēšanas saraksta SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Sīkāku informāciju par kopīgām problēmām un risinājumiem, lūdzu, pārbaudiet [izveidot un izmantot vietnes veidnes](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



