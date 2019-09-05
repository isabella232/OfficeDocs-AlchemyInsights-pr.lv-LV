---
title: Darba sākšana ar SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 4c0220dd2535a1ef41aeef99e2bfc3fe28bac03a
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751679"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="ef9c1-102">Darbplūsmas SharePoint</span><span class="sxs-lookup"><span data-stu-id="ef9c1-102">Workflows in SharePoint</span></span>

<span data-ttu-id="ef9c1-103">Ja SharePoint darbplūsmas nesūta e-pasta ziņojumus, jūsu uzņēmums var būt saskāries ar Exchange Online sūtītāja ierobežojumus.</span><span class="sxs-lookup"><span data-stu-id="ef9c1-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="ef9c1-104">"Darbplūsma ir apturēta" kļūdas ziņojums var rasties, ja jums ir kāds no šiem vienumiem:</span><span class="sxs-lookup"><span data-stu-id="ef9c1-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="ef9c1-105">Jums ir darbplūsma SharePoint Online, kas izmanto SharePoint 2010 vai SharePoint 2013 darbplūsmas platformas tips.</span><span class="sxs-lookup"><span data-stu-id="ef9c1-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="ef9c1-106">Darbplūsma ir konfigurēta, lai nosūtītu pielāgotu e-pasta ziņojumu vairāk nekā 200 lietotājiem laikā, vairāk nekā 10 000 adresāti dienā vai vairāk nekā 30 ziņojumi minūtē.</span><span class="sxs-lookup"><span data-stu-id="ef9c1-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="ef9c1-107">Palaižot darbplūsmu, e-pasta ziņojums netiek nosūtīts un pamanāt kļūdas ziņojumu, iekšējais statuss ir iestatīts uz apturēta vai nevar nosūtīt adresātam tiek parādīts.</span><span class="sxs-lookup"><span data-stu-id="ef9c1-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="ef9c1-108">Lai iegūtu papildinformāciju, lūdzu, skatiet šo [rakstu](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="ef9c1-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

