---
title: AtP Office 365 iespējošana SharePoint, OneDrive un Microsoft Teams
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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543935"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Microsoft Defender iespējošana programmatūrai Office 365 SharePoint Online, OneDrive un Microsoft Teams

1. Dodieties https://protection.office.com uz sadaļu un pierakstieties.
2. Izvēlieties **Apdraudējumu pārvaldības**  >  **politika** Seifs  >  **pielikumiem.**
3. Atlasiet **Opciju Programmatūras Defender Office 365 programmatūrām SharePoint, OneDrive programmatūrā un Microsoft Teams** tam noklikšķiniet uz **Saglabāt.**
4. (Ieteicams) Kā globālais administrators vai SharePoint Online administrators izpildiet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet ar iestatīto parametru **DisallowInfectedFileDownload** kā *true*.
5. (Ieteicams) [Iestatīt brīdinājumus par konstatētajiem](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) failiem.

> [!NOTE]
> Microsoft Defender Office 365 neskenēs katru failu programmā SharePoint Online, OneDrive vai Microsoft Teams. Faili tiek skenēti asinhroni, izmantojot procesu, kas izmanto koplietošanas un viesdarbību notikumus, kā arī viedos heurtiku un apdraudējumu signālus, lai identificētu ļaunprātīgus failus. Skatiet [rakstu Microsoft Defender Office 365 SharePoint, OneDrive un Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)