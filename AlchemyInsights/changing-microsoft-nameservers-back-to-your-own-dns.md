---
title: Pāreja no Microsoft nosaukumu serveriem atpakaļ uz savu DNS ierakstu pārvaldību
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506607"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Pāreja no Microsoft nosaukumu serveriem atpakaļ uz savu DNS ierakstu pārvaldību

Iepriekš esat mainījis savus NS ierakstus, lai tie norāda uz Microsoft (ns1.bdm.microsoftonline.com), taču tagad esat izlēmis pārvaldīt savus DNS ierakstus:

Domēnu reģistrētāja tīmekļa vietnē mainiet nosaukumu serveri atpakaļ uz reģistrētāju vai iepriekšējo iestatījumu. Ja nepārzināt DNS darbības, sazinieties ar atbalsta dienestu pie domēnu reģistrētāja. Ņemiet vērā, ka nosaukumu serveru izmaiņas var izplatīties līdz 48 stundām. 

1. Administrēšanas Microsoft 365 dodieties uz Iestatījumi   >  [**Domēni**](https://admin.microsoft.com/Adminportal/Home#/Domains), atzīmējiet izvēles rūtiņu blakus domēnam un atlasiet **Pārvaldīt DNS**. 

2. Vednī atlasiet Pievienot **savus DNS ierakstus un** pabeidziet darbības vednī. Tādējādi tiek mainīts jūsu DNS pārvaldības veids, un jūs varat pievienot pielāgotos DNS ierakstus, kas nepieciešami atlasīto pakalpojumu atbalstam.

Vai arī, ja mainīsit nosaukumu servera ierakstus uz Microsoft un jums ir tīmekļa vietne, varat pievienot tīmekļa vietnes DNS ierakstus, nevis mainīt nosaukumu serverus atpakaļ. Papildinformāciju skatiet rakstā [DNS ierakstu atjaunināšana, lai tīmekļa vietni uzturētu pie pašreizējā viesošanas pakalpojumu sniedzēja.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


