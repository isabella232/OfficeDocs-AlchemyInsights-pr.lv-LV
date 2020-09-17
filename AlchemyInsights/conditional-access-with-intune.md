---
title: Ierobežotas piekļuves tiesības ar Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807666"
---
# <a name="conditional-access-with-intune"></a>Ierobežotas piekļuves tiesības ar Intune

**Ierobežotas piekļuves** izmantošanai ar Intune ir jāveic 3 darbības:

- Izveidojiet  **atbilstības politiku**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), lai definētu iestatījumus, kas jāizpilda, pirms ierīce tiek uzskatīta par atbilstošu. Piemēram, ierīcei ir jābūt vismaz 6 ciparu spraudīti, pirms tā tiek uzskatīta par atbilstošu.
- Izveidojiet **nosacījuma piekļuves politiku**  , kas nosaka, kādi resursi tiek aizsargāti, un kādi nosacījumi ir jāievēro, lai piekļūtu šiem resursiem.  [Piemēram,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  ierīcei ir jābūt savietojamai, pirms piekļūstat korporatīvajam e-pastam.
- Nodrošināt, lai **atbilstības politikas**  un  **ierobežotas piekļuves politikas**  būtu paredzētas vajadzīgajām lietotāju grupām. Tam var būt nepieciešama noteiktu lietotāju grupu izveide Azure Active Directory.

**Noderīgas saites:**

[Ierīces atbilstības pārskats](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problēmu novēršana CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Problēmu novēršanas politika](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Lai aizsargātu e-pastu (Exchange Online) no piekļuves nesavietojamās ierīcēs, ir jāievēro abi dokumenti:

1. [E-pasta piekļuves aizsardzība no ierīcēm, kas izmanto EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [E-pasta piekļuves aizsardzība no ierīcēm, kas izmanto modernās autentifikācijas klientus, piemēram, Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)