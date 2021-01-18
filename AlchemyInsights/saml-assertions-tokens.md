---
title: SAML apgalvojumi (marķieri)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885681"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="ebb7c-102">SAML apgalvojumi (marķieri)</span><span class="sxs-lookup"><span data-stu-id="ebb7c-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="ebb7c-103">Drošības apgalvojumu atzīmju valodas (SAML) marķierierīces ir XML atspoguļojums prasībās.</span><span class="sxs-lookup"><span data-stu-id="ebb7c-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="ebb7c-104">Pēc noklusējuma SAML marķieri Windows Communication Foundation (WCF) izmanto Federatīvajās drošības scenārijos ir izdotas marķieri.</span><span class="sxs-lookup"><span data-stu-id="ebb7c-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="ebb7c-105">Papildinformāciju skatiet rakstā [SAML marķieri un prasības](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="ebb7c-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="ebb7c-106">Microsoft Identity Platform izstaro vairāku veidu drošības marķierus katras autentifikācijas plūsmas apstrādē.</span><span class="sxs-lookup"><span data-stu-id="ebb7c-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="ebb7c-107">[SAML marķiera norāžu atsauce](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) apraksta SAML 2,0 marķieru formātu, drošības raksturlielumus un saturu.</span><span class="sxs-lookup"><span data-stu-id="ebb7c-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="ebb7c-108">Lai izprastu, kā konfigurēt marķierierīces ilgumus, izpildiet norādījumus [konfigurējamas marķierierīces kalpošanas laikā Microsoft Identity platformā](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) .</span><span class="sxs-lookup"><span data-stu-id="ebb7c-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="ebb7c-109">Izpildiet [šajā rakstā](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) norādītās darbības, lai uzzinātu, kā konfigurēt AZURE ad SAML marķierierīces šifrēšanu.</span><span class="sxs-lookup"><span data-stu-id="ebb7c-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="ebb7c-110">Azure AD varat iestatīt sertifikāta parakstīšanas opcijas un sertifikāta parakstīšanas algoritmu.</span><span class="sxs-lookup"><span data-stu-id="ebb7c-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="ebb7c-111">Lai iegūtu papildinformāciju, skatiet rakstu [papildu sertifikāta parakstīšanas opcijas SAML pilnvarā par Gallery programmām Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="ebb7c-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
