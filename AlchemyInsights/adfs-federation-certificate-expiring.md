---
title: ADFS federācijas sertifikāta derīguma termiņš beidzas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952976"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS federācijas sertifikāta derīguma termiņš beidzas

Lai novērstu šo problēmu, veiciet tālāk norādītās darbības.
  
1. Datorā Microsoft Azure Active Directory moduli Windows PowerShell moduli (ja modulis vēl nav instalēts). Lai to izdarītu, dodieties uz [Azure AD pārvaldība, izmantojot Windows PowerShell](https://aka.ms/aadposh).

2. Izpildiet darbības sadaļā "1. scenārijs: AD FS pilnvaru parakstīšanas sertifikāta derīgums beidzies" rakstā Kļūda "Radās problēma, piekļūstot vietnei" no AD FS, kad federatīvs lietotājs pierakstās pakalpojumā [Microsoft 365, Azure vai Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Izpildiet rakstā [Federatīvā domēna Microsoft, Azure vai Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)iestatījumu atjaunināšana vai labošana minētās darbības.

    Papildinformāciju par federācijas sertifikātu atjaunošanu skatiet rakstā [Federācijas sertifikātu atjaunošana Microsoft 365 Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
