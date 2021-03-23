---
title: Lietotāju pārvaldības problēmas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036285"
---
# <a name="user-management-issues"></a>Lietotāju pārvaldības problēmas

**Kas notiek ar pašreizējiem piešķirtajiem lietotājiem uz lietojumprogrammu, ja tiek atspējota rekvizīta lietotāja uzdevuma piešķiršana (iestatīt šo rekvizītu uz Nē)?**

**Lietotāja uzdevuma atspējošana obligāts** neietekmē pašlaik piešķirtos lietotājus. Atspējojot šo rekvizītu, visiem lietotājiem tiks atļauts piekļūt lietojumprogrammai. Visi sarakstā uzskaitītie lietotāji un lietotāji, kas ir piešķirti lietojumprogrammas, joprojām būs derīgi.

- Lai programmu ierobežotu ar konkrētu lietotāju kopu, skatiet rakstu [AZURE ad lietojumprogrammas ierobežošana lietotāju grupā — Microsoft identitātes platforma | Microsoft dokumenti](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Lai lietotājiem un grupām piešķirtu uzņēmuma lietojumprogrammas Azure Active Directory (Azure AD), vai nu Azure portālā vai izmantojot PowerShell, skatiet rakstu [lietotāja piešķires izveide programmai Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Lai deleģētu lietojumprogrammu izveides un pārvaldības atļaujas, skatiet rakstu [pārstāvja lietojumprogrammu pārvaldības administratora atļaujas — AZURE ad | Microsoft dokumenti](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Paslēpiet noteiktas uzņēmuma lietojumprogrammas no lietotājiem** — veiciet tālāk norādītās darbības, lai paslēptu visas Microsoft 365 programmas no **manas programmas** paneļa. Lietojumprogrammas joprojām būs redzamas Office 365 portālā.

 1. Pierakstieties Azure portālā kā globālais administrators jūsu direktorijā. 
 2. Atlasiet **Azure Active Directory**. 
 3. Atlasiet **lietotāji**. 
 4. Atlasiet **lietotāja iestatījumi**. 
 5. Sadaļā **uzņēmuma lietojumprogrammas** noklikšķiniet uz **Pārvaldīt, kā lietotāji palaidīs un skatīt savas lietojumprogrammas**. 
 6. **Lietotājiem var skatīt tikai office 365 lietojumprogrammas office 365 portālā**, noklikšķiniet uz **Jā**. 
 7. Noklikšķiniet uz **Saglabāt**. 
 8. Papildinformāciju skatiet rakstā [uzņēmuma lietojumprogrammas paslēpšana no lietotāja pieredzes pakalpojumā AZURE ad | Microsoft dokumenti](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Ja programmu kā pakalpojumu (SaaS) piedāvājat daudzām organizācijām, varat to konfigurēt, lai akceptētu pierakstīšanās no jebkura Azure Active Directory (Azure AD) nomnieka. Šī konfigurācija tiek dēvēta par lietojumprogrammas vairāku nomnieku veidošanu. Jebkurā Azure AD nomnieka lietotāji varēs pierakstīties savā lietojumprogrammā pēc tam, kad tā ir pieprasījusi izmantot savu kontu lietojumprogrammā. Papildinformāciju skatiet rakstā [lietojumprogrammu izveide, kas pierakstīšanās AZURE ad lietotājiem — Microsoft identitātes platforma | Microsoft dokumenti](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Kā lietotājs var piekļūt lietojumprogrammai, tiklīdz tas ir piešķirts lietojumprogrammai?**

Katrai lietojumprogrammai uzņēmuma lietojumprogrammas diskam ir saite lietotājiem, lai piekļūtu. Lietotāji var piekļūt programmai arī, izmantojot **manas programmas** portālu.

- **Vai vēlaties uzzināt, kuras lietojumprogrammas un tipa lietojumprogrammas izmanto lietotāji?**

Varat lejupielādēt pierakstīšanās atskaites par pēdējām 30 dienām no **portal.azure.com > Azure Active directory> Signins> lejupielādētu atskaites**.

- Uzziniet, kā [piešķirt nomnieka plaša administratora piekrišanu lietojumprogrammai](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) un [konfigurēt, kā lietotāji piekrīt lietojumprogrammām](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Saprast, [kā darbojas piekrišana](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) un [Pārvaldīt piekrišana lietojumprogrammām](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


