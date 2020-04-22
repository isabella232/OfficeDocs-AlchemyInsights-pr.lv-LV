---
title: Izvietojot darba grupas kā savrupas vai ar jaunām vai esošām biroja instalācijām
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 4b843407f05db207f3b676c03c7088d3d0ba062e
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704640"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Izvietojot darba grupas kā savrupas vai ar jaunām vai esošām biroja instalācijām

Microsoft Teams tagad ir iekļauta kā daļa no ***jaunajām instalācijām*** Microsoft 365 Apps uzņēmumiem, Microsoft 365 Apps uzņēmumiem un Office Mac. Lai iegūtu papildinformāciju, skatiet [kad Microsoft Teams sāks iekļaut jaunas Office instalācijas?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Turklāt, sākot ar versiju 1906 ikmēneša kanālā, komandas tiks ***pievienotas esošajām instalācijām*** Microsoft 365 lietojumprogrammām uzņēmumiem (un Microsoft 365 lietojumprogrammām uzņēmumiem) ierīcēs, kurās darbojas sistēma Windows, atjauninot esošo instalāciju uz jaunāko versiju. Papildinformāciju skatiet sadaļā kas ir [par esošajām Office instalācijām?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Ja nevēlaties gaidīt šo izvēršanas grafiku, varat izvietot darba grupas kā savrupas lietotājiem, [izpildot šos norādījumus](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) , vai varat izmantot savus lietotājus, lai paši instalētu grupas [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Ja jūsu organizācija nav gatava izvietot darba grupas, mums ir darbības, ko varat veikt, lai ***izslēgtu komandas*** no [jaunajām](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) vai [esošajām](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office instalācijām. Ja vēlaties, lai darba grupas tiktu instalētas, bet nevēlaties, lai grupas automātiski tiktu startētam lietotājam pēc instalēšanas, skatiet sadaļu [neļaut Microsoft Teams automātisku startēšanu pēc instalācijas](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Lai ***atinstalētu darba grupas*** no ierīces, kurā darbojas sistēma Windows, skatiet sadaļu [Microsoft Teams atinstalēšana](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Lai notīrītu Microsoft Teams no vairākām mērķa mašīnām vai lietotājiem, skatiet sadaļu [Microsoft Teams izvietošanas tīrīšana](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ja izmantojat koplietojamos datorus, attālās darbvirsmas pakalpojumus (RDS) vai virtuālās darbvirsmas infrastruktūru (VDI), skatiet sadaļu [koplietojamā datora un VDI vide, izmantojot Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ja izmantojat Office for Mac, skatiet [Microsoft Teams instalācijas Mac datorā](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Kad komandas ir instalētas, tās tiek [automātiski atjauninātas](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) aptuveni ik pēc divām nedēļām ar jaunām funkcijām un kvalitātes atjauninājumiem. 