---
title: Kalendāra atļaujas
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
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748800"
---
# <a name="calendar-permissions"></a>Kalendāra atļaujas

Lietotāji var mainīt savas kalendāra atļaujas, izmantojot programmu Outlook tīmeklī vai citiem klientiem, bet kā administrators, iespējams, būs nepieciešams izpētīt.  
Izmantojot Exchange PowerShell cmdlet, jums tiek rādītas atļaujas lietotāja kalendārā:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Lai skatītu papildinformāciju, skatiet tālāk minēto informāciju.

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalendāra atļaujas tiek lietotas kalendāru kopīgošanā, lai skatītu papildinformāciju par Outlook kalendāra koplietošanu, skatiet šos rakstus:

- [Outlook kalendāra koplietošana ar citiem lietotājiem](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Kalendāra kopīgošana programmā Outlook tīmeklī uzņēmumiem](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Lai novērstu kalendāra atļaujas, varat izmantot rīku [atbalsta un atkopšanas palīgs](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .