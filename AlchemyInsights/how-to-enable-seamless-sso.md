---
title: Kā iespējot viengabala SSO
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
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780534"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="d6f86-102">Kā iespējot viengabala SSO</span><span class="sxs-lookup"><span data-stu-id="d6f86-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="d6f86-103">Iespējojiet nevainojamu SSO, izmantojot [AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="d6f86-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="d6f86-104">Ja veicat jaunu Azure AD Connect instalāciju, izvēlieties [pielāgoto instalācijas ceļu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="d6f86-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="d6f86-105">**Lietotāja pierakstīšanās** lapā izvēlieties opciju **Iespējot vienotu pierakstīšanos** .</span><span class="sxs-lookup"><span data-stu-id="d6f86-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="d6f86-106">Lai pārliecinātos, vai ir iespējots viengabalains SSO.</span><span class="sxs-lookup"><span data-stu-id="d6f86-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="d6f86-107">Pierakstieties [Azure Active Directory administrēšanas centrā](https://aad.portal.azure.com) kā globālais administrators.</span><span class="sxs-lookup"><span data-stu-id="d6f86-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="d6f86-108">Kreisajā rūtī atlasiet **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="d6f86-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="d6f86-109">Pārbaudiet, vai ir **iespējota**bezproblēmu vienotā pierakstīšanās.</span><span class="sxs-lookup"><span data-stu-id="d6f86-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="d6f86-110">Lai uzzinātu vairāk, skatiet rakstu [Azure Active Directory vienotā pierakstīšanās: īsā palaišana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="d6f86-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  