---
title: E-pasta piegādes problēmu novēršana uz pasta iespējotām publiskajām mapēm
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677935"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="f1025-102">E-pasta piegādes problēmu novēršana uz pasta iespējotām publiskajām mapēm</span><span class="sxs-lookup"><span data-stu-id="f1025-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="f1025-103">Ja ārējie sūtītāji nevar nosūtīt ziņojumus uz jūsu e-pasta publiskajām mapēm, un sūtītāji saņem kļūdu: nav **atrasts (550 5.4.1)**, pārbaudiet, vai publiskas mapes e-pasta domēns ir konfigurēts kā iekšējs pārraides domēns, nevis autoritatīvs domēns:</span><span class="sxs-lookup"><span data-stu-id="f1025-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="f1025-104">Atveriet [Exchange admin Center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="f1025-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="f1025-105">Dodieties uz sadaļu **pasta plūsmas** \> **akceptētie domēni**, atlasiet akceptēto domēnu un pēc tam noklikšķiniet uz **Rediģēt**.</span><span class="sxs-lookup"><span data-stu-id="f1025-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="f1025-106">Rekvizītu lapā, kas tiek atvērta, ja domēna tips ir iestatīts kā **autoritatīvs**, nomainiet vērtību uz **iekšējo releju** un pēc tam noklikšķiniet uz **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="f1025-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="f1025-107">Ja ārējie sūtītāji saņem kļūdas ziņojumu, kam **nav atļaujas (550 5.7.13)**, izpildiet šo komandu pakalpojumā [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , lai skatītu anonīmu lietotāju atļaujas publiskajā mapē:</span><span class="sxs-lookup"><span data-stu-id="f1025-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="f1025-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Piemēram, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="f1025-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="f1025-109">Lai atļautu ārējiem lietotājiem nosūtīt e-pasta ziņojumus uz šo publisko mapi, pievienojiet CreateItems piekļuves tiesības lietotājam anonīms.</span><span class="sxs-lookup"><span data-stu-id="f1025-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="f1025-110">Piemēram, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="f1025-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
