---
title: Ar paroli pamatotas vienotās pierakstīšanās (SSO) problēmu novēršana
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714892"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="f1f46-102">Ar paroli pamatotas vienotās pierakstīšanās (SSO) problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="f1f46-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="f1f46-103">Lai apgūtu SSO ar paroli pamatotos pamatprincipus, skatiet rakstu [ar paroli pamatota autentifikācija ar Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="f1f46-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="f1f46-104">**Ar paroli pamatota SSO konfigurēšana**</span><span class="sxs-lookup"><span data-stu-id="f1f46-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="f1f46-105">Ar [paroli pamatotas vienotās pierakstīšanās konfigurēšana](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) . Šajā rakstā ir sniegta detalizēta informācija par SSO opciju ar paroli.</span><span class="sxs-lookup"><span data-stu-id="f1f46-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="f1f46-106">Ja pievienojamajai lietojumprogrammai nepieciešama pielāgota konfigurācija un jums ir jāizmanto ar paroli pamatots SSO, šis raksts ir paredzēts jums.</span><span class="sxs-lookup"><span data-stu-id="f1f46-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="f1f46-107">Ar [paroli pamatotas vienotās pierakstīšanās konfigurēšana lietojumprogrammā Prem lietojumprogrammas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) starpniekserveris atbalsta vairākus vienotās pierakstīšanās režīmus.</span><span class="sxs-lookup"><span data-stu-id="f1f46-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="f1f46-108">Pierakstīšanās ar paroli ir paredzēts lietojumprogrammām, kas izmanto lietotājvārdu/paroļu kombināciju autentifikācijai.</span><span class="sxs-lookup"><span data-stu-id="f1f46-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="f1f46-109">Ja savā lietojumprogrammā konfigurējat pierakstīšanos ar paroli, lietotājiem ir vienreiz jāpierakstās lokālajā lietojumprogrammā.</span><span class="sxs-lookup"><span data-stu-id="f1f46-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="f1f46-110">Pēc tam Azure Active Directory saglabā pierakstīšanās informāciju un automātiski nodrošina to lietojumprogrammai, kad lietotāji tam piekļūst attāli.</span><span class="sxs-lookup"><span data-stu-id="f1f46-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="f1f46-111">Jūs jau esat publicējis un testējis savu programmu ar lietojumprogrammas starpniekserveri.</span><span class="sxs-lookup"><span data-stu-id="f1f46-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="f1f46-112">Ja tā nav, izpildiet darbības, kas aprakstītas sadaļā [lietojumprogrammu publicēšana, izmantojot AZURE ad Application starpniekserveri](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) , un pēc tam turpiniet ar paroli balstītas SSO for on-Prem lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="f1f46-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="f1f46-113">Lai novērstu ar paroli balstītu SSO, skatiet rakstu [ar paroli pamatotas vienotās pierakstīšanās problēmu novēršana AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="f1f46-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
