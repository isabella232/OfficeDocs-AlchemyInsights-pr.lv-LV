---
title: Yammer paziņojumi
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: a07d5f502beb61ab130e801b0e42579718f4d175a937fee4e21ab9f7339dbffd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097205"
---
# <a name="notifications-in-yammer"></a>Yammer paziņojumi

Lai informētu jūs par jaunām darbībām saistošās sarunās, [Yammer nosūta paziņojumus](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) pa e-pastu, vai, ja izmantojat Yammer mobilajā ierīcē, ar pašpiegādes paziņojumu palīdzību. Pēc noklusējuma Yammer nosūta paziņojumus par dažādu veidu darbībām jūsu tīklā. Lietotāji var atjaunināt savus e-pasta iestatījumus Yammer vietnē, bet pašpiegādes paziņojumu konfigurēšana ir jāveic mobilajā lietotnē. 

Yammer ir pievienots atbalsts [Outlook interaktīvajiem e-pasta ziņojumiem](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Daži e-pasta ziņojumi (ziņojumu kopijas) kļūs interaktīvi Outlook tīmekļa versijā. Citās Outlook versijās šī funkcija būs pieejama vienā no nākamajiem atjauninājumiem.

**Yammer paziņojumu tipu**

- E-pasta ziņojumi (atjauninājumi no grupas, uzaicinājumi grupā, saņemts ziņojums jūsu iesūtnē utt.)
- Pašpiegādes paziņojumi (tiek nosūtīti uz mobilajām ierīcēm, kad jūs tiekat pieminēti, saņemat ziņojumu savā iesūtnē utt.)
- Darbvirsmas uznirstošie logi (ja jūsu datorā ir instalēta Yammer programma, tā parādīs paziņojumus, kas tiek dēvēti par "ziņlodziņiem").
- Joslas paziņojumi (Yammer vietnē lietoti redzēs paziņojumus par dažādiem notikumiem. Šie paziņojumi ne vienmēr var būt saistīti ar konkrētu e-pasta vai pašpiegādes ziņojumu).

Ir pieejama [plašāka informācija par paziņojumiem](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Paziņojumu pārvaldība**

Lietotājiem pašiem ir jāpārvalda savi paziņojumi. Ir pieejama informācija [par Yammer paziņojumu iespējošanu vai atspējošanu e-pastā vai mobilajās ierīcēs](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Administratori nevar atspējot visus paziņojumus vai kontrolēt paziņojumus lietotāju vārdā. Administratori var [kontrolēt e-pastā iekļautos logotipus un to, vai lietotājiem ir jāapstiprina ziņojumi,](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) kas tiek nosūtīt pa e-pastu.

**E-pasta paziņojumi, kas tiek nosūtīti daudziem lietotājiem jūsu organizācijā**

Dažreiz vienu Yammer sūtīto paziņojumu saņems daudz lielāks lietotāju skaits jūsu organizācijā nekā plānots. Tas notiek, kad Yammer tiek pievienots izplatīšanas sarakts vai cita veida kopīgā e-pasta adrese. Yammer nespēj noteikt visos gadījumos, kad e-pasta adrese pieder vienam lietotājam un kad e-pasta adresi sūtītos paziņojumus saņems daudzi adresāti. Kad notiek šī problēma, jums ir jāveic nepieciešamās darbības, lai [apturētu (deaktivizētu) attiecīgā lietotāja nederīgās e-pasta adreses](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) darbību pakalpojumā Yammer. 

Lai samazinātu šīs problēmas rašanās iespējamību, veiciet tālāk norādītās darbības:

1. [Office 365 identitātes](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) ieviešana Yammer.
2. Bloķēt ārējos sūtītājus no e-pasta ziņojumu sūtīšanas jūsu organizācijai vai ierobežojiet sūtītāju skaitu ar apstiprināto sūtītāju sarakstu.

Ja notiek šī problēma:

1. Identificējiet e-pasta ziņojuma adresātu, kam ir jāatbilst Yammer lietotājam. Piemēram, all-in-sales@fabrikam.com ir visai pārdošanas nodaļai kopīga adrese. Šī kopīgā adrese būs identificējama no Yammer e-pasta ziņojuma, ko saņems lietotāji.
2. Izmantojiet [Tīkla administrēšanas deaktivizēšanas (darbības apturēšanas) līdzekli,](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) lai deaktivizētu lietotāju ar all-in-sales@fabrikam.com e-pasta adresi. Deaktivizēšanu ir iespējams atsaukt, tāpēc tā ir drošāka par dzēšanu. Lietotājs tiks automātiski dzēsts pēc 90 dienām.
3. Jūs varat izmantot [Lietotāju eksportēšanu](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers), lai identificētu citas e-pasta adreses, kuru darbība ir jāpārtrauc.
