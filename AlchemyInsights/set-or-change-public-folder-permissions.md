---
title: Publiskās mapes atļauju iestatīšana vai mainīšana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: cf891a4db05b8a2bdb223cc86693f5072faca494
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43681111"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="750e7-102">Atļaujas un publiskās mapes</span><span class="sxs-lookup"><span data-stu-id="750e7-102">Permissions and Public Folders</span></span>

<span data-ttu-id="750e7-103">Publiskās mapes atļaujas var mainīt, izmantojot programmu Outlook, Exchange administrēšanas centru (EAC) vai PowerShell:</span><span class="sxs-lookup"><span data-stu-id="750e7-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="750e7-104">Outlook instrukcijas, [noklikšķiniet šeit](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="750e7-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="750e7-105">EAC skatiet [šo rakstu](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) , lai saņemtu norādījumus.</span><span class="sxs-lookup"><span data-stu-id="750e7-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="750e7-106">PowerShell, skatiet [šo rakstu](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) , lai saņemtu norādījumus par to, kā izmantot ADD-PublicFolderClientPermission commandlet.</span><span class="sxs-lookup"><span data-stu-id="750e7-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="750e7-107">Ja jums ir nepieciešami norādījumi, lai izveidotu savienojumu ar Exchange PowerShell, noklikšķiniet [šeit](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="750e7-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="750e7-108">Ja **ārējie lietotāji nevar sūtīt e-pasta ziņojumu publiskajai mapei ar pasta**starpniecību, iemesls, iespējams, ir tas, ka publiskajai mapei trūkst atļauju, kas nepieciešamas ārējai e-pasta piegādei.</span><span class="sxs-lookup"><span data-stu-id="750e7-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="750e7-109">To var novērst, izmantojot Outlook instrukcijas [šeit](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)vai PowerShell instrukcijas [šeit](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="750e7-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

