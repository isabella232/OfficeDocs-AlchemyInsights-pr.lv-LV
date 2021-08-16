---
title: Savrupu Teams izvietošana ar jaunām vai esošām Office instalācijām
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
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102209"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Savrupu Teams izvietošana ar jaunām vai esošām Office instalācijām

Microsoft Teams tagad ir iekļauta jaunajās  Microsoft 365 programmas lieluzņēmumiem, Microsoft 365 programmas darbam un Office darbam ar Mac instalācijās. Papildinformāciju skatiet [rakstā Kad Microsoft Teams tiks iekļauta jaunajās Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Turklāt, sākot ar versiju 1906 pašreizējā kanālā  , Teams tiks pievienota esošajām Microsoft 365 programmas lieluzņēmumiem (un Microsoft 365 programmas darbam) instalācijām ierīcēs, kurās darbojas Windows, kad atjaunināt esošo instalāciju uz jaunāko versiju. Papildinformāciju skatiet rakstā [Kā ar esošajām Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ja nevēlaties gaidīt šo ieviešanas grafiku, varat izvietot Teams kā savrupu pakalpojumu [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) saviem lietotājiem, izpildot šos norādījumus, vai arī varat atļaut lietotājiem instalēt Teams saviem lietotājiem [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) no .

Ja jūsu organizācija nav gatava izvietot Teams, mēs veicamās darbības, lai Teams izslēgtu [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) no [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) jaunām vai esošām Office.  Ja Teams vēlaties, lai tā tiktu instalēta, bet nevēlaties Teams lai lietotājs tiktu automātiski startēts pēc instalēšanas, skatiet rakstu Automātiskas Microsoft Teams startēšanas nepieļaušana pēc [instalēšanas.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Lai ***atinstalētu Teams*** ierīcē, kurā darbojas Windows, skatiet [rakstu Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Informāciju par Microsoft Teams no vairākiem mērķa datoriem vai lietotājiem skatiet rakstā [Microsoft Teams tīrīšana.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Ja izmantojat koplietojamos [datorus, attālās darbvirsmas](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)pakalpojumus (Remote Desktop Services - RDS) vai virtuālās darbvirsmas infrastruktūru (VDI), skatiet sadaļu Koplietotais dators un VDI vides ar Microsoft Teams.

Ja izmantojat programmu Office darbam ar Mac, skatiet [rakstu Microsoft Teams instalācijas Mac datorā.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> Pēc Teams atjaunināšana tiek automātiski atjaunināta [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) aptuveni ik pēc divām nedēļām, izmantojot jaunus līdzekļus un kvalitātes atjauninājumus. 