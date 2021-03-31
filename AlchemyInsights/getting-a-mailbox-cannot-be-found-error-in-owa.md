---
title: 126 Vai programmā OWA nevar atrast pastkastes iegūšanas kļūdu?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426669"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Vai programmā Outlook tīmeklī tiek atrasta kļūda pastkastē?

Ja izmantojat Outlook tīmeklī un saņemat  kļūdas ziņojumu par pastkasti, kontam, kuru izmantojāt, lai izveidotu savienojumu ar Outlook tīmeklī, nav Exchange Online licences un tāpēc ar kontu nav saistīta neviena pastkaste. Administrators var piešķirt licenci jūsu kontam, veicot tālāk norādītās darbības.

1. Atveriet [Microsoft 365 administrēšanas centru,](https://portal.office.com/adminportal/home#/homepage) sadaļā  Lietotāji dodieties uz sadaļu Aktīvie lietotāji un atlasiet lietotāju, kuram tiek rādīta kļūda. 

2. Atvērtajā lietotāja lapā dodieties uz sadaļu Licences un  programmas, atlasiet atbilstošo vērtību **Atrašanās** vieta un piešķiriet licenci, kas satur Exchange Online (izvērsiet licenci, lai skatītu detalizētu informāciju par to). Kad esat pabeidzis, noklikšķiniet uz **Saglabāt izmaiņas.**

Dažos gadījumos, ja licence jau ir piešķirta lietotāja kontam, licences noņemšana un atkārtota piešķiršana palīdz novērst problēmu un nodrošināt to pareizi sistēmā: 

- Pārbaudiet, vai jūsu M365 Exchange Online (un citi, ja jums ir) abonementi ir pašreizējie un nav nesen beidzies derīgums.

Kad esat pārliecināts, ka jūsu abonementa derīgums nav beidzies un lietotāja kontam ir piešķirta derīga licence, var paiet līdz pat 24 stundām, līdz licence tiek nodrošināta, tāpēc, iespējams, būs jāgaida, līdz problēma tiks atrisināta. Papildinformāciju skatiet [rakstā Licenču piešķiršana un pārvaldība.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)