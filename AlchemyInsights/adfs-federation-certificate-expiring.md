---
title: ADFS Federācijas sertifikāts beidzas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/25/2019
ms.locfileid: "36737196"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federācijas sertifikāts beidzas

Lai novērstu šo problēmu, rīkojieties šādi:
  
1. Instalējiet Microsoft Azure Active Directory modulis Windows PowerShell datorā (ja modulis jau nav instalēts). Lai to izdarītu, dodieties uz [pārvaldīt AZURE ad, izmantojot programmu Windows PowerShell](https://aka.ms/aadposh).

2. Izpildiet darbības "1. scenārijs: AD FS pilnvaru parakstīšanas sertifikāta derīgums" sadaļā ["radās problēma, piekļūstot vietnes" kļūda no ad FS, ārējam lietotājam pierakstās Office 365, Azure vai InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Veiciet darbības, lai [atjauninātu vai labotu integrētās domēna Office 365, Azure vai InTune iestatījumus](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Lai iegūtu papildinformāciju par atjaunošanas Federācijas sertifikātu, skatiet [atjaunot Federācijas sertifikāti Office 365 un Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
