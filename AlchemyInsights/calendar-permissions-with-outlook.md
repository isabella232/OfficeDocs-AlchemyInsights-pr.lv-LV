---
title: Kalendāra atļaujas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862091"
---
# <a name="calendar-permissions"></a>Kalendāra atļaujas

Lietotāji var mainīt savas kalendāra atļaujas programmā Outlook tīmeklī vai citos klientos, bet kā administrators, iespējams, būs jāizpēta.  
Ar Exchange PowerShell cmdlet jums parādīs atļauju lietotāja kalendārā:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Lai skatītu papildinformāciju, skatiet tālāk norādītoinformāciju.

- [Iegūt MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set MailboxFolderPermission Set MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Pievienot MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalendāra atļaujas tiek izmantotas kalendāru koplietošanai, lai skatītu papildinformāciju par Outlook kalendāra koplietošanu, skatiet šos rakstus:

- [Outlook kalendāra koplietošana ar citiem lietotājiem](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Kalendāra kopīgošana programmā Outlook tīmeklī darbam](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Lai novērstu kalendāra atļaujas, varat izmantot atbalsta [un atkopšanas palīga](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) rīku.