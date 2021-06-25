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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117990"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="aada8-102">Kā iestatīt vairākfunkciju ierīci vai programmu e-pasta nosūtīšanai</span><span class="sxs-lookup"><span data-stu-id="aada8-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="aada8-103">Lai iegūtu informāciju par iespējām un norādījumiem, skatiet rakstu [Kā iestatīt vairākfunkciju ierīci vai programmu e-pasta nosūtīšanai, izmantojot Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="aada8-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="aada8-104">Ja jums ir ierīce vai lietojumprogramma, kas nesen pārtrauca darboties, visbiežāk sastopamās problēmas ir:</span><span class="sxs-lookup"><span data-stu-id="aada8-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="aada8-105">**Ar autentifikāciju saistītas kļūdas, izmantojot SMTP autentifikācijas klienta iesniegšanu** Nesen veicām dažas izmaiņas saistībā ar SMTP autentifikācijas darbību.</span><span class="sxs-lookup"><span data-stu-id="aada8-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="aada8-106">Papildinformāciju par to, kā novērst problēmas, skatiet sadaļā To printeru, skeneru un LOB lietojumprogrammu problēmu [novēršana,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)kas nosūta e-pastu, izmantojot Microsoft 365 vai Office 365 .</span><span class="sxs-lookup"><span data-stu-id="aada8-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="aada8-107">**Mēs pieņemam tikai TLS 1.2 versiju, kamēr** tiek izveidots drošs savienojums ar Office 365 Ja izmantojat drošo savienojumu (TLS), pārliecinieties, vai jūsu lietojumprogrammas ierīce atbalsta TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="aada8-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="aada8-108">Papildinformāciju skatiet rakstā [Gatavošanās TLS 1.2 sagatavošanai programmā Office 365 un Office 365 GCC.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="aada8-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="aada8-109">Informāciju par citām problēmām un risinājumiem skatiet rakstā To printeru, skeneru un LOB lietojumprogrammu problēmu novēršana, kas sūta [e-pastu, Microsoft 365 vai Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span><span class="sxs-lookup"><span data-stu-id="aada8-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="aada8-110">Lai redzētu ietekmētās ierīces, dodieties uz [SMTP Auth klientu atskaiti](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="aada8-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="aada8-111">**Piezīme.** Exchange Online nav pielāgoti lielapjoma pasta sūtīšanas scenāriji.</span><span class="sxs-lookup"><span data-stu-id="aada8-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="aada8-112">Lai nosūtītu komercpasta lielapjoma ziņojumus (piemēram, klientu biļetenus), izmantojiet trešo pušu pakalpojumu sniedzējus, kas specializējas šajos pakalpojumos.</span><span class="sxs-lookup"><span data-stu-id="aada8-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
