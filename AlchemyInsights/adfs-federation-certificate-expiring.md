---
title: Federācijas ADF beidzas sertifikātu
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
ms.openlocfilehash: c9922258c2d203cc07c1a1055ffa36c23a756115
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499898"
---
# <a name="adfs-federation-certificate-expiring"></a>Federācijas ADF beidzas sertifikātu

Lai atrisinātu šo problēmu, rīkojieties šādi:
  
1. Datorā, instalējiet Microsoft Azure Active Directory moduli par Windows PowerShell (ja jau nav instalēta modulis). Lai to izdarītu, _ pārejiet uz [pārvaldīt debeszils reklāmu, izmantojot programmu Windows PowerShell](https://aka.ms/aadposh).

2. Izpildiet norādījumus sadaļā "scenārijs 1: AD FS pilnvaru paraksta sertifikāta derīgums" sadaļā ["Tur bija problēma, lai piekļūtu vietnei" kļūda no AD FS kad Federatīvas lietotājs pierakstās pakalpojumā Office 365, debeszils, vai Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Izpildiet norādījumus sadaļā [kā jāatjaunina vai jālabo Federatīvas domēnu pakalpojumā Office 365, debeszils, vai Intune iestatījumus](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).

    Lai uzzinātu vairāk par Federācijas apliecības atjaunošanu, skatiet [atjaunot Federācijas sertifikātus Office 365 un debeszils Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
