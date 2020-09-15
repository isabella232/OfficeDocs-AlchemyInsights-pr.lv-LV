---
title: Beidzas viens no jūsu lokālo Federāciju pakalpojumu sertifikātiem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673504"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="1a983-102">Beidzas viens no jūsu lokālo Federāciju pakalpojumu sertifikātiem</span><span class="sxs-lookup"><span data-stu-id="1a983-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="1a983-103">Lai atrisinātu šo problēmu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="1a983-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="1a983-104">Instalējiet Microsoft Azure Active Directory moduli, kas paredzēts Windows PowerShell datorā (ja modulis jau nav instalēts).</span><span class="sxs-lookup"><span data-stu-id="1a983-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="1a983-105">Lai to izdarītu, dodieties uz [Azure Active Directory PowerShell diagrammai ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="1a983-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="1a983-106">Rīkojieties saskaņā ar darbībām, kas aprakstītas sadaļā "1. scenārijs: AD FS pilnvaru parakstīšanas sertifikāta derīgums" [ir radusies problēma, piekļūstot vietnei "kļūdas ziņojums no AD FS, kad ārējs lietotājs pierakstās pakalpojumā Microsoft 365, Azure vai Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="1a983-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="1a983-107">Veiciet darbības, kas norādītas rakstā [kā atjaunināt vai labot domēna ārējos domēnu, kas atrodas pakalpojumā Microsoft 365, Azure vai Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="1a983-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="1a983-108">Papildinformāciju par Federācijas sertifikātu atjaunošanu skatiet rakstā [O365 un AZURE ad sertifikātu atjaunošana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="1a983-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

