---
title: Publisko mapju atļauju iestatīšana vai mainīšana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: c035d56ffade45cc4360a1d0dfca4c63bf110a38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771179"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="7e81b-102">Atļaujas un publiskās mapes</span><span class="sxs-lookup"><span data-stu-id="7e81b-102">Permissions and Public Folders</span></span>

<span data-ttu-id="7e81b-103">Varat mainīt publisko mapju atļaujas, izmantojot programmu Outlook, Exchange admin Center (EAC) vai PowerShell:</span><span class="sxs-lookup"><span data-stu-id="7e81b-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="7e81b-104">Lai skatītu Outlook instrukcijas, [noklikšķiniet šeit](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="7e81b-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="7e81b-105">Par EAC skatiet [šajā rakstā](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) sniegtos norādījumus.</span><span class="sxs-lookup"><span data-stu-id="7e81b-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="7e81b-106">PowerShell gadījumā skatiet [šo rakstu](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) , lai uzzinātu, kā izmantot pievienojumprogrammu PublicFolderClientPermission unifiedgroup.</span><span class="sxs-lookup"><span data-stu-id="7e81b-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="7e81b-107">Ja ir nepieciešami norādījumi, lai izveidotu savienojumu ar Exchange PowerShell, noklikšķiniet [šeit](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="7e81b-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="7e81b-108">Ja **ārējie lietotāji nevar nosūtīt e-pasta ziņojumus uz publiski pieejamu publisko mapi**, iespējams, ka publiskajai mapei trūkst atļauju, kas nepieciešama ārējai e-pasta piegādei.</span><span class="sxs-lookup"><span data-stu-id="7e81b-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="7e81b-109">To var novērst, izmantojot Outlook norādījumus [šeit](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)vai PowerShell [instrukcijas.](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)</span><span class="sxs-lookup"><span data-stu-id="7e81b-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

