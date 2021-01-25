---
title: Lietotāja nodrošināšanas atribūtu kartēšana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949766"
---
# <a name="user-provisioning-attribute-mapping"></a>Lietotāja nodrošināšanas atribūtu kartēšana

1. Lai novērstu zināmās atribūtu kartēšanas problēmas, skatiet rakstu [atribūtu kartēšana](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) nodrošina lietotāju nodrošināšanas atbalstu trešo pušu SaaS lietojumprogrammām, piemēram, Salesforce, G Suite un citiem. Ja iespējojat lietotāja nodrošināšanu trešās puses SaaS lietojumprogrammai, Azure portāls kontrolē tās atribūtu vērtības, izmantojot atribūtu kartējumus. Lai uzzinātu, kā pielāgot noklusējuma atribūtu kartējumus, skatiet rakstu [lietotāja nodrošinājuma atribūta pielāgošana San lietojumprogrammām Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Papildinformāciju par SaaS lietojumprogrammas lietotāju nodrošināšanu skatiet rakstā [kas ir automatizētās Saas lietojumprogrammas lietotāju nodrošinājums AZURE ad?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Pielāgojot atribūtu kartējumus lietotāju nodrošināšanai, var gadīties, ka atribūtu, kuru vēlaties kartēt, neparādās avota atribūtu sarakstā. [Sinhronizējot atribūtu no lokālā Active Directory uz AZURE AD,](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) lai to piešķirtu lietojumprogrammas rakstam, tiek parādīts, kā pievienot trūkstošo atribūtu, sinhronizējot to no lokālās ad uz Azure AD.
