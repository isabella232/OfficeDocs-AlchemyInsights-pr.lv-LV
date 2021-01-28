---
title: Problēmas ar token prasībām un atribūtiem
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035965"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="e9971-102">Problēmas ar token prasībām un atribūtiem</span><span class="sxs-lookup"><span data-stu-id="e9971-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="e9971-103">**Apliecinājuma prasību atjaunināšana, konfigurēšana un noņemšana**</span><span class="sxs-lookup"><span data-stu-id="e9971-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="e9971-104">Izmantojot Azure Active Directory (Azure AD), varat [pielāgot pieprasījuma tipu lomai](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) , kas saņemta pēc tam, kad esat autorizējis programmu.</span><span class="sxs-lookup"><span data-stu-id="e9971-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="e9971-105">Lietojumprogrammu izstrādātāji var izmantot neobligātas prasības to Azure AD lietojumprogrammās, lai norādītu, kuras prasības tās vēlas piešķirt.</span><span class="sxs-lookup"><span data-stu-id="e9971-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="e9971-106">Lai iegūtu papildinformāciju, skatiet rakstu [kā sniegt neobligātus pieprasījumus savai programmai](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="e9971-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="e9971-107">[Konfigurējiet grupu pieprasījumus pakalpojumam Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="e9971-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="e9971-108">Ja lietojumprogrammā izmantojat nemanāmu vienoto pierakstīšanos, skatiet rakstu [SAML pilnvarā izsniegto prasību pielāgošana Enterprise lietojumprogrammām](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="e9971-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="e9971-109">**Pretenziju atribūtu kartēšana**</span><span class="sxs-lookup"><span data-stu-id="e9971-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="e9971-110">Lai konfigurētu pieprasījumu kartēšanas politikas izmantošanu, izmantojot PowerShell, skatiet rakstu kā noteiktās [programmas nomniekā (priekšskatījums) pielāgotās prasības](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="e9971-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="e9971-111">Direktorija shēmas paplašinājuma atribūti nodrošina veidu, kā glabāt papildu datus Azure Active Directory lietotāju objektos un citos direktorija objektos, piemēram, grupās, nomnieka informācijā, pakalpojumu principālos.</span><span class="sxs-lookup"><span data-stu-id="e9971-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="e9971-112">Tikai lietotāja objektu paplašinājuma atribūtus var izmantot, lai izceltu lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="e9971-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="e9971-113">[Direktorija shēmas paplašinājuma atribūtu izmantošana prasībās](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) ir aprakstīts, kā izmantot direktorija shēmas paplašinājuma atribūtus, lai sūtītu lietotāja datus lietojumprogrammām ar marķiera prasībām.</span><span class="sxs-lookup"><span data-stu-id="e9971-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="e9971-114">Papildinformāciju par marķierierīces prasībām skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="e9971-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="e9971-115">Prasības Access marķierierīcēs</span><span class="sxs-lookup"><span data-stu-id="e9971-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="e9971-116">Prasības id_token</span><span class="sxs-lookup"><span data-stu-id="e9971-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="e9971-117">[Norādes](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) , ko var sagaidīt ID marķierierīcēs un piekļuves marķierierīcēs, ko izsniedz AZURE ad B2C</span><span class="sxs-lookup"><span data-stu-id="e9971-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="e9971-118">SAML marķiera norādes</span><span class="sxs-lookup"><span data-stu-id="e9971-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
