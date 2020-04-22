---
title: ADFS Federācijas sertifikāts beidzas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710414"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federācijas sertifikāts beidzas

Lai novērstu šo problēmu, rīkojieties šādi:
  
1. Instalējiet Microsoft Azure Active Directory modulis Windows PowerShell datorā (ja modulis jau nav instalēts). Lai to izdarītu, dodieties uz [pārvaldīt AZURE ad, izmantojot programmu Windows PowerShell](https://aka.ms/aadposh).

2. Izpildiet darbības "1. scenārijs: AD FS pilnvaru parakstīšanas sertifikāta derīgums" sadaļā ["radās problēma, piekļūstot vietnes" kļūda no ad FS, ārējam lietotājam pierakstās Microsoft 365, Azure vai InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Veiciet darbības, lai [atjauninātu vai labotu integrētās domēnu Microsoft, Azure vai InTune iestatījumus](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Lai iegūtu papildinformāciju par atjaunošanu Federācijas sertifikātu, skatiet [atjaunot Federācijas sertifikāti Microsoft 365 un Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
