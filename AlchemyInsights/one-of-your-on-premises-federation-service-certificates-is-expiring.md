---
title: Viens no lokālajiem Federācijas pakalpojumu sertifikāti beidzas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: e1afad0bab317af0f60a6ebda8c3ec8be398e38d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753037"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="51c4d-102">Viens no lokālajiem Federācijas pakalpojumu sertifikāti beidzas</span><span class="sxs-lookup"><span data-stu-id="51c4d-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="51c4d-103">Lai atrisinātu šo problēmu, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="51c4d-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="51c4d-104">Datorā, instalējiet Microsoft Azure Active Directory moduli par Windows PowerShell (ja jau nav instalēta modulis).</span><span class="sxs-lookup"><span data-stu-id="51c4d-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="51c4d-105">Lai to izdarītu, dodieties uz [Debeszils Active Directory PowerShell Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="51c4d-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="51c4d-106">Izpildiet norādījumus sadaļā "scenārijs 1: AD FS pilnvaru paraksta sertifikāta derīgums" sadaļā ["Tur bija problēma, lai piekļūtu vietnei" kļūda no AD FS kad Federatīvas lietotājs pierakstās pakalpojumā Office 365, debeszils, vai Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="51c4d-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="51c4d-107">Izpildiet norādījumus sadaļā t[kā jāatjaunina vai jālabo Federatīvas domēnu pakalpojumā Office 365, debeszils, vai Intune iestatījumus](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="51c4d-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="51c4d-108">Plašāku informāciju par Federācijas apliecības atjaunošanu skatiet [sertifikāta atjaunošanu O365 un debeszils reklāmu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="51c4d-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

