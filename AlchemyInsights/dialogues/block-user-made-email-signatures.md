---
title: Lietotāja veikto e-pasta parakstu bloķēšana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243627"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="3b058-102">Lietotāja veikto e-pasta parakstu bloķēšana</span><span class="sxs-lookup"><span data-stu-id="3b058-102">Block user-made email signatures</span></span>

<span data-ttu-id="3b058-103">Šis risinājums attiecas tikai uz e-pasta parakstiem, kas izveidoti programmā Outlook tīmeklī.</span><span class="sxs-lookup"><span data-stu-id="3b058-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="3b058-104">Jūs varat bloķēt parakstus tikai programmā Outlook, ja jums ir lokāls Exchange serveris.</span><span class="sxs-lookup"><span data-stu-id="3b058-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="3b058-105">Administrēšanas centrā izvēlieties **administrēšanas centru**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="3b058-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="3b058-106">Noklikšķiniet uz **atļaujas**  >  **Outlook Web App politikas**.</span><span class="sxs-lookup"><span data-stu-id="3b058-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="3b058-107">Atlasiet politiku un pēc tam noklikšķiniet uz zīmuļa ikonas, lai to rediģētu.</span><span class="sxs-lookup"><span data-stu-id="3b058-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="3b058-108">Noklikšķiniet **uz**  >  **Papildu opcijas**.</span><span class="sxs-lookup"><span data-stu-id="3b058-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="3b058-109">Sadaļā **lietotāja pieredze** notīriet izvēles rūtiņu **e-pasta paraksts** un pēc tam noklikšķiniet uz **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="3b058-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="3b058-110">**Svarīgi!** Ja paraksts ir pievienots pirms šīs izvēles rūtiņas notīrīšanas, lietotājs to joprojām varēs izmantot.</span><span class="sxs-lookup"><span data-stu-id="3b058-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="3b058-111">Lūdziet to noņemt.</span><span class="sxs-lookup"><span data-stu-id="3b058-111">Ask them to remove it.</span></span>