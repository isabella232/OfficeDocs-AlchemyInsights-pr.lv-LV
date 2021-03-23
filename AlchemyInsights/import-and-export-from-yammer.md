---
title: Importēšana un eksportēšana no Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036122"
---
# <a name="import-and-export-from-yammer"></a>Importēšana un eksportēšana no Yammer

**Importa**

Lietotāja importēšanas opcijas atšķiras atkarībā no tā, vai jūsu Yammer tīkls ir [Microsoft 365 vietējā režīmā](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode).

- **Nevietējais režīms**: lietotājus var importēt grupās, izmantojot opciju [Pievienot no adrešu grāmatas](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (ierobežot līdz 100 lietotājiem) grupas iestatījumos vai tīklā, izmantojot [lielapjoma atjaunināšanu](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) tīkla administrators.
- **Vietējais režīms**: dalības grupas un tīkla dalības darbības jāveic no [Microsoft 365 administrēšanas portāla](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portāla](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)vai izmantojot citu Azure AD opciju. Vietējā režīmā tīkliem vairs nav pieejama lielapjoma atjaunināšana un citi mantotie līdzekļi.

> [!IMPORTANT]
> Yammer nekad neatbalsta satura importēšanu no tīkla administratora pat tad, ja datu eksportēšanas līdzeklis ir izmantots citā tīklā. Saturu var atkārtoti publicēt partnera risinājumos vai Yammer REST API.

**Eksportēšana**

Tīkla [datu eksportēšana tīkla administrators](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) ļauj eksportēt saturu no Yammer tīkliem, tostarp ziņojumiem un failiem. Pielikumi var būt ļoti lieli, un to veikšanai būs nepieciešams ievērojams laiks. Ir ieteicams, lai aktīvie tīkli tiktu eksportēti, izmantojot [datu eksportēšanas API](https://developer.yammer.com/docs/data-export-api) , kas atrodas gabalos pēc dienas vai nedēļas. Microsoft atbalsts šim nolūkam nenodrošina pielāgotus skriptus.

Pastāv atsevišķs [vdar eksports](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) , lai eksportētu saturu atsevišķam lietotājam.