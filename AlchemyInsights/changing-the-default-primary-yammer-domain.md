---
title: Noklusējuma Yammer domēna maiņa
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
- "9002662"
- "5162"
ms.openlocfilehash: dd29f2dc044fe4ee7f50acc6f0ca491d0ceb80bc360534de10d4010230614f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950123"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Noklusējuma/primārā Yammer domēna maiņa

Yammer vietrādis URL ietver pašreizējo primārā domēna nosaukumu jūsu Yammer tīklā. Šis domēna nosaukums, iespējams, neatbilst primārajam domēna nosaukumam, kas iestatīts Office 365 vai Azure Active Directory. Pastāv atšķirības uzvedībā, pamatojoties uz nomniekam pievienoto pielāgoto domēnu skaitu un to, vai Yammer ir atbalstītā konfigurācijā (1 nomnieks: 1 tīkls vai 1:1). Ir pieejama dokumentācija par [Yammer domēniem un Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains).

Visizplatītākais iemesls, kāpēc tiek rādīts nepareizs domēns, ir tas, ka pastāv vairāki Yammer tīkli un tie ir jākonsolidē. [Lai konsolidētu vienu tīkla](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks), tīkla migrēšanas rīka izmantošana ir svarīga pirmā darbība. Pirms mēģināt iestatīt primāro domēnu, izpildiet šo iespēju.

**Nav pielāgotu domēnu**

Jaunu nomnieku gadījumā pakalpojumā Yammer tiks lietots noklusējuma domēns (piemēram, fabrikam.onmicrosoft.com) no nomnieka. Primārais domēns ir iestatīts uz yammer.com/fabrikam.onmicrosoft.com.

**Viens pielāgots domēns**

Yammer automātiski atlasīs no nomnieka pielāgoto domēnu (piem., fabrikam.com) kā primāro domēnu pakalpojumā Yammer. Tas ir iestatīts uz yammer.com/fabrikam.com. Šīs izmaiņas jāveic domēna sinhronizācijas pakalpojumā, un var paiet līdz pat 24 stundām, līdz tās stājas spēkā.

**Vairāki pielāgoti domēni**

Yammer var izmantot primāro domēnu, kas atšķiras no noklusējuma nomnieka domēna. Tā kā ir vairāki pielāgoti domēni, Yammer necenšas uzminēt pareizo domēnu no pieejamajiem. Jums ir jāatver atbalsta pieteikums, lai pieprasītu primārā domēna nosaukuma maiņu uz primāro domēnu pēc savas izvēles.

**Papildu problēmu novēršanas informācija**

Dažos gadījumos domēni, iespējams, ir pārvietoti starp nomniekiem, un domēnu sinhronizācijas pakalpojums nevarēja sekmīgi darboties. Papildus nepareizajam primārajam domēnam var rasties pierakstīšanās vai citas problēmas. Lai atrisinātu šo problēmu, domēni, iespējams, ir jāpārvieto uz pareizo tīklu, izmantojot Microsoft atbalsta dienestu. Šai situācijai ir nepieciešama tieša palīdzība, un tas var ilgt kādu laiku, jo īpaši, ja ir ļoti liels domēnu nosaukumu saraksts. Atveriet atbalsta gadījumu, lai saņemtu palīdzību saistībā ar šāda veida problēmu novēršanu.

Strādājot ar atbalsta dienesta darbinieku, kas pārbaudīs, vai domēni ir verificēti nomniekā, kas atrodas jūsu kontrolē. Jums var tikt uzdoti papildu pārbaudes jautājumus par jūsu domēniem, ja tie tiek pievienoti jūsu nomniekam, bet nav verificēti ar DNS. Lūdzu, nodrošiniet, lai domēni tiktu verificēti, izmantojot DNS, kas paātrinās procesu.
