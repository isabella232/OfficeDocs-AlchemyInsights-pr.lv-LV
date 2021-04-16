---
title: E-pasta retranslēšana, izmantojot Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809662"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="d0f43-102">Kā iestatīt vairākfunkciju ierīci vai programmu e-pasta nosūtīšanai</span><span class="sxs-lookup"><span data-stu-id="d0f43-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="d0f43-103">Lai iegūtu informāciju par iespējām un norādījumiem, skatiet rakstu [Kā iestatīt vairākfunkciju ierīci vai programmu e-pasta nosūtīšanai, izmantojot Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="d0f43-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="d0f43-104">**Piezīme.** Ja izmantojat ierīci vai programmu, kas pēdējā laikā vairs nedarbojas, ņemiet vērā, ka nesen esam sākuši [atspējot 3DES šifru](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption), kā plānots.</span><span class="sxs-lookup"><span data-stu-id="d0f43-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="d0f43-105">Lai redzētu ietekmētās ierīces, dodieties uz [SMTP Auth klientu atskaiti](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="d0f43-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="d0f43-106">Biežākās kļūdas var būt līdzīgas šīm: autentifikācijas kļūme/kļūda, TLS kļūme/kļūda, šifra algoritma kļūda, algoritma neatbilstība vai savienojuma pārtraukums.</span><span class="sxs-lookup"><span data-stu-id="d0f43-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="d0f43-107">Lai novērstu problēmu:</span><span class="sxs-lookup"><span data-stu-id="d0f43-107">To resolve the issue:</span></span>

 - <span data-ttu-id="d0f43-108">**Windows Server 2003 IIS SMTP vairs nedarbosies — nepieciešama jaunāka Windows versija.**</span><span class="sxs-lookup"><span data-stu-id="d0f43-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="d0f43-109">Sazinieties ar lietojumprogrammas vai ierīces pārdevēju, lai pārbaudītu, vai tiek atbalstīts jaunākais šifrs un vai ir pieejams atjauninājums.</span><span class="sxs-lookup"><span data-stu-id="d0f43-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
