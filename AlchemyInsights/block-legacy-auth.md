---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685605"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="a5711-102">Mantotās autentifikācijas bloķēšana</span><span class="sxs-lookup"><span data-stu-id="a5711-102">Blocking legacy authentication</span></span>

<span data-ttu-id="a5711-103">Mantotā autentifikācija ir termins, kas attiecas uz autentifikācijas pieprasījumu, ko veicis:</span><span class="sxs-lookup"><span data-stu-id="a5711-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="a5711-104">Vecāki Office klienti, kas neizmanto moderno autentifikāciju (piemēram, Office 2010 klients).</span><span class="sxs-lookup"><span data-stu-id="a5711-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="a5711-105">Jebkurš klients, kas izmanto iepriekšējās paaudzes pasta protokolus, piemēram, IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="a5711-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="a5711-106">Papildinformāciju par mantotās autentifikācijas bloķēšanu un modernās autentifikācijas iespējošanu skatiet sadaļā [mantotās autentifikācijas bloķēšana](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="a5711-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="a5711-107">Drošības noklusējumi Azure Active Directory (Azure AD) palīdz padarīt drošību un palīdzēt aizsargāt jūsu organizāciju.</span><span class="sxs-lookup"><span data-stu-id="a5711-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="a5711-108">Drošības noklusējumos ir iepriekš konfigurēti drošības iestatījumi biežiem uzbrukumiem.</span><span class="sxs-lookup"><span data-stu-id="a5711-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="a5711-109">Papildinformāciju par drošības noklusējumiem skatiet sadaļā [kas ir drošības noklusējumi?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="a5711-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="a5711-110">**Piezīme**. Ja jūsu nomnieks ir izveidots vai pēc 22. oktobra, 2019, ir iespējams, ka jums ir jauna drošā izturēšanās, un jau ir iespējots drošības noklusējums jūsu nomniekā.</span><span class="sxs-lookup"><span data-stu-id="a5711-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="a5711-111">Lai aizsargātu visus mūsu lietotājus, tiek izveidoti drošības noklusējumi visiem jaunajiem nomniekiem.</span><span class="sxs-lookup"><span data-stu-id="a5711-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
