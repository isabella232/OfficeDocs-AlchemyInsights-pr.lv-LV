---
title: Pamati darbam ar SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: afb1ef115d364ee3e2cf09ea850adb57ad1d44e6
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770569"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="f651f-102">Darbplūsmas, koplietošanas vidē SharePoint</span><span class="sxs-lookup"><span data-stu-id="f651f-102">Workflows in SharePoint</span></span>

<span data-ttu-id="f651f-103">Ja SharePoint darbplūsmas nesūta e-pastu, jūsu organizācija ir konstatējis Exchange Online sūtītāja robežas.</span><span class="sxs-lookup"><span data-stu-id="f651f-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="f651f-104">"Darba plūsma tiks pārtraukta" kļūdas ziņojums var rasties, ja esat viens no šiem vienumiem:</span><span class="sxs-lookup"><span data-stu-id="f651f-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="f651f-105">Darbplūsma ir SharePoint Online, kas izmanto SharePoint 2010 vai SharePoint 2013 darbplūsmas platformas tipa.</span><span class="sxs-lookup"><span data-stu-id="f651f-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="f651f-106">Darbplūsma ir konfigurēta, lai nosūtītu pielāgotus e-pasta ziņu vairāk nekā 200 lietotājiem laikā, vairāk nekā 10000 adresāti dienā vai vairāk nekā 30 ziņojumi minūtē.</span><span class="sxs-lookup"><span data-stu-id="f651f-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="f651f-107">Kad tiek palaista darbplūsma, e-pasta ziņa nav nosūtīta un pamanāt kļūdas ziņojumu, iekšējais statuss ir iestatīts uz ir parādīts atliktās vai nevar nosūtīt adresātam.</span><span class="sxs-lookup"><span data-stu-id="f651f-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="f651f-108">Lai iegūtu papildinformāciju, skatiet šādu [pantu](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="f651f-108">For more information, please refer to the following [article](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

