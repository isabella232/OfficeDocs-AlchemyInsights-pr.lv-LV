---
title: Marķierierīces ilguma konfigurēšana un pagarināšana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917004"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="9c836-102">Marķierierīces ilguma konfigurēšana un pagarināšana</span><span class="sxs-lookup"><span data-stu-id="9c836-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="9c836-103">Varat norādīt, kāda ir Access, SAML vai ID pilnvara, ko izsniedz Microsoft Identity Platform.</span><span class="sxs-lookup"><span data-stu-id="9c836-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="9c836-104">Varat iestatīt token mūžus visās programmās savā organizācijā, vairāku nomnieku (vairāku organizāciju) lietojumprogrammai vai konkrētam pakalpojumu pilnvarotājam jūsu organizācijā.</span><span class="sxs-lookup"><span data-stu-id="9c836-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="9c836-105">Lai iegūtu papildinformāciju, izlasiet [konfigurējamas marķierierīces ilgumus](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="9c836-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="9c836-106">Piemēram, izlasiet [piemērus par to, kā konfigurēt marķierierīces ilgumu](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="9c836-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="9c836-107">Lai uzzinātu, kā konfigurēt marķiera mūžu un saderību Azure Active Directory B2C (Azure AD B2C), skatiet rakstu [tokens konfigurēšana Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="9c836-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="9c836-108">Rakstā [sesijas darbības konfigurēšana Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) apraksta vienotās pierakstīšanās (SSO) metodēs, ko izmanto AZURE ad B2C, un palīdz izvēlēties piemērotāko SSO metodi, konfigurējot politiku.</span><span class="sxs-lookup"><span data-stu-id="9c836-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="9c836-109">**Cik ilgi žetoni ir pēdējie? Cik ilgi tie ir derīgi?**</span><span class="sxs-lookup"><span data-stu-id="9c836-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="9c836-110">Token kalpošanas ilgums ir 1 stunda un sesijas ilgums ir 24 stundas.</span><span class="sxs-lookup"><span data-stu-id="9c836-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="9c836-111">Tas nozīmē, ka, ja pieprasījumi nav veikti 24 stundās, jums ir atkārtoti jāpiesakās, lai tiktu pieprasīta jauna pilnvara.</span><span class="sxs-lookup"><span data-stu-id="9c836-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="9c836-112">Pēc 30. maija 2020 neviens jaunais nomnieks nevarēs izmantot konfigurējamu marķierierīces kalpošanas ilgumu, lai konfigurētu sesijas un atsvaidzināšanas marķierus.</span><span class="sxs-lookup"><span data-stu-id="9c836-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="9c836-113">Novecošana notiks vairāku mēnešu laikā pēc tam, kas nozīmē, ka mēs pārstām ievērot pašreizējo sesiju un atsvaidzināt marķierus.</span><span class="sxs-lookup"><span data-stu-id="9c836-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="9c836-114">Jūs joprojām varat konfigurēt piekļuves pilnvaru ilgumu pēc izslēgšanas.</span><span class="sxs-lookup"><span data-stu-id="9c836-114">You can still configure access token lifetimes after the deprecation.</span></span>






