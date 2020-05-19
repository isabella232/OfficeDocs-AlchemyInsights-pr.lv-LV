---
title: Vai ir nepieciešams atzīmēt domēnu vai e-pasta sūtītāju kā drošu?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281178"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="483ce-102">Vai ir nepieciešams atzīmēt domēnu vai e-pasta sūtītāju kā drošu?</span><span class="sxs-lookup"><span data-stu-id="483ce-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="483ce-103">**Drošo sūtītāju sarakstu** izmantošana nav ieteicama, jo tā atver jūsu organizācijai surogātpastu, phish un izlikšanās uzbrukumiem.</span><span class="sxs-lookup"><span data-stu-id="483ce-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="483ce-104">Tomēr, ja ir biznesa prasības, **ieteicams izmantot** **[pasta plūsmas kārtulas](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .</span><span class="sxs-lookup"><span data-stu-id="483ce-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="483ce-105">Mūsu norādījumi nodrošina sūtītāja autentifikāciju (pārbauda sūtīšanas domēns netiek viltoti).</span><span class="sxs-lookup"><span data-stu-id="483ce-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="483ce-106">**Piezīme**: nav ieteicams pārvaldīt viltus pozitīvi, izmantojot drošo sūtītāju sarakstus, jo surogātpasta filtrēšanas izņēmumi var atvērt jūsu organizācijas drošības uzbrukumiem.</span><span class="sxs-lookup"><span data-stu-id="483ce-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="483ce-107">Ja jūsu lietotājs (i) saņem ziņojumus, kas nepareizi atzīmēti kā surogātpasts vai Nevēlamais e-pasts, lūdzu, **[ziņojiet par ziņojumiem un failiem korporācijai Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="483ce-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="483ce-108">Droši sūtītāji programmā Outlook, atļauto sūtītāju sarakstā vai atļauto domēnu sarakstā pretsurogātpasta politikā **ir jāizvairās** , jo sūtītāji apiet visus surogātpastu, mānību, un phish aizsardzību un sūtītāja AUTENTIFIKĀCIJU (SPF, DKIM, dmarc).</span><span class="sxs-lookup"><span data-stu-id="483ce-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="483ce-109">Šo metodi ieteicams izmantot tikai pagaidu testēšanai.</span><span class="sxs-lookup"><span data-stu-id="483ce-109">This method is best used for temporary testing only.</span></span>
