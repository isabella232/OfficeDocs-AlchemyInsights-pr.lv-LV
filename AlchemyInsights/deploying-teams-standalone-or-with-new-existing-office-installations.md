---
title: Grupu izvietošana kā savrupa vai ar jaunām vai esošām Office instalācijām
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806766"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Grupu izvietošana kā savrupa vai ar jaunām vai esošām Office instalācijām

Tagad Microsoft Teams ir iekļautas jauno Microsoft 365 programmu, Microsoft 365 programmu darbam un Office darbam ar Mac ***instalāciju*** ietvaros. Papildinformāciju skatiet rakstā [kad Microsoft Teams sāks iekļauties jaunās Office instalācijās?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Turklāt, sākot ar versiju 1906 pašreizējā kanālā, darba grupas tiks ***pievienotas esošām*** Microsoft 365 lietojumprogrammu darbam ar Enterprise (un Microsoft 365 programmām darbam) ierīcēs, kurās darbojas sistēma Windows, atjauninot esošo instalāciju uz jaunāko versiju. Lai iegūtu papildinformāciju, skatiet rakstu [kā par esošām Office instalācijām?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ja nevēlaties gaidīt šo izvēršanas plānu, varat izvietot grupas kā savrupi saviem lietotājiem, [izpildot šos norādījumus](https://docs.microsoft.com/MicrosoftTeams/msi-deployment),   vai varat likt lietotājiem instalēt komandas savā datorā  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Ja jūsu organizācija nav gatava komandu izvietošanai, mums ir darbības, ko varat veikt, lai ***izslēgtu darba grupas*** no [jaunām](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) vai [esošām](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office instalācijām. Ja vēlaties, lai grupas tiktu instalētas, bet nevēlaties, lai grupas tiktu sāktas automātiski pēc tam, kad tās ir instalētas, skatiet rakstu [Microsoft darba grupu automātiska startēšana pēc instalēšanas](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Lai ***atinstalētu komandas*** no ierīces, kurā darbojas operētājsistēma Windows, skatiet rakstu [Microsoft Teams atinstalēšana](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Lai iztīrītu Microsoft Teams no vairākiem Target datoriem vai lietotājiem, skatiet rakstu [Microsoft Teams izvietošanas tīrīšana](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ja izmantojat koplietojamus datorus, attālās darbvirsmas pakalpojumus (RDS) vai virtuālās darbvirsmas infrastruktūru (VDI), skatiet rakstu [koplietojama datora un VDI vidē ar Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ja izmantojat Office darbam ar Mac, skatiet rakstu [Microsoft Teams instalācijas Mac datorā](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Pēc tam, kad komandas ir instalētas, tās tiek [automātiski atjauninātas](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) ik pēc divām nedēļām, izmantojot jaunus līdzekļus un kvalitātes atjauninājumus. 