---
title: Iespējojiet Office 365 ATP pakalpojumam SharePoint, OneDrive un Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709914"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Iespējojiet Office 365 Advanced Threat Protection pakalpojumam SharePoint Online, OneDrive un Microsoft Teams

1. Dodieties uz https://protection.office.com un pierakstieties.
2. Izvēlieties **draudus pārvaldības**  >  **politikas**  >  **drošības pielikumi**.
3. Atlasiet **Ieslēgt ATP pakalpojumam SharePoint, OneDrive un Microsoft Teams**un pēc tam noklikšķiniet uz **Saglabāt**.
4. Ieteicams Kā globālais administrators vai SharePoint Online administrators izpildiet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet ar parametru **DisallowInfectedFileDownload** , kas iestatīts kā *patiess*.
5. Ieteicams [Iestatiet brīdinājumus](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) par noteiktajiem failiem.

> [!NOTE]
> ATP ir NTO skenē katru atsevišķu failu pakalpojumā SharePoint Online, OneDrive vai Microsoft Teams. Faili tiek skenēti asinhroni, izmantojot procesu, kas izmanto koplietošanas un viesa aktivitāšu notikumus, kā arī viedos heiristiku un draudu signālus, lai identificētu ļaunprātīgus failus. Skatiet rakstu [ATP for SharePoint, OneDrive un Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).