---
title: Office iepriekšējo MSI versiju noņemšana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680725"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="a0ee5-102">Office iepriekšējo MSI versiju noņemšana</span><span class="sxs-lookup"><span data-stu-id="a0ee5-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="a0ee5-103">Pirms Office 365 ProPlus instalēšanas iesakām noņemt iepriekšējās Office Windows Installer (MSI) versijas.</span><span class="sxs-lookup"><span data-stu-id="a0ee5-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="a0ee5-104">Tālāk ir aprakstīts, kā to paveikt.</span><span class="sxs-lookup"><span data-stu-id="a0ee5-104">Here's how to do this:</span></span>

1. <span data-ttu-id="a0ee5-105">Ja esat izmantojis MSI, lai instalētu Office, varat izmantot Office izvietošanas rīku (ODT), lai atinstalētu Office.</span><span class="sxs-lookup"><span data-stu-id="a0ee5-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="a0ee5-106">Varat izmantot RemoveMSI elementu **configuration.xml** failā.</span><span class="sxs-lookup"><span data-stu-id="a0ee5-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="a0ee5-107">Izpildiet norādījumus šajā rakstā: [Office 365 drošības & atbilstības centrs.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="a0ee5-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>