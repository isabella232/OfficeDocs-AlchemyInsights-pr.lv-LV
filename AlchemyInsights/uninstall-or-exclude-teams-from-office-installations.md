---
title: Darba grupu atinstalēšana vai izslēgšana no Office instalācijām
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658228"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Grupu atinstalēšana vai izslēgšana no jaunajām vai esošajām Office instalācijām

Microsoft Teams ir iekļautas Microsoft 365 lietojumprogrammās, kas paredzētas uzņēmumiem, Microsoft 365 lietojumprogrammām darbam un Office for Mac.

- Izmantojiet [Office izvietošanas rīku](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) , lai izslēgtu komandas no jaunām Office instalācijām.
- Lai *atinstalētu* komandas no ierīces, kurā darbojas operētājsistēma Windows, skatiet rakstu [Microsoft Teams atinstalēšana](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Lai iztīrītu Microsoft Teams no vairākiem Target datoriem vai lietotājiem, skatiet rakstu [Microsoft Teams izvietošanas tīrīšana](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Izmantojiet [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) opciju, lai neļautu programmai Microsoft Teams automātiski instalēt Office.
- Izmantojiet [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) opciju, *pirms darba grupas ir instalētas*, lai neļautu Microsoft Teams automātiski startēties pēc instalēšanas.

Ja izmantojat Office darbam ar Mac, skatiet rakstu [Microsoft Teams instalācijas Mac datorā](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).