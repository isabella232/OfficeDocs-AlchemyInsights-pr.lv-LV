---
title: Nosacījum piekļuves izmantošana ar Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005781"
---
# <a name="using-conditional-access-with-intune"></a>Nosacījum piekļuves izmantošana ar Intune

Nosacījum piekļuves izmantošanai ar Intune ir jāveic 3 darbības:

- [Izveidojiet atbilstības politiku, lai noteiktu iestatījumus, kuriem ir jābūt, lai ierīci uzskatītu par atbilstošu. Piemēram, ierīcei ir jābūt 6 ciparu PIN kodam, lai to varētu uzskatīt par atbilstošu.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Izveidojiet nosacījum piekļuves politiku, kas nosaka, kādi resursi tiek aizsargāti un kādi nosacījumi ir jāizpilda, lai piekļūtu šiem resursiem. Piemēram, ierīcei ir jābūt atbilstošai, lai varētu piekļūt uzņēmuma e-pastam.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Pārliecinieties, vai atbilstības politikas un nosacījum piekļuves politikas attiecas uz vajadzīgajām lietotāju grupām. Tam var būt nepieciešama noteiktu grupu izveide programmā Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Papildinformācija...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
