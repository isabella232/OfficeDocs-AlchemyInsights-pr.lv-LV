---
title: Klienta autentifikācijas sertifikātu izvietošanas problēmu novēršana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555306"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="15749-102">Klienta autentifikācijas sertifikātu izvietošanas problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="15749-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="15749-103">Intune NDES/SCEP un PKCS/PFX klientu sertifikātu profili parasti tiek izmantoti kopā ar citiem profilu tipiem, piemēram, WiFi, VPN un e-pastu, lai lietotāji varētu veikt autentifikāciju korporatīvajos resursos.</span><span class="sxs-lookup"><span data-stu-id="15749-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="15749-104">Ja šie profilu tipi ir saistīti ar klienta sertifikāta profilu, tie ir atkarīgi no šī profila sekmīgas izvietošanas.</span><span class="sxs-lookup"><span data-stu-id="15749-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="15749-105">Sākotnējai infrastruktūras iestatīšanai un saistītajai klienta sertifikāta profila konfigurācijai bieži ir nepieciešama problēmu novēršana.</span><span class="sxs-lookup"><span data-stu-id="15749-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="15749-106">Detalizētus norādījumus par NDES savienotāja un problēmu novēršanas norādījumus, lai izolētu problēmas ar sertifikātu izvietošanu, skatiet:</span><span class="sxs-lookup"><span data-stu-id="15749-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="15749-107">Infrastruktūras konfigurēšana, lai atbalstītu SCEP ar Intune</span><span class="sxs-lookup"><span data-stu-id="15749-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="15749-108">Pārskats par to, kā novērst SCEP sertifikātu profilus ar Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="15749-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="15749-109">Izmantojiet atsauces PowerShell skriptus, lai verificētu savu konfigurāciju.</span><span class="sxs-lookup"><span data-stu-id="15749-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="15749-110">Papildinformāciju skatiet rakstā [Intune Certificate Connector verifikācijas skripti](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="15749-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="15749-111">**Citas biežāk sastopamās problēmas**</span><span class="sxs-lookup"><span data-stu-id="15749-111">**Other common issues**</span></span>

<span data-ttu-id="15749-112">**Kad mēģinu instalēt Intune Certificate Connector NDES Connector serverī, tiek parādīts ziņojums "nevar pārbaudīt sertifikāta pieprasījuma paroli. Tas, iespējams, jau ir izmantots. Iegūstiet jaunu paroli, ko iesniegt, izmantojot šo pieprasījumu.**</span><span class="sxs-lookup"><span data-stu-id="15749-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="15749-113">Šis ziņojums nozīmē, ka ir jāpalaiž sertifikātu savienotāja instalācija kā administratoram.</span><span class="sxs-lookup"><span data-stu-id="15749-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="15749-114">Dažās vidēs serveros, kuros Intune sertifikāts darbojas, ir jāizmanto starpniekserveris, lai izveidotu savienojumu ar Intune, un tāpēc sertifikāta savienotājam ir jāizmanto starpniekserveris.</span><span class="sxs-lookup"><span data-stu-id="15749-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="15749-115">Dažos gadījumos NDES savienotājs ignorē konfigurētos starpniekservera iestatījumus, un, izmantojot konts LocalSystem drošības kontekstu, var būt nepieciešams konfigurēt starpniekservera iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="15749-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="15749-116">Risinājums ir palaist Internet Explorer kā sistēmu un konfigurēt starpniekserveri IE.</span><span class="sxs-lookup"><span data-stu-id="15749-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="15749-117">Pēc Intune savienotāja pakalpojuma restartēšanas NDES savienotājs izveido savienojumu ar Intune.</span><span class="sxs-lookup"><span data-stu-id="15749-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="15749-118">**Lietotāja ierīces vairs nesaņem SCEP sertifikātus no NDES.**</span><span class="sxs-lookup"><span data-stu-id="15749-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="15749-119">Ir iespējams, ka klienta autentifikācijas sertifikāts, kas tiek izdots NDES serverim un norādīts NDES savienotāja instalēšanas laikā, ir beidzies vai trūkst.</span><span class="sxs-lookup"><span data-stu-id="15749-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="15749-120">Lai novērstu šo problēmu:</span><span class="sxs-lookup"><span data-stu-id="15749-120">To resolve:</span></span> 
 
1. <span data-ttu-id="15749-121">Atinstalējiet NDES savienotāju.</span><span class="sxs-lookup"><span data-stu-id="15749-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="15749-122">Izmantojiet šo detalizētu informāciju, lai pieprasītu jaunu klienta autentifikāciju vai servera autentifikācijas sertifikātu:</span><span class="sxs-lookup"><span data-stu-id="15749-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="15749-123">Tēmas nosaukums: CN = ārējais FQDN</span><span class="sxs-lookup"><span data-stu-id="15749-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="15749-124">Tēmas alternatīvais nosaukums (ir obligāti): DNS = ārējais FQDN, DNS = iekšējā FQDN</span><span class="sxs-lookup"><span data-stu-id="15749-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="15749-125">Pārinstalējiet NDES savienotāju ar jauno sertifikātu.</span><span class="sxs-lookup"><span data-stu-id="15749-125">Reinstall the NDES connector with the new certificate.</span></span>