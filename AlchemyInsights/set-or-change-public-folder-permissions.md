---
title: Iestatītu vai mainītu publiskās mapes atļaujas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: d1554e8a63455f3549044e526183c0e8709f2631
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32421823"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="fdce4-102">Atļaujas un publiskās mapes</span><span class="sxs-lookup"><span data-stu-id="fdce4-102">Permissions and Public Folders</span></span>

<span data-ttu-id="fdce4-103">Jūs varat mainīt atļaujas uz publiskajām mapēm, izmantojot Outlook Exchange administratoru centrā (VNK), vai PowerShell:</span><span class="sxs-lookup"><span data-stu-id="fdce4-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="fdce4-104">Outlook instrukcijas, [noklikšķiniet šeit](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="fdce4-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="fdce4-105">VNK, skatiet [rakstā](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) instrukcijas.</span><span class="sxs-lookup"><span data-stu-id="fdce4-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> <span data-ttu-id="fdce4-106">Jūs varat noklikšķināt [šeit](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) , lai virzītos uz VNK.</span><span class="sxs-lookup"><span data-stu-id="fdce4-106">You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="fdce4-107">Powershell, skatiet [šī raksta](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) norādījumus par to, izmantojot pievienot PublicFolderClientPermission commandlet.</span><span class="sxs-lookup"><span data-stu-id="fdce4-107">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="fdce4-108">Ja jums ir nepieciešams pieslēgties apmaiņa Powershell instrukcijas, noklikšķiniet [šeit](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="fdce4-108">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="fdce4-109">Ja **ārējie lietotāji nevar nosūtīt vēstules, pasta publiskajā mapē**, iemesls, iespējams, ka publiskā mape ir pazudis atļaujas pieprasīt ārējiem e-pasta piegādei.</span><span class="sxs-lookup"><span data-stu-id="fdce4-109">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="fdce4-110">To var labot, izmantojot Outlook instrukcijas [šeit](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)vai PowerShell instrukcijas [šeit](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="fdce4-110">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

