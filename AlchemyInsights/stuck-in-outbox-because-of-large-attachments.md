---
title: Iestrēdzis izsūtnē lielu pielikumu dēļ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241259"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Labot izsūtnē iestrēgušos ziņojumus

Ieteicams sākt, palaižot scenāriju ["man ir problēmas ar e-pasta ziņojumu sūtīšanu, saņemšanu vai atrašanu"](https://aka.ms/SaRA-OutlookSendReceive) no [Microsoft atbalsta un atkopšanas palīga](https://diagnostics.office.com/#/) rīka.

Kad ziņojums tiek iestrēdzis izsūtnē, Visdrīzāk iemesls ir liels pielikumu vai opciju "nosūtīt uzreiz pēc savienojuma" nav iespējots.

**Noņemiet lielo pielikumu**

1. Programmā Outlook atlasiet **Nosūtīt/saņemt** > **darbu bezsaistē**. 
2. Navigācijas rūtī atlasiet **Izsūtne**. No šejienes jūs varat: 
    - Izdzēsiet ziņu (atlasiet to un pēc tam atlasiet **Dzēst**).
    - Velciet ziņojumu uz melnrakstu mapi, veiciet dubultklikšķi, lai to atvērtu, un noņemiet pielikumu atlasiet to un pēc tam atlasiet **Dzēst**).
3. Ja tiek parādīts kļūdas ziņojums, kurā teikts, ka programma Outlook mēģina pārraidīt ziņojumu, aizveriet programmu Outlook. Tas var aizņemt kādu brīdi, lai izietu. Ja programma Outlook netiek aizvērta, nospiediet taustiņu kombināciju CTRL + ALT + DELETE un atlasiet **startēt uzdevumu pārvaldnieku**. Uzdevumu pārvaldniekā atlasiet cilni **procesi** , ritiniet uz leju līdz Outlook. exe un atlasiet **Beigt procesu**.
4. Kad programma Outlook tiek aizvērta, restartējiet to un atkārtojiet 2. un 3. darbību. 
5. Pēc pielikuma noņemšanas noklikšķiniet uz **Nosūtīt/saņemt** > **darbu bezsaistē** , lai atsāktu darbu tiešsaistē. 

Ziņojumi tiek iestrēguši arī izsūtnē, kad noklikšķināt uz **nosūtīt**, bet nav izveidots savienojums. Noklikšķiniet uz **Nosūtīt/saņemt** un paskatieties uz pogu **strādāt bezsaistē** . Ja tas ir zils, jūs esat atvienots. Noklikšķiniet uz tās, lai savienotu (poga kļūst balta) un noklikšķiniet uz **Sūtīt visu**.
 
**Iespējot nosūtīšanu uzreiz pēc savienojuma**
 
1. Cilni failu, noklikšķiniet uz **Opcijas**.

2. Outlook opcijas dialoglodziņā noklikšķiniet uz **papildu**.

3. Sadaļā nosūtīt un saņemt noklikšķiniet, lai iespējotu **nosūtīt uzreiz pēc savienojuma**. Noklikšķiniet uz **Labi**.
 
Lai iegūtu pilnīgu informāciju, skatiet:
- [Video: sūtīt vai izdzēst iestrēdzis e-pastu](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-pasts paliek mapē Izsūtne līdz jūs manuāli uzsākt sūtīšanas/saņemšanas operāciju programmā Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
