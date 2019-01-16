---
title: Pārvēršot koplietojamās pastkastes lietotāja pastkasti?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2019
ms.locfileid: "28300865"
---
<span data-ttu-id="9902b-p101">Lietotāja pastkastē var konvertēt tikai koplietojamā pastkasti, ja lietotājam ir Exchange licences. Pēc konvertēšanas pastkasti, tā turpinās, jo šis saraksts ietver kopīgu pastkastes Aktīvie lietotāji sarakstā parādās. Tomēr konvertēto pastkastītē arī parādīsies koplietojamo pastkastu sarakstā.</span><span class="sxs-lookup"><span data-stu-id="9902b-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="9902b-p102">Ja jūs mēģināt konvertēt ar pastkasti Exchange administratora konsole un konversijas neizdodas, notīrīt pārlūkprogrammas kešatmiņu un sīkfailus un mēģiniet vēlreiz. Ja tas joprojām nedarbojas, mēģiniet konvertēt uz pastkasti Exchange Management Shell, izpildot šādu komandu:</span><span class="sxs-lookup"><span data-stu-id="9902b-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="9902b-107">Vairākas pastkastes konversijas informācija ir pieejama [pārvērst koplietojamās pastkastes lietotāja pastkastes](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="9902b-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
