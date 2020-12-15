---
title: Ierīce gaidīšanas režīmā
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678484"
---
# <a name="device-in-pending-state"></a>Ierīce gaidīšanas režīmā

**Priekšnoteikumi**

1. Ja iestatāt ierīču reģistrācijas pirmo reizi, lūdzu, pārliecinieties, ka esat pārskatījis [Azure Active Directory (AZURE AD) Ievads](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) par ierīču pārvaldību, kas palīdzēs iegūt ierīces, kas atrodas Azure AD vadībā.
2. Ja esat reģistrējis ierīces Azure AD tiešā veidā un reģistrējat to Intune, jums ir jāpārliecinās, vai esat [konfigurējis Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) un ir vispirms [jālicencē](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .
3. Pārliecinieties, vai jums ir atļauts veikt darbības Azure AD un lokālajā REKLĀMā. Tikai globālais administrators Azure AD var pārvaldīt ierīces reģistrācijām paredzētos iestatījumus. Turklāt, ja iestatāt automātiskas reģistrācijas savā lokālajā Active Directory, jums būs nepieciešams Active Directory un AD FS administrators (ja piemērojams).

Hibrīdā Azure AD pievienošanās reģistrācijas procesam ir nepieciešamas ierīces, lai tās būtu korporatīvajā tīklā. Tā darbojas arī uz VPN, bet tam ir daži brīdinājumi. Mēs esam dzirdējuši, ka klientiem ir nepieciešama palīdzība saistībā ar Hibrīdā Azure AD pievienošanās reģistrācijas procesam attālā darba apstākļos.

**Mākoņa autentifikācijas vide (izmantojot Azure AD Password hash Sync vai tranzīta autentifikāciju)**

Šo reģistrācijas plūsmu dēvē arī par sinhronizācijas savienojumu.

Tālāk ir aprakstīts, kas notiek reģistrācijas procesa laikā.

1. Windows 10 atklāj pakalpojumu savienojuma punkta (SCP) ierakstu, kad lietotājs piesakās savā ierīcē.

    1. Ierīce vispirms mēģina izgūt nomnieka informāciju no klienta puses SCP reģistrā [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Papildinformāciju skatiet rakstā [dokuments](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Ja tas nelīdz, ierīce komunicē ar lokālo Active Directory, lai iegūtu nomnieka informāciju no SCP. Lai verificētu SCP, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Ieteicams iespējot SCP Active Directory un izmantot tikai klienta puses SCP sākotnējai validācijai.

2. Windows 10 mēģina sazināties ar Azure AD, izmantojot sistēmas kontekstu, lai autentificētu sevi pret Azure AD.

    Varat pārbaudīt, vai ierīce var piekļūt Microsoft resursiem sistēmas kontā, izmantojot [testa ierīces reģistrācijas savienojamības skriptu](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 izveido pašparakstītu sertifikātu un saglabā to zem datora objekta lokālajā Active Directory. Lai to izdarītu, ir nepieciešams domēna kontrolleris.

4. Ierīces objekts, kura sertifikāts tiek sinhronizēts ar Azure AD, izmantojot Azure AD Connect. Sinhronizācijas cikls ik pēc noklusējuma ir 30 minūtes, tomēr tas ir atkarīgs no Azure AD Connect konfigurēšanas. Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Šajā posmā varat skatīt tēmas ierīci sadaļā "**gaida**", sadaļā ierīces disks Azure Portal.

6. Nākamajā lietotāja pierakstīšanās operētājsistēmā Windows 10 reģistrācija tiks pabeigta.

    > [!NOTE]
    > Ja esat VPN un atteikšanās/pierakstīšanās pārtrauc domēna savienojamību, varat manuāli aktivizēt reģistrāciju. Lai to izdarītu:
    >
    > `dsregcmd /join`Lokāli jautājiet savā datorā, izmantojot PSExec.
    >
    > Piemēram: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Biežāk sastopamās problēmas ar Azure Active Directory ierīces reģistrēšanu skatiet rakstā [bieži uzdotie jautājumi par ierīcēm](https://docs.microsoft.com/azure/active-directory/devices/faq).
