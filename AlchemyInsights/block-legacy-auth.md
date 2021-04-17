---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820185"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="99f10-102">Mantotās autentifikācijas bloķēšana</span><span class="sxs-lookup"><span data-stu-id="99f10-102">Blocking legacy authentication</span></span>

<span data-ttu-id="99f10-103">Mantotā autentifikācija ir termins, kas attiecas uz autentifikācijas pieprasījumu, ko veicis:</span><span class="sxs-lookup"><span data-stu-id="99f10-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="99f10-104">Vecāki Office klienti, kuri neizmanto moderno autentifikāciju (piemēram, Office 2010 klients).</span><span class="sxs-lookup"><span data-stu-id="99f10-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="99f10-105">Jebkurš klients, kas izmanto mantotos pasta protokolus, piemēram, IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="99f10-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="99f10-106">Papildinformāciju par mantotās autentifikācijas bloķēšanu un modernās autentifikācijas iespējošanu skatiet sadaļā [Mantotās autentifikācijas bloķēšana.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="99f10-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="99f10-107">Drošības noklusējuma iestatījumi pakalpojumā Azure Active Directory (Azure AD) atvieglo drošību un palīdz aizsargāt jūsu organizāciju.</span><span class="sxs-lookup"><span data-stu-id="99f10-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="99f10-108">Drošības noklusējuma iestatījumos ir iepriekš konfigurēti bieži sastopamu uzbrukumu drošības iestatījumi.</span><span class="sxs-lookup"><span data-stu-id="99f10-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="99f10-109">Papildinformāciju par drošības noklusējuma iestatījumiem skatiet sadaļā [Kas ir drošības noklusējuma iestatījumi?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="99f10-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="99f10-110">**Piezīme.** Ja jūsu nomnieks tika izveidots 2019. gada 22. oktobrī vai pēc tā, iespējams, ir radusies jaunā, pēc noklusējuma drošā darbība un jūsu nomniekā jau ir iespējotas drošības noklusējuma vērtības.</span><span class="sxs-lookup"><span data-stu-id="99f10-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="99f10-111">Lai aizsargātu visus mūsu lietotājus, drošības noklusējuma iestatījumi tiek lietoti visiem jaunajiem nomniekiem.</span><span class="sxs-lookup"><span data-stu-id="99f10-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
