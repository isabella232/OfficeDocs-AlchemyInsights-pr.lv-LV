---
title: Portu Google Chrome paplašinājumi Microsoft Edge (Hroms)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677877"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="4c24f-102">Portu Google Chrome paplašinājumi Microsoft Edge (Hroms)</span><span class="sxs-lookup"><span data-stu-id="4c24f-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="4c24f-103">Ir viegli [pārnest Google Chrome paplašinājumus uz Microsoft Edge (Hroms)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="4c24f-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="4c24f-104">Lielākajā daļā gadījumu šīs Extensions izpildei pārlūkprogrammā Microsoft Edge ir jāveic tikai minimālas izmaiņas.</span><span class="sxs-lookup"><span data-stu-id="4c24f-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="4c24f-105">Google Chrome atbalstītie paplašinājumi API un manifesta taustiņi ir ar kodu saderīgi ar Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="4c24f-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="4c24f-106">Taču Microsoft Edge neatbalsta paplašinājumu API Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken un Chrome. gadījuma ID GUID.</span><span class="sxs-lookup"><span data-stu-id="4c24f-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>