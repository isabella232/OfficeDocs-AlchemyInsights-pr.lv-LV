---
title: 2491 brīdinājuma e-pasta ziņojumus no "phish piegādāts nomnieka vai lietotāja apiešanas dēļ" politika
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758935"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="19af4-102">Alert e-pasta ziņojumus no "phish piegādāts dēļ nomnieka vai lietotāja ignorēt" politika</span><span class="sxs-lookup"><span data-stu-id="19af4-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="19af4-103">Noklusējuma brīdinājuma politika ar nosaukumu "phish piegādāts nomnieka vai lietotāja apiešanas dēļ" ir tika izvelēta nomniekiem ar Office 365 ATP P1 un P2 licencēm.</span><span class="sxs-lookup"><span data-stu-id="19af4-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="19af4-104">Ja saņēmāt šo brīdinājumu, tālāk ir norādītas darbības, kas jāveic, lai izpētītu:</span><span class="sxs-lookup"><span data-stu-id="19af4-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="19af4-105">Brīdinājuma ziņojumā noklikšķiniet uz **Skatīt brīdinājumu** , lai drošības & atbilstības centrā pārietu uz lapu **brīdinājumi** .</span><span class="sxs-lookup"><span data-stu-id="19af4-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="19af4-106">Atlasiet brīdinājumu, lai skatītu opciju skatīt **ziņojumu sarakstu** vai **skatītu ziņojumus programmā Explorer**.</span><span class="sxs-lookup"><span data-stu-id="19af4-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="19af4-107">Abas šīs opcijas ļauj piekļūt ziņojuma detaļām, kas ietver ziņojuma ID.</span><span class="sxs-lookup"><span data-stu-id="19af4-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="19af4-108">Ņemiet vērā, ka saite Threat Explorer automātiski filtrē ziņojumus, kas atbilst brīdinājuma kritērijiem.</span><span class="sxs-lookup"><span data-stu-id="19af4-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="19af4-109">Iespējams, ir jāpielāgo datuma filtrs Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="19af4-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="19af4-110">Pikšķerēšanas ziņojums tika piegādāts dēļ manuāli konfigurēta ignorēšana:</span><span class="sxs-lookup"><span data-stu-id="19af4-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="19af4-111">Atļauto sūtītāju vai domēnu, ko iestatījis lietotājs.</span><span class="sxs-lookup"><span data-stu-id="19af4-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="19af4-112">Atļauto sūtītāju vai domēnu, ko administrators iestatījis pretsurogātpasta politikā.</span><span class="sxs-lookup"><span data-stu-id="19af4-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="19af4-113">Atļauto IP adresi savienojuma filtra politikā.</span><span class="sxs-lookup"><span data-stu-id="19af4-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="19af4-114">Pasta plūsmas kārtula (tiek dēvēta arī par transportēšanas kārtulu), kas ir konfigurēta, lai atļautu ziņojumus.</span><span class="sxs-lookup"><span data-stu-id="19af4-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="19af4-115">Ja uzskatāt, ka ziņojums ir nepareizi atzīmēts kā phish, izmantojiet Outlook ziņojumu [ziņojumu pievienojumprogrammu](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) iesniegt ziņojumu paraugi Microsoft.</span><span class="sxs-lookup"><span data-stu-id="19af4-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
