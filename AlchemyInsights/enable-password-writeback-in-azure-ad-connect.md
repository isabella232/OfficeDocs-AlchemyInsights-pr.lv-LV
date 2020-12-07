---
title: Paroļu atpakaļrakstīšanas iespējošana Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560447"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Paroļu atpakaļrakstīšanas iespējošana Azure AD Connect

Lai iespējotu patstāvīgi izmantojamu paroles atiestatīšanas atpakaļrakstīšanu, vispirms Azure AD Connect iespējojiet atpakaļrakstīšanas opciju. Savā Azure AD Connect serverī veiciet tālāk minētās darbības:

1. Pierakstieties savā AD Connect serverī un palaidiet **Azure AD Connect** konfigurēšanas vedni.
2. **Sākuma** lapā noklikšķiniet uz **Konfigurēt**.
3. **Papildu uzdevumu** lapā atlasiet **Pielāgot sinhronizācijas opcijas** un noklikšķiniet uz **Tālāk**.
4. Lapā **Izveidot savienojumu ar Azure AD**, ievadiet jūsu Azure nomnieka globālā administratora akreditācijas datus un pēc tam noklikšķiniet **Tālāk**.
5. Filtrēšanas lapās **Connect direktoriji** un **Domēns/OU** noklikšķiniet uz **Tālāk**.
6. Lapā **Papildu līdzekļi**, atlasiet rūtiņu pie **Paroles atpakaļrakstīšana** un noklikšķiniet uz **Tālāk**.
7. Lapā **Gatavs konfigurēšanai** noklikšķiniet uz **Konfigurēt** un sagaidiet procesa beigas.
8. Kad tiks parādīta konfigurācija, noklikšķiniet uz **Iziet**.

Kad Azure AD Connect paroles atpakaļrakstīšana ir iespējota, konfigurējiet Azure AD SSPR atpakaļrakstīšanai.  Lai iespējotu SSPR paroles atpakaļrakstīšanu, veiciet tālāk minētās darbības: 

1. Ierakstieties Azure portālā ar globālā administratora kontu.
2. Meklējiet un atlasiet **Azure Active Directory**, noklikšķiniet uz **Paroles atiestatīšana**, pēc tam noklikšķiniet uz **Lokālā integrācija**.
3. Iestatiet opciju **Veikt paroļu atpakaļrakstīšanu jūsu lokālajam direktorijam?** kā **Jā**.
4. Iestatiet opciju **Ļaut lietotājiem atbloķēt kontus bez paroļu atiestatīšanas?** kā **Jā**.
5. Pēc tam noklikšķiniet uz **Saglabāt**.

Papildinformācijai lasiet [Azure Active Directory patstāvīgās paroles atiestatīšanas atpakaļrakstīšanas iespējošana lokālajā vidē](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Kad administrators atiestata lietotāja paroli Azure portālā, ja lietotājs ir federatīvs vai parole ir sinhronizēta ar jaucējkodu, parole tiek lokāli atpakļrakstīta. Šī funkcija pašlaik netiek atbalstīta Office administratora portālā.