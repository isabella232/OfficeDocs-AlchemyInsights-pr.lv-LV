---
title: Klienta autentifikācijas sertifikāta izvietošanas problēmu novēršana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020811"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Klienta autentifikācijas sertifikāta izvietošanas problēmu novēršana

Intune NDES/SCEP un PKCS/PFX klienta sertifikātu profili parasti tiek izmantoti kopā ar citiem profilu veidiem, piemēram, Wi-Fi, VPN un e-pastu, lai lietotājiem ļautu veikt autentifikāciju uzņēmuma resursos. Ja šie profilu tipi ir saistīti ar klienta sertifikāta profilu, tie ir atkarīgi no šī profila sekmīgās izvietošanas.

Bieži vien ir jānovērš problēmas saistībā ar sākotnējo infrastruktūras iestatīšanu un saistīto klienta sertifikāta profila konfigurāciju. Lai skatītu deizvēršanas ceļvedi par NDES savienotāja sekmīgu iestatīšanu un problēmu novēršanas norādījumus, lai izolētu problēmas ar sertifikātu izvietošanu, skatiet: 

- [Infrastruktūras konfigurēšana SCEP atbalstam ar Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Pārskats par problēmu novēršanu saistībā ar SCEP sertifikātu profiliem, izmantojot Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Izmantojiet powershell skriptus, uz kuriem ir atsauces, lai pārbaudītu konfigurāciju. Papildinformāciju skatiet rakstā [Intune sertifikāta savienotāja verifikācijas skripti.](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)

  
**Citas bieži sastopamas problēmas**

**Mēģinot instalēt Intune sertifikāta savienotāju NDES savienotāja serverī, tiek parādīts ziņojums "Paroli sertifikāta pieprasījumā nevar pārbaudīt. Iespējams, tas jau ir izmantots. Iegūstiet jaunu paroli, lai iesniegtu ar šo pieprasījumu."**  

Šis ziņojums nozīmē, ka ir jāpalaiž sertifikāta savienotāja instalācija kā administratoram.

Dažās vidēs serveros, kur tiek palaists Intune sertifikāts, ir jāizmanto starpniekserveris, lai izveidotu savienojumu ar Intune, un tāpēc sertifikāta savienotājam ir jāizmanto starpniekserveris. Dažos gadījumos NDES savienotājs ignorē konfigurētos starpniekservera iestatījumus, un var būt nepieciešams konfigurēt starpniekservera iestatījumus, kamēr tie darbojas LocalSystem drošības kontekstā. 
 
Risinājums ir palaist Internet Explorer kā SYSTEM un konfigurēt starpniekserveri pārlūkprogrammā IE. Pēc Intune savienotāja pakalpojuma restartēšanas NDES savienotājs izveido savienojumu ar Intune.

**Lietotāju ierīces vairs nesaņem SCEP sertifikātus no NDES.**

Iespējams, ka klienta autentifikācijas sertifikātam, kas izsniegts NDES serverim un ir norādīts NDES savienotāja instalēšanas laikā, ir beidzies derīgums vai tā trūkst. Lai atrisinātu: 
 
1. Atinstalējiet NDES savienotāju.  
2. Izmantojiet šo detalizēto informāciju, lai pieprasītu jaunu klienta autentifikāciju vai servera autentifikācijas sertifikātu: 
 
    - Tēmas nosaukums: CN=external fqdn  
    - Tēmas alternatīvais nosaukums (abi ir obligāti): DNS=external fqdn, DNS=internal fqdn 
 
3. Atkārtoti instalējiet NDES savienotāju ar jauno sertifikātu.