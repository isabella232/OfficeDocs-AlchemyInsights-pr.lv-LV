---
title: Noteikt e-pasta piegādes jautājumiem pasta publiskajās mapēs
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525124"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="8f6c1-102">Noteikt e-pasta piegādes jautājumiem pasta publiskajās mapēs</span><span class="sxs-lookup"><span data-stu-id="8f6c1-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="8f6c1-103">Ja ārējiem sūtītājiem ziņas nevar nosūtīt pasta publiskajām mapēm un sūtītāju atgriezta kļūda: **nav atrodama (550 5.4.1)**, pārbaudīt e-pasta adreses domēns, lai publiskā mape ir konfigurēta kā iekšējo pārraides domēnu, nevis autoritatīvu domēnu:</span><span class="sxs-lookup"><span data-stu-id="8f6c1-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="8f6c1-104">Atveriet [Exchange administratoru centrā (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="8f6c1-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="8f6c1-105">Dodieties uz **pasta plūsmu** \> **akceptēts domēni**atlasiet akceptēto domēnu un pēc tam noklikšķiniet uz **Rediģēt**.</span><span class="sxs-lookup"><span data-stu-id="8f6c1-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="8f6c1-106">Rekvizītu lapa kas tiek atvērts, ja domēna tips ir iestatīts kā **Authoritative**, mainiet vērtību uz **iekšējo pārraides** un pēc tam noklikšķiniet uz **saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="8f6c1-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="8f6c1-107">Ja ārējiem sūtītājiem saņemtu, **jums nav atļaujas (550 5.7.13)** kļūda, palaidiet tālāk norādīto komandu [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , lai redzētu, kādas atļaujas par anonīmiem lietotājiem publiskajā mapē.</span><span class="sxs-lookup"><span data-stu-id="8f6c1-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="8f6c1-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Piemēram, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="8f6c1-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="8f6c1-109">Ļaut ārējiem lietotājiem sūtīt e-pastu uz šo publisko mapi, pievienot CreateItems piekļuves tiesības anonīms lietotājs.</span><span class="sxs-lookup"><span data-stu-id="8f6c1-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="8f6c1-110">Piemēram, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="8f6c1-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
