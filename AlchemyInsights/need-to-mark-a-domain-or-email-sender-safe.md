---
title: Vai vēlaties atzīmēt domēnu vai e-pasta sūtītāju kā drošu?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792139"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="447c2-102">Vai vēlaties atzīmēt domēnu vai e-pasta sūtītāju kā drošu?</span><span class="sxs-lookup"><span data-stu-id="447c2-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="447c2-103">Drošo **sūtītāju sarakstu izmantošana nav ieteicama,** jo tādējādi jūsu organizācija tiek atvērta surogātpasta, pikšķerēšanas un izlikšanās uzbrukumiem.</span><span class="sxs-lookup"><span data-stu-id="447c2-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="447c2-104">Tomēr, ja ir biznesa prasības, iesakām **šim nolūkam** **[izmantot pasta](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** plūsmas kārtulas.</span><span class="sxs-lookup"><span data-stu-id="447c2-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="447c2-105">Mūsu norādījumi nodrošina, ka sūtītāja autentifikācija (verificē domēna sūtīšanu netiek izlikšanās).</span><span class="sxs-lookup"><span data-stu-id="447c2-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="447c2-106">**Piezīme.** Nav ieteicams pārvaldīt aplami pozitīvos ziņojumus, izmantojot drošo sūtītāju sarakstus, jo surogātpasta filtrēšanas izņēmumi var atvērt jūsu organizāciju drošības uzbrukumiem.</span><span class="sxs-lookup"><span data-stu-id="447c2-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="447c2-107">Ja lietotājs(i) saņem ziņojumus, kas nepareizi atzīmēti kā surogātpasts vai nevēlamais e-pasts, lūdzu, ziņojiet par **[ziņojumiem un failiem korporācijai Microsoft.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="447c2-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="447c2-108">Ir jāizvairās no drošiem sūtītājiem programmā Outlook, atļauto  sūtītāju sarakstam vai atļautajiem domēnu sarakstiem pretsurogātpasta politikās, jo sūtītāji apiet visu surogātpastu, izlikšanās un pikšķerēšanas aizsardzību, kā arī sūtītāju autentifikāciju (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="447c2-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="447c2-109">Šo metodi ir vislabāk izmantot tikai pagaidu testēšanai.</span><span class="sxs-lookup"><span data-stu-id="447c2-109">This method is best used for temporary testing only.</span></span>
