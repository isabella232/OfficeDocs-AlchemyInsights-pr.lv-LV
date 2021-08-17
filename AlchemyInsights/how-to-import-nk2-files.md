---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043213"
---
# <a name="how-to-import-nk2-files"></a>Kā importēt .nk2 failus 

Pirmoreiz startējot Microsoft Outlook 2013, Outlook 2016, Outlook 2019 vai Outlook pakalpojumam Microsoft 365, segvārdu kešatmiņa (saglabāta *profila* nosaukumā .nk2 failā) tiek importēta paslēptā ziņojumā noklusējuma ziņojumu krātuvē.

Lai importētu .nk2 failus programmā Outlook 2013, Outlook 2016, Outlook 2019 vai Outlook pakalpojumam Microsoft 365, pārliecinieties, vai fails .nk2 atrodas šajā mapē: %appdata%\Microsoft\Outlook

**Piezīme.**.nk2 failam ir jābūt tādam pašam nosaukumam, kā pašreizējam 2013 Outlook 2013. gada Outlook 2016 profilam. Pēc noklusējuma profila nosaukums ir "Vārds Outlook". Lai pārbaudītu profila nosaukumu, veiciet tālāk norādītās darbības. 
1. Noklikšķiniet **uz** Sākt un pēc tam uz **Vadības panelis.**
2. Veiciet dubultklikšķi uz **Pasts.**
3. Dialoglodziņā Pasta iestatīšana atlasiet Rādīt **profilus**.
4. Atlasiet **Sākt**  >  **palaist**.
5. Lodziņā **Atvērt ierakstiet** importēšanas *outlook.exe /importnk2* un pēc tam atlasiet **Labi**. 

Pēc faila .nk2 importēšanas faila saturs tiek sapludināts esošajā segvārdu kešatmiņā, kas tiek glabāta jūsu pastkastē.

**Piezīme.** Nākamajā reizē, kad startēsiet Outlook 2013, Outlook 2016, Outlook 2019 vai 2019, tiks pārdēvēts .nk2 fails Outlook pakalpojumam Microsoft 365. Ja vēlaties atkārtoti importēt .nk2 failu, vispirms noņemiet .old faila nosaukuma paplašinājumu.

Papildinformāciju skatiet [rakstā Automātiskās pabeigšanas saraksta importēšana vai kopēšana citā datorā.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)