---
title: Intune Exchange lokālajā savienotājā
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808136"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange lokālajā savienotājā

Lai uzzinātu, kā iestatīt savienotāju starp Intune un Exchange, kas tiek viesots lokāli, skatiet tālāk norādīto dokumentāciju.

[Intune lokālās Exchange Connector iestatīšana programmā Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**FAQ**

Jautājums: mēģinot iestatīt Exchange savienotāju, tiek rādīta kļūda, piemēram, "Exchange Connector versija netiek atbalstīta". Kāds varētu būt iemesls?

A: konts, kuru izmantojat, ir atbilstoši licencēts — tam ir jābūt Active Intune licencei

J: vai ir iespējams izmantot vairākus Exchange savienotājus?

A: jūs varat iestatīt tikai vienu Exchange Connector katram Intune nomniekam vienai Exchange organizācijai. Savienotāju var instalēt tikai vienā serverī vairāku serveru Exchange organizācijā.

Jūs arī nevarat būt konfigurēti savienotāji gan Exchange lokālajā, gan Exchange Online vienā nomniekā.

J: vai savienotājs var izmantot CAS masīvu kā tā savienojumu ar Exchange?

A: CAS masīva norādīšana nav atbalstīta konfigurācija savienotāja iestatījumos. Ir jābūt norādītam tikai vienam serverim, un tam jābūt hardcoded savienotāja konfigurācijas failā, ko var atrast

programmas data\microsoft\microsoft Intune lokālajā Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

Atrodiet šo ievadni ```<ExchangeWebServiceURL />``` un aizstājiet vietrādi URL ar Exchange serveri.

**Piemēram**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Papildinformāciju par problēmu novēršanu skatiet tālāk norādītajos dokumentos. [Intune problēmu novēršana lokālajā Exchange savienotājā](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Izvērstas reģistrēšanas iespējošana Exchange Connector**

1. Atveriet Exchange Connector trasēšanas konfigurācijas failu rediģēšanai.  
Fails atrodas:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Piemēram**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Atrodiet TraceSourceLine, izmantojot šādu atslēgu: OnPremisesExchangeConnectorService  
  
3. SourceLevel mezgla vērtības mainīšana no informācijas ActivityTracing (noklusējums) uz runīgs ActivityTracing  

**Piemēram**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Restartējiet Microsoft Intune Exchange pakalpojumu  
5. Pilna sinhronizācija Intune portālā, līdz tā ir pabeigta, un pēc tam nomainiet XML atpakaļ uz "informācijas ActivityTracing" un restartējiet Microsoft Intune Exchange pakalpojumu.  
6. Žurnālu atrašanās vieta ir: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`