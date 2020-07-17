---
title: E-pasta retranslēšana, izmantojot Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 074a9106553bf3a2a5e563f9ebaca9dfc38111cb
ms.sourcegitcommit: 9872280f71429d2344b0b441e218fba5b3bd3cf7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/02/2020
ms.locfileid: "45023466"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="2559c-102">Kā iestatīt vairākfunkciju ierīci vai programmu e-pasta nosūtīšanai</span><span class="sxs-lookup"><span data-stu-id="2559c-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="2559c-103">Lai iegūtu informāciju par iespējām un norādījumiem, skatiet rakstu [Kā iestatīt vairākfunkciju ierīci vai programmu e-pasta nosūtīšanai, izmantojot Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="2559c-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="2559c-104">**Piezīme.** Ja izmantojat ierīci vai programmu, kas pēdējā laikā vairs nedarbojas, ņemiet vērā, ka nesen esam sākuši [atspējot 3DES šifru](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption), kā plānots.</span><span class="sxs-lookup"><span data-stu-id="2559c-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="2559c-105">Lai redzētu ietekmētās ierīces, dodieties uz [SMTP Auth klientu atskaiti](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="2559c-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="2559c-106">Biežākās kļūdas var būt līdzīgas šīm: autentifikācijas kļūme/kļūda, TLS kļūme/kļūda, šifra algoritma kļūda, algoritma neatbilstība vai savienojuma pārtraukums.</span><span class="sxs-lookup"><span data-stu-id="2559c-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="2559c-107">Lai novērstu problēmu:</span><span class="sxs-lookup"><span data-stu-id="2559c-107">To resolve the issue:</span></span>

 - <span data-ttu-id="2559c-108">**Windows Server 2003 IIS SMTP vairs nedarbosies — nepieciešama jaunāka Windows versija.**</span><span class="sxs-lookup"><span data-stu-id="2559c-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="2559c-109">Sazinieties ar lietojumprogrammas vai ierīces pārdevēju, lai pārbaudītu, vai tiek atbalstīts jaunākais šifrs un vai ir pieejams atjauninājums.</span><span class="sxs-lookup"><span data-stu-id="2559c-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
