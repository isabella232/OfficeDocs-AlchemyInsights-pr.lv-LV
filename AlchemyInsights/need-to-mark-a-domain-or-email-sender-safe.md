---
title: Vai vēlaties atzīmēt, ka domēns vai e-pasta sūtītājs ir drošībā?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803252"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="94530-102">Vai vēlaties atzīmēt, ka domēns vai e-pasta sūtītājs ir drošībā?</span><span class="sxs-lookup"><span data-stu-id="94530-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="94530-103">**Drošo sūtītāju sarakstu izmantošana nav ieteicama** , jo tā atver jūsu organizāciju surogātpasta, adresi phish un izlikšanās uzbrukumiem.</span><span class="sxs-lookup"><span data-stu-id="94530-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="94530-104">Tomēr, ja pastāv biznesa prasība, **iesakām izmantot** **[pasta plūsmas kārtulas](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .</span><span class="sxs-lookup"><span data-stu-id="94530-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="94530-105">Mūsu norādījumi nodrošina sūtītāja autentifikāciju (pārbauda, vai sūtītais domēns netiek viltots).</span><span class="sxs-lookup"><span data-stu-id="94530-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="94530-106">**Piezīme**: neiesakām pārvaldīt viltus pozitīvos, izmantojot drošo sūtītāju sarakstus, jo surogātpasta filtrēšanas izņēmumi var atvērt jūsu organizāciju drošības uzbrukumiem.</span><span class="sxs-lookup"><span data-stu-id="94530-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="94530-107">Ja jūsu lietotājs (i) saņem ziņojumus, kas nepareizi atzīmēti kā surogātpasts vai Nevēlamais e-pasts, lūdzu, **[Ziņojiet par ziņojumiem un failiem korporācijai Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="94530-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="94530-108">Ir **jāizvairās no** drošo sūtītāju saraksta programmā Outlook, atļauto sūtītāju sarakstā vai atļauto domēnu sarakstā surogātpasta novēršanas politikā, jo sūtītāji apiet visu surogātpasta, mānīšanās un adresi phish aizsardzību un sūtītāja AUTENTIFIKĀCIJU (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="94530-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="94530-109">Šo metodi ieteicams izmantot tikai pagaidu pārbaudei.</span><span class="sxs-lookup"><span data-stu-id="94530-109">This method is best used for temporary testing only.</span></span>
