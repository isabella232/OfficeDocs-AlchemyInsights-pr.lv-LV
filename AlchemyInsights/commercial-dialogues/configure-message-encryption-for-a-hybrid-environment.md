---
title: Ziņojumu šifrēšanas konfigurēšana hibrīdajai videi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745398"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="e36da-102">Ziņojumu šifrēšanas konfigurēšana hibrīdajai videi</span><span class="sxs-lookup"><span data-stu-id="e36da-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="e36da-103">Hibrīdajām Exchange vidēm Lokālie lietotāji var sūtīt šifrētus e-pasta ziņojumus, izmantojot Office ziņojumu šifrēšanu (OME) tikai tad, ja e-pasts tiek maršrutēts, izmantojot Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="e36da-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="e36da-104">Lai šifrētu e-pasta ziņojumus, izmantojot OME, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="e36da-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="e36da-105">Izmantojiet [hibrīdās konfigurācijas vedni](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) , lai iestatītu hibrīdo vidi.</span><span class="sxs-lookup"><span data-stu-id="e36da-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="e36da-106">Nav nepieciešamas īpašas darbības, lai iestatītu šifrēšanu.</span><span class="sxs-lookup"><span data-stu-id="e36da-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="e36da-107">[Iestatiet pasta plūsmas kārtulas šifrēšanai](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) tāpat kā parasti.</span><span class="sxs-lookup"><span data-stu-id="e36da-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


