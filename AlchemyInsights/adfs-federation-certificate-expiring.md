---
title: ADFS Federācijas sertifikāta derīguma termiņš beidzas
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686721"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federācijas sertifikāta derīguma termiņš beidzas

Lai atrisinātu šo problēmu, veiciet tālāk norādītās darbības.
  
1. Instalējiet Microsoft Azure Active Directory moduli, kas paredzēts Windows PowerShell datorā (ja modulis jau nav instalēts). Lai to izdarītu, dodieties uz [AZURE ad pārvaldība, izmantojot Windows PowerShell](https://aka.ms/aadposh).

2. Rīkojieties saskaņā ar darbībām, kas aprakstītas sadaļā "1. scenārijs: AD FS pilnvaru parakstīšanas sertifikāta derīgums" [ir radusies problēma, piekļūstot vietnei "kļūdas ziņojums no AD FS, kad ārējs lietotājs pierakstās pakalpojumā Microsoft 365, Azure vai Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Izpildiet darbības, kas aprakstītas rakstā [Microsoft, Azure vai Intune integrētās domēna iestatījumu atjaunināšana vai labošana](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Papildinformāciju par Federācijas sertifikātu atjaunošanu skatiet rakstā [Microsoft 365 un Azure Active Directory Federācijas sertifikātu atjaunošana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
