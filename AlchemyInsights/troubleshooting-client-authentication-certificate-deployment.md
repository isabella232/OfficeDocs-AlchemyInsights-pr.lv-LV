---
title: Klienta autentifikācijas sertifikātu izvietošanas problēmu novēršana
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
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658993"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Klienta autentifikācijas sertifikātu izvietošanas problēmu novēršana

Intune NDES/SCEP un PKCS/PFX klientu sertifikātu profili parasti tiek izmantoti kopā ar citiem profilu tipiem, piemēram, WiFi, VPN un e-pastu, lai lietotāji varētu veikt autentifikāciju korporatīvajos resursos. Ja šie profilu tipi ir saistīti ar klienta sertifikāta profilu, tie ir atkarīgi no šī profila sekmīgas izvietošanas.

Sākotnējai infrastruktūras iestatīšanai un saistītajai klienta sertifikāta profila konfigurācijai bieži ir nepieciešama problēmu novēršana. Detalizētus norādījumus par NDES savienotāja un problēmu novēršanas norādījumus, lai izolētu problēmas ar sertifikātu izvietošanu, skatiet: 

- [Infrastruktūras konfigurēšana, lai atbalstītu SCEP ar Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Pārskats par to, kā novērst SCEP sertifikātu profilus ar Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Izmantojiet atsauces PowerShell skriptus, lai verificētu savu konfigurāciju. Papildinformāciju skatiet rakstā [Intune Certificate Connector verifikācijas skripti](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Citas biežāk sastopamās problēmas**

**Kad mēģinu instalēt Intune Certificate Connector NDES Connector serverī, tiek parādīts ziņojums "nevar pārbaudīt sertifikāta pieprasījuma paroli. Tas, iespējams, jau ir izmantots. Iegūstiet jaunu paroli, ko iesniegt, izmantojot šo pieprasījumu.**  

Šis ziņojums nozīmē, ka ir jāpalaiž sertifikātu savienotāja instalācija kā administratoram.

Dažās vidēs serveros, kuros Intune sertifikāts darbojas, ir jāizmanto starpniekserveris, lai izveidotu savienojumu ar Intune, un tāpēc sertifikāta savienotājam ir jāizmanto starpniekserveris. Dažos gadījumos NDES savienotājs ignorē konfigurētos starpniekservera iestatījumus, un, izmantojot konts LocalSystem drošības kontekstu, var būt nepieciešams konfigurēt starpniekservera iestatījumus. 
 
Risinājums ir palaist Internet Explorer kā sistēmu un konfigurēt starpniekserveri IE. Pēc Intune savienotāja pakalpojuma restartēšanas NDES savienotājs izveido savienojumu ar Intune.

**Lietotāja ierīces vairs nesaņem SCEP sertifikātus no NDES.**

Ir iespējams, ka klienta autentifikācijas sertifikāts, kas tiek izdots NDES serverim un norādīts NDES savienotāja instalēšanas laikā, ir beidzies vai trūkst. Lai novērstu šo problēmu: 
 
1. Atinstalējiet NDES savienotāju.  
2. Izmantojiet šo detalizētu informāciju, lai pieprasītu jaunu klienta autentifikāciju vai servera autentifikācijas sertifikātu: 
 
    - Tēmas nosaukums: CN = ārējais FQDN  
    - Tēmas alternatīvais nosaukums (ir obligāti): DNS = ārējais FQDN, DNS = iekšējā FQDN 
 
3. Pārinstalējiet NDES savienotāju ar jauno sertifikātu.