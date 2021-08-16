---
title: Nosacījum piekļuve ar Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069719"
---
# <a name="conditional-access-with-intune"></a>Nosacījum piekļuve ar Intune

Nosacījum  **piekļuves izmantošanai**  ar Intune ir jāveic 3 darbības:

- Izveidojiet **atbilstības politiku** ([Android,](https://docs.microsoft.com/intune/compliance-policy-create-android) [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios) [, Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), lai definētu iestatījumus, kuriem ir jābūt, lai ierīci varētu uzskatīt par atbilstošu. Piemēram, ierīcei ir jābūt 6 ciparu PIN kodam, lai to varētu uzskatīt par atbilstošu.
- Izveidojiet **nosacījum piekļuves politiku,**  kas nosaka, kādi resursi tiek aizsargāti un kādi nosacījumi ir jāizpilda, lai piekļūtu šiem resursiem.  [Piemēram, ierīcei](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  ir jābūt atbilstošai, lai varētu piekļūt uzņēmuma e-pastam.
- **Pārliecinieties, vai atbilstības politikas** un nosacījum **piekļuves** politikas attiecas uz vajadzīgajām lietotāju grupām. Tam var būt nepieciešama noteiktu grupu izveide programmā Azure Active Directory.

**Noderīgas saites:**

[Ierīces atbilstības pārskats](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problēmu novēršana CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Problēmu novēršanas politika](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Lai aizsargātu e-pastu (Exchange tiešsaistē) pret piekļuvi bezsalīdzināmām ierīcēm, ir jāievēro abi dokumenti:

1. [Kā aizsargāt piekļuvi e-pastam no ierīcēm, izmantojot EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Kā aizsargāt piekļuvi e-pastam no ierīcēm, kas izmanto modernās autentifikācijas klientus, piemēram, Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)