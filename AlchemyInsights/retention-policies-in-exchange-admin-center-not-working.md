---
title: Saglabāšanas politikas Exchange administrēšanas centrā nedarbojas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952235"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="d1ff1-102">Saglabāšanas politikas Exchange administrēšanas centrā</span><span class="sxs-lookup"><span data-stu-id="d1ff1-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="d1ff1-103">Ja vēlaties, lai mēs automatizēti veiktu tālāk minēto iestatījumu pārbaudes, atlasiet pogu Atpakaļ <- šīs lapas augšdaļā un pēc tam ievadiet tā lietotāja e-pasta adresi, kuram ir problēmas ar saglabāšanas politikām.</span><span class="sxs-lookup"><span data-stu-id="d1ff1-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="d1ff1-104">Ja rodas problēmas ar saglabāšanas politikām Exchange administrēšanas centrā, kas netiek lietots pastkastēm vai vienumiem, kas nepārvieto uz arhīva pastkasti, pārbaudiet šādus elementus:</span><span class="sxs-lookup"><span data-stu-id="d1ff1-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="d1ff1-105">**Saknes iemesli:**</span><span class="sxs-lookup"><span data-stu-id="d1ff1-105">**Root Causes:**</span></span>

- <span data-ttu-id="d1ff1-106">**Pārvaldītais mapes** palīgs nav apstrādājis lietotāja pastkasti.</span><span class="sxs-lookup"><span data-stu-id="d1ff1-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="d1ff1-107">Pārvaldīto mapju palīgs ik pēc septiņām dienām mēģina apstrādāt katru pastkasti jūsu mākoņa organizācijā.</span><span class="sxs-lookup"><span data-stu-id="d1ff1-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="d1ff1-108">**Risinājums:** Palaidiet pārvaldīto mapju palīgu.</span><span class="sxs-lookup"><span data-stu-id="d1ff1-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="d1ff1-109">Pastkastē ir **iespējota opcija** **RetentionHold.**</span><span class="sxs-lookup"><span data-stu-id="d1ff1-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="d1ff1-110">Ja pastkaste ir novietota saglabāšanas vietā, saglabāšanas politika pastkastē šajā laikā netiks apstrādāta.</span><span class="sxs-lookup"><span data-stu-id="d1ff1-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="d1ff1-111">**Risinājums:** Pārbaudiet saglabāšanas aizturēšanas iestatījuma statusu un atjauniniet pēc nepieciešamības.</span><span class="sxs-lookup"><span data-stu-id="d1ff1-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="d1ff1-112">Detalizētu informāciju skatiet rakstā [Pastkastes saglabāšanas aizturēšana.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="d1ff1-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="d1ff1-113">**Piezīme.** Ja pastkaste ir mazāka par 10 MB, pārvaldīto mapju palīgs automātiski neapstrādā pastkasti.</span><span class="sxs-lookup"><span data-stu-id="d1ff1-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="d1ff1-114">Papildinformāciju par saglabāšanas politikām Exchange administrēšanas centrā skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="d1ff1-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="d1ff1-115">Saglabāšanas atzīmes un saglabāšanas politikas</span><span class="sxs-lookup"><span data-stu-id="d1ff1-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="d1ff1-116">[Saglabāšanas politikas izmantošana pastkastēm vai Saglabāšanas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [tagu pievienošana vai noņemšana](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="d1ff1-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="d1ff1-117">Pastkastes aizturēšanas veida identificēšana</span><span class="sxs-lookup"><span data-stu-id="d1ff1-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
