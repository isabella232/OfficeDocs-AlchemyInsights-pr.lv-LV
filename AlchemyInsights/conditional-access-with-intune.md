---
title: Ierobežota piekļuve ar Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931443"
---
# <a name="conditional-access-with-intune"></a>Ierobežota piekļuve ar Intune

Ierobežotas **piekļuves ar** Intune izmantošanai ir jāveic 3 darbības:

- Izveidojiet **atbilstības politiku** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), lai definētu iestatījumus, kas ir jāizpilda, pirms ierīce tiek uzskatīta par atbilstošu. Piemēram, ierīces pin jābūt vismaz 6 ciparu kontaktam, pirms to uzskata par atbilstošu.
- Izveidojiet **ierobežotas piekļuves politiku,** kas definē, kādi resursi tiek aizsargāti un kādi nosacījumi ir jāizpilda, lai piekļūtu šiem resursiem.  [Piemēram, ierīcei](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) ir jābūt saderīgai pirms piekļuves uzņēmuma e-pastam.
- Pārliecinieties, vai **atbilstības politikas** **un ierobežotas piekļuves** politikas ir paredzētas vēlamajās lietotāju grupās. Tas var būt nepieciešams izveidot noteiktas lietotāju grupas Azure Active Directory.

**Noderīgas saites:**

[Ierīces atbilstības pārskats](https://docs.microsoft.com/intune/device-compliance-get-started)

[Ca problēmu novēršana](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Problēmu novēršanas politika](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Lai aizsargātu e-pastu (Exchange online) no piekļuves nesaderīgām ierīcēm, jāievēro abi dokumenti:

1. [E-pasta piekļuves aizsardzība no ierīcēm, izmantojot EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [E-pasta piekļuves aizsardzība no ierīcēm, izmantojot mūsdienu autentifikācijas klientus, piemēram, Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)