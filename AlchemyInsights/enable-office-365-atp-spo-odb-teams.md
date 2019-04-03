---
title: Iespējotu Office 365 ATP SharePoint, OneDrive un grupu Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031022"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Iespējotu Office SharePoint tiešsaistē, OneDrive un komandas Microsoft 365 papildu draudus aizsardzībai

1. Dodieties uz https://protection.office.com un pierakstieties.
2. Izvēlieties **draudu pārvaldības** > **politikas** > **Drošu pielikumu**.
3. Atlasiet **Ieslēgt ATP SharePoint, OneDrive, un Microsoft komandas**un pēc tam noklikšķiniet uz **Saglabāt**.
4. (Ieteicams) Kā pasaules administrators vai SharePoint Online administrators, palaist [Set SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet ar parametru **DisallowInfectedFileDownload** , kas iestatīts uz *true*.
5. (Ieteicams) [Iestatīt brīdinājumus](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) noteiktajiem failiem.

> [!NOTE]
> ATP būs nto skenēšanas ik viena faila SharePoint Online, OneDrive vai Microsoft Teams. Faili tiek skenēti asinhroni, caur procesu, kas izmanto koplietošanas un viesu aktivitāti notikumi kopā ar gudru heiristiku un draudu signālus identificēt ļaunprātīgu failus. Sk. [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).