---
title: 2491 brīdinājuma e-pasta ziņojumus no Phish piegādāti, nomnieks vai lietotājs ignorē politikas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391388"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="7b39b-102">Brīdinājuma e-pasta ziņojumus no Phish piegādāti, nomnieks vai lietotājs ignorē politikas</span><span class="sxs-lookup"><span data-stu-id="7b39b-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="7b39b-103">Noklusējuma brīdinājuma politiku ar nosaukumu "Phish piegādāts nomnieka vai lietotāja ignorēšanas dēļ" ir iepazīstinājusi ar Office 365 ATP P1 un P2 licences īrniekiem.</span><span class="sxs-lookup"><span data-stu-id="7b39b-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="7b39b-104">Ja esat saņēmis šādu brīdinājumu, šeit ir soļi, lai izpētītu:</span><span class="sxs-lookup"><span data-stu-id="7b39b-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="7b39b-105">Brīdinājuma ziņojumu, noklikšķiniet uz **Skatīt brīdinājumu** iet & drošības ievērošanu centrs lappusi **brīdinājumu** .</span><span class="sxs-lookup"><span data-stu-id="7b39b-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="7b39b-106">Atlasiet brīdinājumu, lai redzētu opciju **Skatīt ziņojumu sarakstu** vai **ziņojumu skatīšana programmā Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="7b39b-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="7b39b-107">Abas šīs iespējas jūs nonāksiet ziņas detaļas, kas ietver ziņojuma ID.</span><span class="sxs-lookup"><span data-stu-id="7b39b-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="7b39b-108">Ņemiet vērā, ka draudus Explorer saites automātiski filtrē ziņojumus, kas atbilst brīdinājumu kritērijiem.</span><span class="sxs-lookup"><span data-stu-id="7b39b-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="7b39b-109">Iespējams, vajadzēs pielāgot datuma filtrs programmā Internet Explorer draudi.</span><span class="sxs-lookup"><span data-stu-id="7b39b-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="7b39b-110">Pikšķerēšanas ziņojums tika piegādāts manuāli konfigurētu ignorēšanas dēļ:</span><span class="sxs-lookup"><span data-stu-id="7b39b-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="7b39b-111">Atļauto sūtītāju vai domēnu signâla lîmeni.</span><span class="sxs-lookup"><span data-stu-id="7b39b-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="7b39b-112">Atļauto sūtītāju vai domēnu noteiktajā admin pretsurogātpasta politiku.</span><span class="sxs-lookup"><span data-stu-id="7b39b-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="7b39b-113">Atļauto IP adresi savienojumu filtrs politikā.</span><span class="sxs-lookup"><span data-stu-id="7b39b-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="7b39b-114">Pasta plūsmas noteikums (pazīstams arī kā transporta noteikums), kas ir konfigurēta, lai atļautu ziņojumus.</span><span class="sxs-lookup"><span data-stu-id="7b39b-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="7b39b-115">Ja jūs uzskatāt, ka ziņojums tika nepareizi atzīmēts kā phish phish, izmantot Outlook [pievienojumprogramma atskaites ziņojumu](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) iesniegt ziņojumu paraugus korporācijai Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7b39b-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
