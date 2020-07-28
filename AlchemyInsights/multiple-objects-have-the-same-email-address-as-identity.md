---
title: Vairākiem objektiem ir viena e-pasta adrese kā identitāte
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439191"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Vairākiem objektiem ir viena e-pasta adrese kā identitāte

**Vairāki objekti**

Viens no biežākajiem šīs kļūdas iemesliem ir tas, ka ar to pašu e-pasta adresi nav iespējams pareizi maršrutēt Outlook Web Access pieprasījumu vairāku objektu klātbūtnē. Lai atrastu šos objektus, izpildiet tālāk norādītās komandas.

· Iegūt adresātu<email address>

· Iegūt lietotāju<email address>

· Get-user <email address> -SoftDeletedUser

· Saņemt kontaktpersonas<email address>

· Get-Pastkaste <email address> — PublicFolder

· Get-Pastkaste <email address> — IncludeSoftDeletedMailbox

· Get-Pastkaste <email address> — InactiveMailboxOnly

Lai atrisinātu šo problēmu, noņemiet vairākus objektus ar tādu pašu e-pasta identitāti un pārliecinieties, vai ir viens objekts ar konkrētu e-pasta identitāti un tā adresāta tips ir UserMailbox.

**To pašu adresi izmanto biznesa un patērētāju pastkastēm**

Vēl viens iemesls ir, kad to pašu adresi izmanto uzņēmumu un patērētāju pastkastēm. Šajā gadījumā lietotājam ir jāmaina primārais patērētāju aizstājvārds, līdz kafejnīca atbalsta šo scenāriju. Šī ir pastāvīga kļūda, kas nepazūd bez iejaukšanās.

Detalizētu informāciju skatiet rakstā [e-pasta adreses vai tālruņa numura maiņa savam Microsoft kontam](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).