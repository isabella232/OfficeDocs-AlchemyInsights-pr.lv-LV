---
title: Federācijas ADF beidzas sertifikātu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2019
ms.locfileid: "28300241"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="f3c46-102">Federācijas ADF beidzas sertifikātu</span><span class="sxs-lookup"><span data-stu-id="f3c46-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="f3c46-103">Lai atrisinātu šo problēmu, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="f3c46-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="f3c46-p101">Datorā, instalējiet Microsoft Azure Active Directory moduli par Windows PowerShell (ja jau nav instalēta modulis). Lai to izdarītu, _ pārejiet uz [pārvaldīt debeszils reklāmu, izmantojot programmu Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="f3c46-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="f3c46-106">Izpildiet norādījumus sadaļā "scenārijs 1: AD FS pilnvaru paraksta sertifikāta derīgums" sadaļā ["Tur bija problēma, lai piekļūtu vietnei" kļūda no AD FS kad Federatīvas lietotājs pierakstās pakalpojumā Office 365, debeszils, vai Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="f3c46-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="f3c46-107">Izpildiet norādījumus sadaļā [kā jāatjaunina vai jālabo Federatīvas domēnu pakalpojumā Office 365, debeszils, vai Intune iestatījumus](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="f3c46-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="f3c46-108">Lai uzzinātu vairāk par Federācijas apliecības atjaunošanu, skatiet [atjaunot Federācijas sertifikātus Office 365 un debeszils Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="f3c46-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

