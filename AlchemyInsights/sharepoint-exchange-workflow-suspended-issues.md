---
title: Darba sākšana ar SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700714"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="5a69f-102">Darbplūsmas pakalpojumā SharePoint</span><span class="sxs-lookup"><span data-stu-id="5a69f-102">Workflows in SharePoint</span></span>

<span data-ttu-id="5a69f-103">Ja SharePoint darbplūsmas nesūta e-pasta ziņojumus, iespējams, jūsu organizācijai ir radušies Exchange Online sūtītāja ierobežojumi.</span><span class="sxs-lookup"><span data-stu-id="5a69f-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="5a69f-104">Ja jums ir kāds no šiem vienumiem, tiek parādīts kļūdas ziņojums "darbplūsma ir aizturēta".</span><span class="sxs-lookup"><span data-stu-id="5a69f-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="5a69f-105">Jums ir SharePoint Online darbplūsma, kas izmanto SharePoint 2010 vai SharePoint 2013 darbplūsmas platformas tipu.</span><span class="sxs-lookup"><span data-stu-id="5a69f-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="5a69f-106">Darbplūsma ir konfigurēta, lai vienlaikus nosūtītu pielāgotu e-pasta ziņojumu vairāk nekā 200 lietotājiem, vairāk nekā 10 000 adresātiem dienā vai vairāk nekā 30 ziņojumiem minūtē.</span><span class="sxs-lookup"><span data-stu-id="5a69f-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="5a69f-107">Palaižot darbplūsmu, netiek nosūtīts e-pasta ziņojums, un tiek parādīts kļūdas ziņojums, iekšējais statuss tiek iestatīts uz apturēts vai nevar nosūtīt adresātam.</span><span class="sxs-lookup"><span data-stu-id="5a69f-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="5a69f-108">Lai iegūtu papildinformāciju, lūdzu, skatiet šo [rakstu](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="5a69f-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

