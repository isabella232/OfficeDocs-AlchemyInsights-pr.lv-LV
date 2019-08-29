---
title: S/MIME programmā Outlook Web
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666847"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="d0cb8-102">Šifrētu e-pasta ziņojumus programmā Outlook</span><span class="sxs-lookup"><span data-stu-id="d0cb8-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="d0cb8-103">365 biroja ziņojumu šifrēšana ir veidota uz Microsoft Azure piekļuves tiesību pārvaldība (Azure RMS), kas ir daļa no Azure informācijas aizsardzību.</span><span class="sxs-lookup"><span data-stu-id="d0cb8-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="d0cb8-104">Ja jūsu abonements ietver debeszils tiesību pārvaldību vai Azure informācijas aizsardzību, **jums nav nepieciešams veikt jebkādas darbības, lai manuāli jāiespējo vai aktivizēt** tiesību pārvaldības pakalpojums.</span><span class="sxs-lookup"><span data-stu-id="d0cb8-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="d0cb8-105">Pamatojoties uz klientu atsauksmēm, mēs būs vairs būt dodot Exchange pasta plūsmas kārtulas, lai automātiski Šifrēt izejošo e-pastu, kurā noteikta veida konfidenciālu informāciju jūsu īrnieks pēc noklusējuma.</span><span class="sxs-lookup"><span data-stu-id="d0cb8-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="d0cb8-106">Tā vietā mēs sniedzam detalizētas instrukcijas par to, kā varat to izdarīt paši.</span><span class="sxs-lookup"><span data-stu-id="d0cb8-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="d0cb8-107">Papildu informāciju par to, kā izveidot transporta kārtulu, lai šifrētu sensitīvu informāciju, izlasiet [šo rakstu](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="d0cb8-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="d0cb8-108">Ja izmantojat Outlook Web (agrāk **OWA**): sastādot e-pasta ziņojumu, vienkārši noklikšķiniet uz **aizsargāt** programmā OWA.</span><span class="sxs-lookup"><span data-stu-id="d0cb8-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="d0cb8-109">Tas attieksies atļauja "Nepārsūtīt".</span><span class="sxs-lookup"><span data-stu-id="d0cb8-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="d0cb8-110">Noklikšķiniet uz **mainīt atļaujas** un izvēlieties **Šifrēt** tikai šifrētu ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="d0cb8-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="d0cb8-111">Ja lietojat **Outlook klients**: lai nosūtītu šifrētu ziņojumu no Outlook 2013 vai 2016 vai Outlook 2016 Mac, izvēlieties **iespējas** > **atļaujas**un pēc tam atlasiet aizsardzības iespēja, kas jums nepieciešams.</span><span class="sxs-lookup"><span data-stu-id="d0cb8-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="d0cb8-112">**Automātiski šifrēt visu e-pastu** nosūtīja uz noteiktiem saņēmējiem vai ārējo partneru organizācijām, jums ir nepieciešams, lai izveidotu pasta plūsmu transporta kārtulas Exchange administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="d0cb8-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="d0cb8-113">[Atbalsta rakstā](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)sniegtas detalizētas instrukcijas.</span><span class="sxs-lookup"><span data-stu-id="d0cb8-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

