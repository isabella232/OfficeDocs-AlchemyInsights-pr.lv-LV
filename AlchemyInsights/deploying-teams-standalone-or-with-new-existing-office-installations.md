---
title: Izvietot komandas kā savrupajam vai ar jaunu vai esošu Office instalāciju
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054237"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Izvietot komandas kā savrupajam vai ar jaunu vai esošu Office instalāciju

Microsoft Teams tagad ir iekļauta kā daļa no ***jaunām iekārtām*** Office 365 ProPlus, Office 365 Business un Office Mac. Lai iegūtu papildinformāciju, skatiet [kad Microsoft Teams sāks netiktu iekļauts jaunās Office instalācijas?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Turklāt sākot ar versiju 1906 ikmēneša kanālā, komandām būs ***pievienots esošajām iekārtām*** Office 365 ProPlus (un Office 365 Business) ierīces, kurās darbojas Windows, kad savai esošajai instalācijai atjaunināt ar jaunāko versiju. Lai iegūtu papildinformāciju, skatiet [kas par esošās iekārtas biroja?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Ja nevēlaties gaidīt šo ieviešanas grafiku, varat izvietot komandas kā savrupu lietotāju, [izpildot šos norādījumus](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) vai arī jums var būt jūsu lietotājiem instalēt sevi no komandas [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Ja uzņēmumā nav gatava izvietot komandas, mums ir darbības, kuras varēsit veikt, lai ***izslēgtu komandu*** no [jauna](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) vai [esoša](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) biroja iekārtām. Ja vēlaties instalēt, bet gribu komandas, lai sāktu darboties automātiski, lietotājam pēc tam, kad tā ir uzstādīta, sk. [Novērst Microsoft komandas startēties automātiski pēc uzstādīšanas](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)komandas.

***Atinstalēt komandām*** no ierīces, kurā darbojas Windows, skatiet [Atinstalēt Microsoft komandām](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Tīrīšanas Microsoft Teams no vairākiem mērķa mašīnas vai lietotājiem, skatiet [Microsoft brigāžu izvietošanu sakopt](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ja izmantojat koplietojamu datoru, attālo darbvirsmas pakalpojumi (RDS) vai virtuālo Desktop infrastruktūru (VDI), sk. [koplietotā datorā un VDI vidēs ar Microsoft komandas](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ja jūs izmantojat Office Mac, skatiet [Microsoft grupas iekārtām uz Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Pēc komandas instalēšanas tā ir [automātiski atjaunināta](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) apmēram ik pēc divām nedēļām ar jauniem līdzekļiem un kvalitāti atjauninājumus. 