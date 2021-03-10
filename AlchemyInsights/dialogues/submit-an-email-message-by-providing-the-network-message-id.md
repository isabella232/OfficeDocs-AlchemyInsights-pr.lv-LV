---
title: E-pasta ziņojuma iesniegšana, norādot tīkla ziņojuma ID
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693914"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="d753c-102">E-pasta ziņojuma iesniegšana, norādot tīkla ziņojuma ID</span><span class="sxs-lookup"><span data-stu-id="d753c-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="d753c-103">**Jaunajā iesniegšanas** izlidošanas lodziņā atlasiet **e-pasta** un **tīkla ziņojuma ID**.</span><span class="sxs-lookup"><span data-stu-id="d753c-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="d753c-104">Veiciet šīs darbības, lai atrastu ziņojuma ID e-pasta ziņojumam programmā Outlook:</span><span class="sxs-lookup"><span data-stu-id="d753c-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="d753c-105">Veiciet dubultklikšķi uz e-pasta ziņojuma, lai to atvērtu.</span><span class="sxs-lookup"><span data-stu-id="d753c-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="d753c-106">Atlasiet **faila**  >  **Rekvizīti**.</span><span class="sxs-lookup"><span data-stu-id="d753c-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="d753c-107">Atveriet Piezīmjbloku vai tukšu Word dokumentu un pēc tam nokopējiet un ielīmējiet to saturu, kas ir atrodams lodziņā **interneta galvenes** , uz atvērtu dokumentu, lai iegūtu labāku redzamību.</span><span class="sxs-lookup"><span data-stu-id="d753c-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="d753c-108">Atrodiet **X-MS-Exchange-Organization-Network-Message-ID** lauku.</span><span class="sxs-lookup"><span data-stu-id="d753c-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="d753c-109">Vērtība pēc **:** atbilst jūsu iesniegtajam ID.</span><span class="sxs-lookup"><span data-stu-id="d753c-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="d753c-110">Sadaļā **adresāti**, ja e-pasta ziņojums ir izkrauts mapē Nevēlamais e-pasts visiem šī e-pasta adresātiem, izvēlieties **Atlasīt visu**.</span><span class="sxs-lookup"><span data-stu-id="d753c-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="d753c-111">Ja nav, atlasiet tikai to lietotāju, kurš ziņoja par šo problēmu.</span><span class="sxs-lookup"><span data-stu-id="d753c-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="d753c-112">Ja atlasāt, ir **jābūt bloķētam** **iesniegšanas iemeslam**, norādiet, vai ziņojumam ir jābūt bloķētam kā **surogātpasts**, **Pikšķerēšana** vai **ļaunprogrammatūra**, un pēc tam atlasiet **iesniegt**.</span><span class="sxs-lookup"><span data-stu-id="d753c-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="d753c-113">Lai uzzinātu vairāk, skatiet rakstu [kā programmā Microsoft meklēt aizdomīgus surogātpasta, adresi phish, vietrāžus URL un failus](https://go.microsoft.com/fwlink/?linkid=2101479).</span><span class="sxs-lookup"><span data-stu-id="d753c-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
