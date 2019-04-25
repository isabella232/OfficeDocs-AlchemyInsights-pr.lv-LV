---
title: Pārvēršot koplietojamās pastkastes lietotāja pastkasti?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374330"
---
<span data-ttu-id="49412-102">Lietotāja pastkastē var konvertēt tikai koplietojamā pastkasti, ja lietotājam ir Exchange licences.</span><span class="sxs-lookup"><span data-stu-id="49412-102">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="49412-103">Pēc konvertēšanas pastkasti, tā turpinās, jo šis saraksts ietver kopīgu pastkastes Aktīvie lietotāji sarakstā parādās.</span><span class="sxs-lookup"><span data-stu-id="49412-103">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="49412-104">Tomēr konvertēto pastkastītē arī parādīsies koplietojamo pastkastu sarakstā.</span><span class="sxs-lookup"><span data-stu-id="49412-104">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="49412-105">Ja jūs mēģināt konvertēt ar pastkasti Exchange administratora konsole un konversijas neizdodas, notīrīt pārlūkprogrammas kešatmiņu un sīkfailus un mēģiniet vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="49412-105">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="49412-106">Ja tas joprojām nedarbojas, mēģiniet konvertēt uz pastkasti Exchange Management Shell, izpildot šādu komandu:</span><span class="sxs-lookup"><span data-stu-id="49412-106">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="49412-107">Vairākas pastkastes konversijas informācija ir pieejama [pārvērst koplietojamās pastkastes lietotāja pastkastes](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="49412-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
