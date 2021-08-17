---
title: Enterprise lietojumprogrammu saraksta izveide
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116735"
---
# <a name="get-a-list-of-enterprise-applications"></a>Enterprise lietojumprogrammu saraksta izveide

1. Lai **iegūtu** sarakstu ar uzņēmuma lietojumprogrammām (visas lietojumprogrammas vai filtrētas pēc parādāmā vārda, ID, identifikatoru URI u.c.), izmantojot Powershell komandu, skatiet rakstu [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Lai iegūtu pakalpojuma pamatobjektu sarakstu (visus objektus vai atfiltrējot pēc ID), izmantojot Powershell komandu, skatiet rakstu [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Ja vēlaties iegūt **SAML konfigurēto programmu sarakstu,** tālāk norādītās PowerShell skripti var palīdzēt:

    Katrā lietojumprogrammā (OAuth programmā vai SAML programmā (gan galerijā, gan programmās, kas nav galerijas) būtu divi objekti, kas tiek izveidoti AAD, kad notiek to reģistrācija. Viens tiek dēvēts par lietojumprogrammas objektu, bet otra — objekts Service Principal. Kad, izmantojot PowerShell, izmantojat pakalpojuma pamat objekta rekvizītus, katrai lietojumprogrammai ir piesaistīts noteikts skaits ar to saistīto atzīmju:

    - OAuth programmām būtu atzīme "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Galerija SAML lietojumprogrammām būtu atzīme **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Bez galerijas SAML lietojumprogrammām būtu atzīme **"WindowsAzureActiveDirectoryCustomSingleSignOnApplication"**

    Tādējādi varat izmantot šīs atzīmes un uzzināt, kāda programma tā ir. Atzīme "**WindowsAzureActiveDirectoryIntegratedApp**" tiek bieži lietots visu veidu programmām. Lai uzskaitītu visas SAML programmas (gan galerijā, gan ārpus galerijas), varat izmantot tālāk norādīto fragmentu.

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Papildinformāciju skatiet rakstā [SamL iespējoto programmu identificēšana pakalpojumā Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Tikai tīmekļa lietojumprogrammu atrašana** un saraksts: izmantojiet tālāk norādīto komandu, lai iegūtu visas Azure AD lietojumprogrammas ar lietojumprogrammas tipu "Tīmekļa lietojumprogramma/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Atrodiet un uzziniet tikai vietējās lietojumprogrammas:** izpildiet tālāk norādīto komandu, lai iegūtu visas vietējās klienta (darbvirsmas/mobilās ierīces) lietojumprogrammas.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Eksportēt visu reģistrēto Azure AD lietojumprogrammas informāciju CSV** failā: tālāk redzama komanda eksportē visas Azure AD programmas ar nepieciešamo informāciju csv failā:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Nepieciešams eksportēt neizmantoto Azure programmu sarakstu** — audita atskaite

    Azure AD var parādīt programmu žurnālus tikai līdz 30 dienām, ja jums ir Azure AD Premium licence.
    Ir divas iespējas saglabāt datus ilgāk par 30 dienām. Varat izmantot [Azure AD atskaišu API, lai](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) programmiski izgūtu datus un glabātu tos datu bāzē. Varat arī integrēt audita žurnālus trešās puses SIEM sistēmā.

    Varat arī lejupielādēt lietojumprogrammu sarakstu visām lietojumprogrammām un piederošām lietojumprogrammām Azure Active Directory>programmu reģistrācijas>lejupielādēt>visas lietojumprogrammas/piederošās lietojumprogrammas.

    Lai iegūtu lietojumprogrammu sarakstu, izmantojot MS Graph, skatiet rakstu Sarakstu lietojumprogrammas [— Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) un lietojumprogrammas resursa tips [— Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
