---
title: Intune Exchange lokālā savienotāja
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013971"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange lokālā savienotāja

Detalizētu informāciju par savienotāja iestatīšanu starp Intune un Exchange, kas tiek viesota lokāli, skatiet tālāk redzamajā dokumentācijā.

[Intune lokālā savienotāja iestatīšana Exchange programmā Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Bieži uzdotie jautājumi:**

Problēma: mēģinot iestatīt savienotāju, tiek Exchange Exchange kļūda "Savienotāja Exchange netiek atbalstīta". Kāds varētu būt iemesls?

A: jūsu izmantotais konts ir atbilstoši licencēts — kontam ir jābūt aktīvai Intune licencei

J: Vai iespējams izmantot vairākus savienotājus Exchange savienojumus?

A: Varat iestatīt tikai vienu savienotāju Exchange katrai Intune nomniekam katrā Exchange organizācijā. Savienotāju var instalēt tikai vienā serverī vairāku serveru exchange organizācijā.

Arī savienotāji nevar būt konfigurēti gan lokālajiem Exchange gan citiem Exchange Online konfigurētiem vienā nomniekā.

J: Vai savienotājs var izmantot CAS masīvu kā tā savienojumu ar Exchange?

A. CAS masīva norādīšana savienotāja iestatīšanā netiek atbalstīta. Ir jānorāda tikai viens serveris, un tam ir jābūt hardcoded savienotāja konfigurācijas failā, ko var atrast

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Atrodiet tālāk norādīto ierakstu ```<ExchangeWebServiceURL />``` un aizstājiet URL ar Exchange serveri.

**Piemērs:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Lai saņemtu papildu problēmu novēršanas informāciju, skatiet šo dokumentāciju: [Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune) lokālā savienotāja Exchange problēmu novēršana

**Verbose reģistrēšanas iespējošana Exchange savienotājam**

1. Atveriet Exchange savienotāja trasēšanas konfigurācijas failu rediģēšanai.  
Fails atrodas šeit: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Piemērs:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Atrodiet TraceSourceLine ar šādu atslēgu: OnPremisesExchangeConnectorService  
  
3. Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing  

**Piemērs:**
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
5. Pilnīga sinhronizācija Intune portālā, līdz tā tiek pabeigta, un pēc tam mainiet XML atpakaļ uz "Informācijas aktivitāšu trasēšana" un restartējiet Microsoft Intune Exchange pakalpojumu.  
6. Žurnālu atrašanās vieta ir: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`