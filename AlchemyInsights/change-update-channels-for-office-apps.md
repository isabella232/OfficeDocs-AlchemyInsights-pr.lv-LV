---
title: Office programmu atjaunināšanas kanālu mainīšana
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
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439391"
---
# <a name="change-update-channels-for-office-apps"></a>Office programmu atjaunināšanas kanālu mainīšana

Jauno Office instalāciju gadījumā izmantojiet Office programmatūras lejupielādes iestatījumus, lai atlasītu vajadzīgo atjaunināšanas kanālu, un pēc tam instalējiet (vai atkārtoti instalējiet) Office lietojumprogrammas. Papildinformāciju skatiet rakstā [programmatūras lejupielādes iestatījumu pārvaldība sistēmā Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Piezīmes** Atlasītais atjaunināšanas kanāls, izmantojot Office programmatūras lejupielādes iestatījumus, attiecas uz visiem lietotājiem, kas veic jaunas instalācijas, izmantojot O365 portālu. Papildinformāciju skatiet rakstā [Microsoft 365 vai Office 2019 lejupielāde un instalēšana vai pārinstalēšana PC vai Mac datorā](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Esošajām Office instalācijām izmantojiet Office izvietošanas rīku (ODT), lai pārslēgtos uz citu atjaunināšanas kanālu:  

1. Lejupielādējiet jaunāko Office izvietošanas rīka versiju (setup.exe) no [Microsoft lejupielādes centra](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Identificējiet tā kanāla nosaukumu, uz kuru vēlaties pārslēgties. Papildinformāciju skatiet rakstā [Office izvietošanas rīka konfigurācijas opcijas](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Izveidojiet konfigurācijas XML failu, kas norāda attiecīgo kanāla nosaukumu, piemēram, update.xml.  
    izveide. <Configuration>  
    b. <atjauninājumi **kanāls = "month"** />  
    c. </Configuration>
4. Priviliģētā komandu uzvednē pārslēdzieties uz mapes atrašanās vietu, kur atrodas setup.exe, un izpildiet šādu komandu:  
    izveide. setup.exe/Configure update.xml
5. Palaidiet Office lietojumprogrammu (piemēram, Excel) un pēc tam atlasiet **faila**  >  **konts**. Sadaļā informācija par produktu atlasiet **atjaunināšanas opcijas**  >  **Atjaunināt tūlīt**.

Papildinformāciju skatiet rakstā [kā mainīt esošo Office programmu atjaunināšanas kanālus](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Informāciju par atjaunināšanas kanālu maiņu atlasītajai lietotāju grupai vai izmantojot konfigurācijas pārvaldnieku (SCCM), konfigurējiet atjaunināšanas kanāla iestatījumu, izmantojot GPO. Papildinformāciju skatiet rakstā [Microsoft 365 programmu atjaunināšanas kanālu pārskats](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Detalizētu informāciju skatiet rakstā [kā pārvaldīt Office 365 ProPlus kanālus IT profesionāļiem](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) un [pārvaldīt Microsoft 365 programmu atjauninājumus, izmantojot Microsoft galapunktu konfigurācijas pārvaldnieku](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).