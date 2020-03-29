---
title: Vai Teams klients avarē?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030681"
---
# <a name="teams-client-crashing"></a>Vai Teams klients avarē?

Ja jūsu Teams klients avarē, mēģiniet veikt tālāk norādītās darbības:

- Ja izmantojat Teams datora programmu, [pārliecinieties, vai programma ir pilnībā atjaunināta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Pārliecinieties, vai ir pieejami visi [Office 365 URL un adrešu diapazoni](https://docs.microsoft.com/microsoftteams/connectivity-issues).

- Piesakieties ar savu administratora kontu un pārbaudiet [Pakalpojumu darbspējas informācijas panelis](https://docs.microsoft.com/office365/enterprise/view-service-health), vai nav dīkstāves vai pakalpojuma degradācijas.

 - Pēdējā darbības solī varat mēģināt iztīrīt savu Teams klienta kešatmiņu:

    1.  Pilnībā aizveriet Microsoft Teams darbvirsmas klientu. Varat ar peles labo pogu noklikšķināt **Teams** no ikonu teknes un noklikšķināt uz **Aizvērt**vai palaist uzdevumu pārvaldnieku un pilnībā apturēt procesu.

    2.  Dodieties uz failu pārlūku un ierakstiet %appdata%\Microsoft\teams.

    3.  Kad būsiet direktorijā, jūs redzēsiet dažas no tālāk norādītajām mapēm:

         - Sadaļā **Programmas kešatmiņa**, atveriet kešatmiņu un izdzēsiet jebkurus no failiem kešatmiņas atrašanās vietā: %appdata%\Microsoft\teams\application cache\cache.

        - Sadaļā **Blob_storage**izdzēsiet visus failus: %appdata%\Microsoft\teams\ blob_storage.

        - Sadaļā **Kešatmiņa**izdzēsiet visus failus: %appdata%\Microsoft\teams\Cache.

        - Sadaļā **datubāzes**izdzēsiet visus failus: %appdata%\Microsoft\teams\databases.

        - Sadaļā **GPU kešatmiņa**izdzēsiet visus failus: %appdata%\Microsoft\teams\GPUcache.

        - Sadaļā **IndexedDB**izdzēsiet .db failu: %appdata%\Microsoft\teams\IndexedDB.

        - Sadaļā **Lokālā krātuve**izdzēsiet visus failus: %appdata%\Microsoft\teams\Local Storage.

        - Visbeidzot **tmp**izdzēsiet jebkuru failu: %appdata%\Microsoft\teams\tmp.

    4. Restartējiet Teams klientu.
