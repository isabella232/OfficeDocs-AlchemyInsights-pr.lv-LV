---
title: S/MIME programmā Outlook Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053232"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="cd1ea-102">E-pasta ziņojumu šifrēšana programmā Outlook</span><span class="sxs-lookup"><span data-stu-id="cd1ea-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="cd1ea-103">Office 365 ziņojumu šifrēšana ir veidota uz Microsoft Azure Rights Management (Azure RMS), kas ir daļa no Azure informācijas aizsardzības.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="cd1ea-104">Ja abonementā ir iekļauta Azure Rights Management vai Azure informācijas aizsardzība, **nav jāveic nekādas darbības, lai manuāli iespējotu vai aktivizētu** tiesību pārvaldības pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="cd1ea-105">Pamatojoties uz klientu atsauksmēm, mēs vairs neiespējosim Exchange pasta plūsmas kārtulas, lai automātiski šifrētu izejošo e-pastu, kurā ir noteikta veida sensitīva informācija jūsu nomniekā pēc noklusējuma.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="cd1ea-106">Tā vietā mēs sniedzam detalizētas instrukcijas par to, kā jūs to varat izdarīt paši.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="cd1ea-107">Lai iegūtu papildinformāciju par to, kā izveidot transporta kārtulu, lai šifrētu konfidenciālu informāciju, skatiet [šo rakstu](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="cd1ea-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="cd1ea-108">Ja izmantojat Outlook Web (iepriekš **OWA**): sastādot e-pasta ziņojumu, vienkārši noklikšķiniet uz **aizsargāt** OWA.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="cd1ea-109">Tas attieksies "nav uz priekšu" atļauju.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="cd1ea-110">Noklikšķiniet uz **mainīt atļauju** un izvēlieties **Šifrēt** , lai tikai šifrētu ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="cd1ea-111">Ja **Outlook klienta**izmantošana: lai sūtītu šifrētu ziņojumu no programmas Outlook 2013 vai 2016 vai Outlook 2016 operētājsistēmai Mac, atlasiet **opciju** > **atļaujas**, pēc tam atlasiet nepieciešamo aizsardzības opciju.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="cd1ea-112">Lai **automātiski šifrētu visus e-pasta** ziņojumus, kas nosūtīti noteiktiem adresātiem vai ārējo partneru organizācijām, jums ir jāizveido pasta plūsmas transportēšanas kārtula Exchange administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="cd1ea-113">Detalizētas instrukcijas ir sniegtas [šajā atbalsta rakstā](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="cd1ea-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

