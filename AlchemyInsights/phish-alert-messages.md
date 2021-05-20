---
title: 2491 Brīdinājuma e-pasta ziņojumi no politikas "Pikšķerēšana piegādāts nomnieka vai lietotāja ignorēšanas dēļ"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544585"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="dde52-102">Brīdinājuma e-pasta ziņojumi no politikas "Pikšķerēšana piegādāts nomnieka vai lietotāja ignorēšanas dēļ"</span><span class="sxs-lookup"><span data-stu-id="dde52-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="dde52-103">Nomniekiem ar programmatūras Microsoft Defender Office 365 P1 un P2 licencēm ir veikta noklusējuma brīdinājuma politika "Pikšķerēšanas piegādāts nomnieka vai lietotāja ignorēšanas dēļ".</span><span class="sxs-lookup"><span data-stu-id="dde52-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="dde52-104">Ja esat saņēmis šo brīdinājumu, veiciet tālāk norādītās darbības, lai izpētītu:</span><span class="sxs-lookup"><span data-stu-id="dde52-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="dde52-105">Brīdinājuma ziņojumā noklikšķiniet uz **Skatīt brīdinājumu,** lai **pārietu** uz lapu Brīdinājumi drošības kontroles & centrā.</span><span class="sxs-lookup"><span data-stu-id="dde52-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="dde52-106">Atlasiet brīdinājumu, lai skatītu opciju Skatīt **ziņojumu sarakstu vai** Skatīt ziņojumus **pārlūkā**.</span><span class="sxs-lookup"><span data-stu-id="dde52-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="dde52-107">Abas šīs opcijas ļauj piekļūt detalizētai informācijai par ziņojumu, kurā iekļauts ziņojuma ID.</span><span class="sxs-lookup"><span data-stu-id="dde52-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="dde52-108">Ņemiet vērā, ka saite Apdraudējumu pārlūks automātiski filtrēs brīdinājumu kritērijiem atbilstošos ziņojumus.</span><span class="sxs-lookup"><span data-stu-id="dde52-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="dde52-109">Var būt nepieciešams pielāgot datuma filtru apdraudējumu pārlūkā.</span><span class="sxs-lookup"><span data-stu-id="dde52-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="dde52-110">Pikšķerēšanas ziņojums tika piegādāts manuāli konfigurētas ignorēšanas dēļ:</span><span class="sxs-lookup"><span data-stu-id="dde52-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="dde52-111">Atļautais sūtītājs vai domēns, ko iestatījis lietotājs.</span><span class="sxs-lookup"><span data-stu-id="dde52-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="dde52-112">Atļautais sūtītājs vai domēns, ko administrators ir iestatījis surogātpasta novēršanas politikā.</span><span class="sxs-lookup"><span data-stu-id="dde52-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="dde52-113">Atļautā IP adrese savienojuma filtra politikā.</span><span class="sxs-lookup"><span data-stu-id="dde52-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="dde52-114">Pasta plūsmas kārtula (tiek dēvēta arī par transporta kārtulu), kas ir konfigurēta atļaut ziņojumus.</span><span class="sxs-lookup"><span data-stu-id="dde52-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="dde52-115">Ja uzskatāt, ka ziņojums ir nepareizi atzīmēts kā [](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) pikšķerēšanas ziņojums, izmantojiet Outlook ziņojuma pievienojumprogrammu, lai iesniegtu ziņojumu paraugus korporācijai Microsoft.</span><span class="sxs-lookup"><span data-stu-id="dde52-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
