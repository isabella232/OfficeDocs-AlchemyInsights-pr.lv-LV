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
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="1cb75-102">Microsoft Defender iespējošana programmatūrai Office 365 SharePoint Online, OneDrive un Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="1cb75-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="1cb75-103">Dodieties https://protection.office.com uz sadaļu un pierakstieties.</span><span class="sxs-lookup"><span data-stu-id="1cb75-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="1cb75-104">Izvēlieties **Apdraudējumu pārvaldības**  >  **politika** Seifs  >  **pielikumiem.**</span><span class="sxs-lookup"><span data-stu-id="1cb75-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="1cb75-105">Atlasiet **Opciju Programmatūras Defender Office 365 programmatūrām SharePoint, OneDrive programmatūrā un Microsoft Teams** tam noklikšķiniet uz **Saglabāt.**</span><span class="sxs-lookup"><span data-stu-id="1cb75-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="1cb75-106">(Ieteicams) Kā globālais administrators vai SharePoint Online administrators izpildiet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet ar iestatīto parametru **DisallowInfectedFileDownload** kā *true*.</span><span class="sxs-lookup"><span data-stu-id="1cb75-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="1cb75-107">(Ieteicams) [Iestatīt brīdinājumus par konstatētajiem](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) failiem.</span><span class="sxs-lookup"><span data-stu-id="1cb75-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="1cb75-108">Microsoft Defender Office 365 neskenēs katru failu programmā SharePoint Online, OneDrive vai Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1cb75-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="1cb75-109">Faili tiek skenēti asinhroni, izmantojot procesu, kas izmanto koplietošanas un viesdarbību notikumus, kā arī viedos heurtiku un apdraudējumu signālus, lai identificētu ļaunprātīgus failus.</span><span class="sxs-lookup"><span data-stu-id="1cb75-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="1cb75-110">Skatiet [rakstu Microsoft Defender Office 365 SharePoint, OneDrive un Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="1cb75-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>