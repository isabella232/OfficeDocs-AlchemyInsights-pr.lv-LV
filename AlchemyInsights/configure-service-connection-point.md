---
title: Pakalpojumu savienojuma punkta konfigurēšana (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036145"
---
# <a name="configure-service-connection-point-scp"></a>Pakalpojumu savienojuma punkta konfigurēšana (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Iemesls**: nevar nolasīt SCP objektu un iegūt Azure AD nomnieka informāciju
- **Risinājums**: skatiet sadaļu [pakalpojumu savienojuma punkta konfigurēšana](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Darbību plāns**

- Pārbaudiet, vai ierīce ir saņēmusi kontrolētās validācijas GPO.
- Pārliecinieties, vai GPO ir izveidojis reģistra atslēgas.
- Pārliecinieties, vai jums ir 2 taustiņi, kas izveidoti ar jūsu direktorija ID un onmicrosoft domēnu.

**Klienta puses reģistra iestatījuma konfigurēšana SCP**

Izmantojiet tālāk norādīto piemēru, lai izveidotu grupas politikas objekta (GPO), lai izvietotu reģistra iestatījumu, kas konfigurē SCP ierakstu savu ierīču reģistrā.

1. Atveriet grupas politikas pārvaldības konsoli un izveidojiet jaunu GPO jūsu domēnā.
     - Nodrošiniet jaunizveidotā GPO nosaukumu (piemēram, ClientSideSCP)

2. Rediģējiet GPO un atrodiet šādu ceļu: **datora konfigurācija > Preferences > Windows iestatījumi > reģistru**.

3. Ar peles labo pogu noklikšķiniet uz **reģistrs** un atlasiet **Jauns > reģistra vienumu**.

4. Cilnē **Vispārīgi** konfigurējiet tālāk norādītās darbības.
  
- **Darbība**: atjaunināšana
    
- **Strops**: HKEY_LOCAL_MACHINE
    
- **Atslēgas ceļš**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Vērtības nosaukums**: TenantId
    
- **Vērtības tips**: REG_SZ
    
- **Vērtību dati**: Azure AD instances GUID vai direktorija ID (šī vērtība var atrast **Azure portālā > azure Active Directory > REKVIZĪTIEM > direktorija ID**)
 
- Noklikšķiniet uz **Labi**.
 
5. Ar peles labo pogu noklikšķiniet uz **reģistrs** un atlasiet **Jauns > reģistra vienumu**.

6. Cilnē **Vispārīgi** konfigurējiet tālāk norādītās darbības.
  
- **Darbība**: atjaunināšana
    
- **Strops**: HKEY_LOCAL_MACHINE
    
- **Atslēgas ceļš**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Vērtības nosaukums**: TenantName
    
- **Vērtības tips**: REG_SZ
    
- **Vērtības dati**: jūsu Verificētais domēna nosaukums, ja izmantojat Federatīvo vidi, piemēram, AD FS. Jūsu Verificētais domēna nosaukums vai jūsu onmicrosoft.com domēna nosaukums (piemēram, contoso. onmicrosoft). com, ja izmantojat pārvaldītu vidi

- Noklikšķiniet uz **Labi**.

7. Jāslēdz jaunizveidotā GPO redaktors.

8. Saistiet jaunizveidoto GPO ar vēlamo OU, kas ietver domēnu, kas pieder jūsu kontrolētajiem izvēršanas iedzīvotājiem.

Lai iegūtu papildinformāciju, skatiet rakstu [Hibrīdā AZURE ad Join-AZURE ad savienojuma pārbaude | Microsoft dokumenti](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) un  [problēmu novēršanas Hibrīdā Azure Active Directory pievienotās ierīces | Microsoft dokumenti](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









