---
title: S/MIME programmā Outlook tīmeklī
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772305"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="b6c44-102">E-pasta ziņojumu šifrēšana programmā Outlook</span><span class="sxs-lookup"><span data-stu-id="b6c44-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="b6c44-103">Microsoft 365 ziņojumu šifrēšana ir veidota Microsoft Azure Rights Management (Azure RMS), kas ir Azure Information Protection daļa.</span><span class="sxs-lookup"><span data-stu-id="b6c44-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="b6c44-104">Ja jūsu abonementā ir iekļauta Azure Rights Management vai Azure Information Protection, **jums nav jāveic nekādas darbības, lai manuāli iespējotu vai aktivizētu** tiesību pārvaldības pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="b6c44-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="b6c44-105">Ņemot vērā klientu atsauksmes, mēs vairs neiespējojam Exchange pasta plūsmas kārtulas, lai automātiski šifrētu izejošos e-pasta ziņojumus, kuros nomniekā ir noteikta veida konfidenciāla informācija.</span><span class="sxs-lookup"><span data-stu-id="b6c44-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="b6c44-106">Tā vietā mēs sniedzam detalizētus norādījumus par to, kā varat to izdarīt pats.</span><span class="sxs-lookup"><span data-stu-id="b6c44-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="b6c44-107">Papildinformāciju par to, kā izveidot transporta kārtulu, lai šifrētu sensitīvu informāciju, skatiet [šajā rakstā](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="b6c44-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="b6c44-108">Ja izmantojat Outlook tīmeklī (iepriekš **OWA**): veidojot e-pasta ziņojumu, vienkārši noklikšķiniet uz **aizsargāt** OWA.</span><span class="sxs-lookup"><span data-stu-id="b6c44-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="b6c44-109">Tas attieksies uz "Nepārsūtīt" atļauju.</span><span class="sxs-lookup"><span data-stu-id="b6c44-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="b6c44-110">Noklikšķiniet uz **mainīt atļaujas** un izvēlieties **Šifrēt** , lai šifrētu tikai šo ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="b6c44-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="b6c44-111">Ja izmantojat **Outlook klientu**: lai nosūtītu šifrētu ziņojumu no programmas Outlook 2013 vai 2016, vai Outlook 2016 darbam ar Mac, atlasiet **opciju**  >  **atļaujas**un pēc tam atlasiet vajadzīgo aizsardzības opciju.</span><span class="sxs-lookup"><span data-stu-id="b6c44-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="b6c44-112">Lai **automātiski šifrētu visus e-pasta** ziņojumus, kas nosūtīti konkrētiem adresātiem vai ārējām partnera organizācijām, ir jāizveido pasta plūsmas transportēšanas kārtula Exchange administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="b6c44-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="b6c44-113">Detalizēti norādījumi ir sniegti [šajā atbalsta rakstā](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="b6c44-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

