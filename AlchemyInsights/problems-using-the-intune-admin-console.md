---
title: Problēmas, izmantojot Intune administrēšanas konsoli
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555385"
---
# <a name="problems-using-the-intune-admin-console"></a>Problēmas, izmantojot Intune administrēšanas konsoli

**"Piekļuve liegta", naviģējot uz Intune administrēšanas portālu.**

- Ja esat Intune pielāgotās lomas dalībnieks, pārliecinieties, vai jūsu kontam ir piešķirta Windows Intune vai Enterprise Mobility Suite (EMS) licence.
- Ja izmantojat konfigurācijas pārvaldnieku, lai pārvaldītu ierīces, pārbaudiet, vai jums nav daļa no Intune lietotāju kolekcijas konfigurēšanas pārvaldnieka MDM.
- Pārbaudiet, vai jums ir piešķirtas atbilstošas administrēšanas vadīklas (RBAC) atļaujas Windows Intune lomas asmeņā.
- Pārbaudiet, vai izmantotā grupa nav adresātu saraksts. Windows Intune Azure portālā atbalsta tikai to lietotāju kontus, kas pieder Azure Active Directory drošības grupām. Pārskatiet savas grupas Azure portālā > **Intune**  >  **groups**vai Azure portālā > **Azure Active Directory**.

**Lietotājam ir pārāk daudz atļauju piešķirtajai Intune lomai**

Ieteikt lietotājam pāriet uz **Intune**  >  **Intune lomām**  >  **manas atļaujas**  >  **Eksportēt** , lai pārskatītu piešķirtās atļaujas.

**Esmu pievienojis tvēruma grupu lomai, taču šīs lomas lietotāji joprojām redz citus lietotājus vai ierīces.**

Tvērumu grupas nefiltrē lietotājus vai ierīces. Tvērumu grupas:

- Ierobežojiet to, kam lietotāji var piešķirt politikas vai lietojumprogrammas.
- Atļaut tikai konkrētiem lietotājiem palaist attālos uzdevumus ierīcēs.

Papildinformāciju par tvērumu grupām skatiet rakstā [lomu piekļuves vadība (RBAC) ar Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Pievienoju lietotāju Intune lomai, bet joprojām ir pilna piekļuve Intune administrēšanas konsolei.**

Pārejiet uz Intune > **lietotājiem** Azure portālā un pārbaudiet, vai lietotājam nav piešķirta neviena no šīm lomām Azure portālā:

- Globālais administrators
- Intune pakalpojuma administrators
- SharePoint administrators

Papildinformāciju skatiet rakstā [lomu piekļuves vadība (RBAC) ar Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Access problēmas**

Papildinformāciju skatiet rakstā [nevar pierakstīties pakalpojumā Office 365, Azure vai Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).