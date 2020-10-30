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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="0b2b1-102">Intune Exchange lokālajā savienotājā</span><span class="sxs-lookup"><span data-stu-id="0b2b1-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="0b2b1-103">Lai uzzinātu, kā iestatīt savienotāju starp Intune un Exchange, kas tiek viesots lokāli, skatiet tālāk norādīto dokumentāciju.</span><span class="sxs-lookup"><span data-stu-id="0b2b1-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="0b2b1-104">Intune lokālās Exchange Connector iestatīšana programmā Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="0b2b1-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="0b2b1-105">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="0b2b1-105">**FAQ:**</span></span>

<span data-ttu-id="0b2b1-106">Jautājums: mēģinot iestatīt Exchange savienotāju, tiek rādīta kļūda, piemēram, "Exchange Connector versija netiek atbalstīta".</span><span class="sxs-lookup"><span data-stu-id="0b2b1-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="0b2b1-107">Kāds varētu būt iemesls?</span><span class="sxs-lookup"><span data-stu-id="0b2b1-107">What could be the cause?</span></span>

<span data-ttu-id="0b2b1-108">A: konts, kuru izmantojat, ir atbilstoši licencēts — tam ir jābūt Active Intune licencei</span><span class="sxs-lookup"><span data-stu-id="0b2b1-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="0b2b1-109">J: vai ir iespējams izmantot vairākus Exchange savienotājus?</span><span class="sxs-lookup"><span data-stu-id="0b2b1-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="0b2b1-110">A: jūs varat iestatīt tikai vienu Exchange Connector katram Intune nomniekam vienai Exchange organizācijai.</span><span class="sxs-lookup"><span data-stu-id="0b2b1-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="0b2b1-111">Savienotāju var instalēt tikai vienā serverī vairāku serveru Exchange organizācijā.</span><span class="sxs-lookup"><span data-stu-id="0b2b1-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="0b2b1-112">Jūs arī nevarat būt konfigurēti savienotāji gan Exchange lokālajā, gan Exchange Online vienā nomniekā.</span><span class="sxs-lookup"><span data-stu-id="0b2b1-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="0b2b1-113">J: vai savienotājs var izmantot CAS masīvu kā tā savienojumu ar Exchange?</span><span class="sxs-lookup"><span data-stu-id="0b2b1-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="0b2b1-114">A: CAS masīva norādīšana nav atbalstīta konfigurācija savienotāja iestatījumos.</span><span class="sxs-lookup"><span data-stu-id="0b2b1-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="0b2b1-115">Ir jābūt norādītam tikai vienam serverim, un tam jābūt hardcoded savienotāja konfigurācijas failā, ko var atrast</span><span class="sxs-lookup"><span data-stu-id="0b2b1-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="0b2b1-116">programmas data\microsoft\microsoft Intune lokālajā Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="0b2b1-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="0b2b1-117">Atrodiet šo ievadni ```<ExchangeWebServiceURL />``` un aizstājiet vietrādi URL ar Exchange serveri.</span><span class="sxs-lookup"><span data-stu-id="0b2b1-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="0b2b1-118">**Piemēram**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="0b2b1-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="0b2b1-119">Papildinformāciju par problēmu novēršanu skatiet tālāk norādītajos dokumentos. [Intune problēmu novēršana lokālajā Exchange savienotājā](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="0b2b1-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="0b2b1-120">**Izvērstas reģistrēšanas iespējošana Exchange Connector**</span><span class="sxs-lookup"><span data-stu-id="0b2b1-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="0b2b1-121">Atveriet Exchange Connector trasēšanas konfigurācijas failu rediģēšanai.</span><span class="sxs-lookup"><span data-stu-id="0b2b1-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="0b2b1-122">Fails atrodas:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="0b2b1-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="0b2b1-123">**Piemēram**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="0b2b1-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="0b2b1-124">Atrodiet TraceSourceLine, izmantojot šādu atslēgu: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="0b2b1-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="0b2b1-125">SourceLevel mezgla vērtības mainīšana no informācijas ActivityTracing (noklusējums) uz runīgs ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="0b2b1-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="0b2b1-126">**Piemēram**</span><span class="sxs-lookup"><span data-stu-id="0b2b1-126">**Example:**</span></span>
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
4. <span data-ttu-id="0b2b1-127">Restartējiet Microsoft Intune Exchange pakalpojumu</span><span class="sxs-lookup"><span data-stu-id="0b2b1-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="0b2b1-128">Pilna sinhronizācija Intune portālā, līdz tā ir pabeigta, un pēc tam nomainiet XML atpakaļ uz "informācijas ActivityTracing" un restartējiet Microsoft Intune Exchange pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="0b2b1-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="0b2b1-129">Žurnālu atrašanās vieta ir: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="0b2b1-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>