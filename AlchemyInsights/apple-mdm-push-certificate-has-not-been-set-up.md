---
title: Apple MDM push sertifikāts nav iestatīts
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
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439380"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM push sertifikāts nav iestatīts

Apple MDM push sertifikāts (zināms arī kā Apple push Notification Service (APN) sertifikāts) nav konfigurēts jūsu abonementam. Ja nav konfigurēts Apple MDM push sertifikāts, jūs nevarat reģistrēties un pārvaldīt iOS un Mac OS ierīces. Pēc sertifikāta pievienošanas Intune lietotāji var instalēt uzņēmuma portāla lietojumprogrammu, lai reģistrētu savas iOS ierīces.

1. Atlasiet **"es piekrītu".** lai piešķirtu Microsoft atļauju nosūtīt datus Apple.

2. Atlasiet **lejupielādēt USA** Intune sertifikāta parakstīšanas pieprasījumu, kas nepieciešams, lai izveidotu Apple MDM push sertifikātu. Fails tiek izmantots, lai pieprasītu uzticamības relācijas sertifikātu no Apple push sertifikātu portāla.

3. Atlasiet **izveidot savu MDM push sertifikātu** , lai pārietu uz Apple push Certificates portālu. Pierakstieties ar sava uzņēmuma Apple ID un pēc tam atlasiet **izveidot sertifikātu**. Atlasiet **izvēlēties failu**, pārlūkojiet līdz sertifikāta parakstīšanas pieprasījuma failam un pēc tam izvēlieties **augšupielādēt**. Apstiprinājuma lapā izvēlieties **lejupielādēt** , lai lejupielādētu sertifikātu (. pem) failu, un saglabājiet failu lokāli.
 
**Piezīme**: sertifikāts ir saistīts ar Apple ID, kas tiek izmantots, lai to izveidotu. Kā paraugpraksi izmantojiet uzņēmuma Apple ID pārvaldības uzdevumiem un pārliecinieties, vai pastkasti pārrauga vairākas personas vai izmantojot adresātu sarakstu. Nekad neizmantojiet personisku Apple ID. Izmantojiet to pašu Apple ID, lai atjaunotu Apple push sertifikātu ik pēc 12 mēnešiem.
 
4. Ievadiet Apple ID, ko izmantojāt, lai izveidotu savu Apple MDM push sertifikātu. Ierakstiet šo ID kā atgādinājumu, kad ir jāatjauno sertifikāts.

5. Dodieties uz sertifikātu (. pem) failu, izvēlieties **Atvērt**un pēc tam izvēlieties **augšupielādēt**. Izmantojot pašpiegādes sertifikātu, Intune var reģistrēt un pārvaldīt Apple ierīces.