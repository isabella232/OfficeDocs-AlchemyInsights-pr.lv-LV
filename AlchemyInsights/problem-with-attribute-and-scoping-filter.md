---
title: Problēma ar atribūtu un tvēruma filtru
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481894"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problēma ar atribūtu un tvēruma filtru

**Problēma ar konfliktējošām UPN vērtībām**

Darba diena līdz AD lietotājam, kas nodrošina funkciju WORKDAY uz reklāmu lietotāju nodrošinājums, rāda kļūdas ziņojuma **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**. Operācija neizdevās, jo UPN vērtība, kas ir nodrošināta pievienošana/modificēšana, nav unikāls meža mērogs. Detalizēta informācija par kļūdu: **CONSTRAINT_ATT_TYPE-userPrincipalName**.

**UserPrincipalName** vērtība, ko WORKDAY Connector mēģina iestatīt, veidojot ad lietotāja kontu, jau ir iekļauta Target ad domēnā. Tas nozīmē, ka (1) lietotājs jau pastāv un atbilstošo ID pārbaude neizdevās lietotājam vai (2) UPN ģenerēšanas kārtula ģenerēja konfliktējošu vērtību.

Tālāk ir norādītas ieteicamās risinājuma darbības.

Ja lietotājs jau pastāv un atbilstošo ID pārbaude neizdevās saistīt darba dienu kontu ar Active Directory kontu, pēc tam pārbaudiet, vai atbilstības ID atribūts (parasti **employeeID**) gan WORKDAY, gan ad ir precīza atbilstība. Ja viņiem nav atbilstību, tas nozīmē, ka ir nepieciešams novērst datu problēmu. Piemēram, ja EmployeeID darbdienā ir 001052 un REKLĀMā tas ir 1052, tad nodrošināšanas programmai neizdosies sasaistīt šos divus kontus un mēģinās izveidot lietotāju, kas jau pastāv. Šajā gadījumā risinājums ir mainīt **EmployeeID** vērtību reklāmā, lai iekļautu sākuma nulles, lai padarītu to 001052.
Ja UPN ģenerētajā izteiksmē netiek ģenerēta unikāla vērtība, apsveriet iespēju izmantot funkciju **SelectUniqueValue** , lai katru reizi ģenerētu unikālu vērtību.

**Funkcija WORKDAY līdz AD lietotāja nodrošinājumam neiestata pārvaldnieka atribūta vērtību AD lietotāja kontam**

Funkcija WORKDAY uz AD lietotāju nodrošināšanas darbu neiestata **pārvaldnieka** atribūta vērtību ad lietotāju kontiem. Ir iespējami divi scenāriji, kad šāda darbība ir redzama:

1. Vadītāju darba dienās nevar atrisināt atbilstošajā AD lietotāja kontā, jo nav šī pārvaldnieka tvēruma.
2. **Vairāku ad domains** scenārijs: vadītājs, kas ir WORKDAY, neatrodas tajā pašā domēnā, kur lietotājs.

Lai atrisinātu šo problēmu, veiciet tālāk norādītās darbības.

1. Ja esat definējis tvēruma filtrus, vispirms pārbaudiet, vai vadītājs ir tvērumā un vai tas atbilst klauzulai tvērums. Ja vadītājs neapmierina tvēruma filtru, mainiet filtru tā, lai vadītājs būtu arī nodrošināšanas darbības sfērā.
2. Ja jums ir vairāki AD domēni, savienotāja ir zināms ierobežojums nespējai atrisināt starpdomēnu pārvaldnieka atsauces.

Lai iegūtu papildinformāciju par to, kā konfigurēt darba dienu automatizētai konfigurēšanai, skatiet rakstu [apmācība: darbdienas konfigurēšana automātiskai lietotāju nodrošināšanai](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).













