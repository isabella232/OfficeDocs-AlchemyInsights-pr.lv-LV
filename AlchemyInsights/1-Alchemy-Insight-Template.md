---
title: Tāpat kā filename ir labākais
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: ec979c2f2246fa06945b79bbb9348a7a57ad5180
ms.sourcegitcommit: b3cf5130ac8118f0fed66abe5286aa80ee91af52
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2019
ms.locfileid: "30683856"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Vajadzīga alķīmija Header H1, H2 ir nestrādā.
Labāko praksi un pamatnostādnēm par alķīmiju autorēšanas:

1. **Neligzdo Alchemy atziņas mapēs**- tas saplīst url struktūru. Mēs meklēja šo noteikšanu.
1. Failus mapē **AlchemyInsights** vajadzētu būt mazie filenames ar telpām ex pārnesumzīmes. ***how-to-enable-tiesvedības-turiet***.
    1. Ietver kārtulas ID vai kopuma ID no [alķīmijas partneru portāla](https://alchemyportal.azurewebsites.net) ms.custom laukā. ex. ***MS.Custom: 100021***
1. Izmantot metadatu atlikušo augšpusē šo failu kā veidnei.
1. [Alchemy partneru portāla](https://alchemyportal.azurewebsites.net)virzītos uz leju līdz sadaļai **klientu ieskatu nosaukums:** un izmantot šo kā sākuma punkts H1 titra par ieskatu. 
    > [!NOTE]
    > Alķīmijas atziņas ir jābūt tikai vienu H1 augšpusē vai viņi pārtrauks ražošanu. H2s nepadara tik lietot **treknraksta** vai citām konvencijām neizsaka atsevišķās sekcijās.
1. Pēc tam aizpildiet pamattekstu, izmantojot iesaukumam Alchemy noteikums lapas sadaļā klientu atziņas
    1. Aizzīmētiem sarakstiem ir smalka
    1. Numurētus sarakstus pārāk
    1. **Treknraksts** un *kursīvs* , tiek a-ok
    1. Saites, vienmēr ir jābūt vai nu **"uz web saites" / ārējo** vai **dziļas saites uz lietotāja interfeisa elementus**, nevis iekšējās saites.
    1. Attēli nav oficiāli atbalstīti šajā laikā, bet tas ir par plānu.

Un tas tiešām jau ir mazliet pārāk ilgi. Vislabākā prakse ir apmēram 400 rakstzīmēm--

Kad jūsu lapa ir gatava, izvelciet to dzīvu zaru. Pēc tam [Alchemy partneru portālā](https://alchemyportal.azurewebsites.net) un url laukā ievadiet faila nosaukumu. M