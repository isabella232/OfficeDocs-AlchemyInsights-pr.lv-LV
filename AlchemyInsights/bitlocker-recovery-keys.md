---
title: BitLocker atkopšanas atslēgas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908821"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="636e1-102">Piekļūšana BitLocker atkopšanas atslēgām</span><span class="sxs-lookup"><span data-stu-id="636e1-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="636e1-103">Konfigurējot BitLocker iestatījumus InTune galapunkta aizsardzības politiku, ir iespējams noteikt, vai BitLocker atkopšanas informācija ir jāglabā Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="636e1-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="636e1-104">Ja šis iestatījums ir konfigurēts, saglabātos atkopšanas dati ir jābūt redzamai InTune admin kā daļa no ierīces ieraksta datu InTune ierīces asmens divos veidos:</span><span class="sxs-lookup"><span data-stu-id="636e1-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="636e1-105">Ierīces-Azure AD ierīces-> "ierīces" vai ierīces-> visas ierīces-> "ierīce"-> atkopšanas atslēgas</span><span class="sxs-lookup"><span data-stu-id="636e1-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="636e1-106">Alternatīvi, ja ir administratīva piekļuve pašai ierīcei, atkopšanas atslēgu (paroli) var redzēt, izpildot šādu komandu priviliģētā komandu uzvednē:</span><span class="sxs-lookup"><span data-stu-id="636e1-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="636e1-107">Ja ierīce ir šifrēta pirms reģistrācijas InTune, atkopšanas atslēga var būt saistīta ar "Microsoft konts" (PPL) izmanto, lai pierakstītos ierīces OOBE procesa laikā.</span><span class="sxs-lookup"><span data-stu-id="636e1-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="636e1-108">Ja tas tā ir, piekļūstot https://onedrive.live.com/recoverykey un pierakstoties ar šo MSA, ir jāparāda ierīces, kurām ir saglabātas atkopšanas atslēgas.</span><span class="sxs-lookup"><span data-stu-id="636e1-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="636e1-109">Ja ierīce tika šifrēta konfigurācijas dēļ ar grupas politiku, izmantojot domēnu, atkopšanas informāciju var saglabāt lokālo Active Directory.</span><span class="sxs-lookup"><span data-stu-id="636e1-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

