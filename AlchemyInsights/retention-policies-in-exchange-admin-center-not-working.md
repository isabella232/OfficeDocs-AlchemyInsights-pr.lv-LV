---
title: Saglabāšanas politikas Exchange administrēšanas centrā nedarbojas
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740517"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Saglabāšanas politikas Exchange administrēšanas centrā

Ja vēlaties, lai mēs veiktu automatizētās pārbaudes par tālāk norādītajiem iestatījumiem, atlasiet pogu atpakaļ < — šīs lapas augšdaļā un pēc tam ievadiet tā lietotāja e-pasta adresi, kuram ir problēmas ar saglabāšanas politikām.

 **Problēma:** Jaunizveidotās vai atjauninātās saglabāšanas politikas Exchange administrēšanas centrā neattiecas uz pastkastēm vai vienumiem netiek pārvietoti uz arhīva pastkasti vai izdzēsti. 
  
 **Saknes cēloņi:**
  
- Tas, iespējams, ir tāpēc, ka **pārvaldītā mapes palīgs** nav apstrādājis lietotāja pastkasti. Pārvaldītā mapes palīgs mēģina apstrādāt katru pastkasti mākonī savā organizācijā ik pēc septiņām dienām. Ja pastkastē maināt saglabāšanas atzīmi vai lietojat citu saglabāšanas politiku, varat nogaidīt līdz brīdim, kad pārvaldītā mape atbalsta šo pastkasti, vai arī varat palaist sākuma ManagedFolderAssistant cmdlet, lai startētu pārvaldīto mapju palīgu, lai apstrādātu noteiktu pastkasti. Šī cmdlet darbība ir noderīga saglabāšanas politikas vai saglabāšanas atzīmju iestatījumu pārbaudei vai problēmu novēršanai. Lai iegūtu papildinformāciju, skatiet rakstu [pārvaldītā mapes palīga palaišana](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Risinājums:** Palaidiet tālāk norādīto komandu, lai startētu pārvaldīto mapju palīgu noteiktai pastkastei.
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Tas var arī rasties, ja pastkastē ir **iespējota** **RetentionHold** . Ja pastkaste ir ievietota RetentionHold, saglabāšanas politika pastkastē netiks apstrādāta šajā laikā. Lai iegūtu vairāk instalāciju par RetentionHold iestatījumu, skatiet rakstu [pastkastes aiztures aizturēšana](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Risinājumu**
    
  - Pārbaudiet RetentionHold statusu noteiktā pastkastē programmā [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps).
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Lai **atspējotu** RetentionHold noteiktā pastkastē, izpildiet šādu komandu:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Tagad atkārtoti palaidiet pārvaldītās mapes palīgu:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Piezīme:** Ja pastkaste ir mazāka par 10 MB, pārvaldītā mapes palīgs automātiski neapstrādās pastkasti.
 
Papildinformāciju par saglabāšanas politikām Exchange administrēšanas centrā skatiet šeit:
- [Saglabāšanas tagi un saglabāšanas politikas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Saglabāšanas politikas lietošana pastkastēm](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Saglabāšanas atzīmju pievienošana un noņemšana](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kā noteikt pastkastes aizturēšanas tipu](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
