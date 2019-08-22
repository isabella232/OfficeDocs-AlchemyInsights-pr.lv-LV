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
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496442"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="d1948-102">Pārvērstu koplietojamās pastkastes lietotāja pastkastē</span><span class="sxs-lookup"><span data-stu-id="d1948-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="d1948-103">Lietotāja pastkastē var konvertēt tikai koplietojamā pastkasti, ja lietotājam ir Exchange licences.</span><span class="sxs-lookup"><span data-stu-id="d1948-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="d1948-104">Pēc konvertēšanas pastkasti, tā turpinās, jo šis saraksts ietver kopīgu pastkastes Aktīvie lietotāji sarakstā parādās.</span><span class="sxs-lookup"><span data-stu-id="d1948-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="d1948-105">Tomēr konvertēto pastkastītē arī parādīsies koplietojamo pastkastu sarakstā.</span><span class="sxs-lookup"><span data-stu-id="d1948-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="d1948-106">Ja jūs mēģināt konvertēt ar pastkasti Exchange administratora konsole un konversijas neizdodas, notīrīt pārlūkprogrammas kešatmiņu un sīkfailus un mēģiniet vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="d1948-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="d1948-107">Ja tas joprojām nedarbojas, mēģiniet konvertēt uz pastkasti Exchange Management Shell, izpildot šādu komandu:</span><span class="sxs-lookup"><span data-stu-id="d1948-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="d1948-108">Vairākas pastkastes konversijas informācija ir pieejama [pārvērst koplietojamās pastkastes lietotāja pastkastes](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="d1948-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
