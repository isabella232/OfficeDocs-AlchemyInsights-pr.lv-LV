---
title: S/MIME programmā Outlook tīmeklī
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772305"
---
# <a name="encrypt-email-messages-in-outlook"></a>E-pasta ziņojumu šifrēšana programmā Outlook

Microsoft 365 ziņojumu šifrēšana ir veidota Microsoft Azure Rights Management (Azure RMS), kas ir Azure Information Protection daļa. Ja jūsu abonementā ir iekļauta Azure Rights Management vai Azure Information Protection, **jums nav jāveic nekādas darbības, lai manuāli iespējotu vai aktivizētu** tiesību pārvaldības pakalpojumu.

Ņemot vērā klientu atsauksmes, mēs vairs neiespējojam Exchange pasta plūsmas kārtulas, lai automātiski šifrētu izejošos e-pasta ziņojumus, kuros nomniekā ir noteikta veida konfidenciāla informācija. Tā vietā mēs sniedzam detalizētus norādījumus par to, kā varat to izdarīt pats. Papildinformāciju par to, kā izveidot transporta kārtulu, lai šifrētu sensitīvu informāciju, skatiet [šajā rakstā](https://aka.ms/OmeEtr).

- Ja izmantojat Outlook tīmeklī (iepriekš **OWA**): veidojot e-pasta ziņojumu, vienkārši noklikšķiniet uz **aizsargāt** OWA. Tas attieksies uz "Nepārsūtīt" atļauju. Noklikšķiniet uz **mainīt atļaujas** un izvēlieties **Šifrēt** , lai šifrētu tikai šo ziņojumu.

- Ja izmantojat **Outlook klientu**: lai nosūtītu šifrētu ziņojumu no programmas Outlook 2013 vai 2016, vai Outlook 2016 darbam ar Mac, atlasiet **opciju**  >  **atļaujas**un pēc tam atlasiet vajadzīgo aizsardzības opciju.

- Lai **automātiski šifrētu visus e-pasta** ziņojumus, kas nosūtīti konkrētiem adresātiem vai ārējām partnera organizācijām, ir jāizveido pasta plūsmas transportēšanas kārtula Exchange administrēšanas centrā. Detalizēti norādījumi ir sniegti [šajā atbalsta rakstā](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

