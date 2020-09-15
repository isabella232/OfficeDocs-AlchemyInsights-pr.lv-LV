---
title: tas pats, kas faila nosaukums ir vispiemērotākais
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664141"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Required Alchemy header H1, H2's nedarbojas".
Paraugprakse un norādījumi par alķīmijas autorēšanu:

1. **Neligzdojiet alķīmijas ieskatus mapēs**— tas pārtrauks vietrāža URL struktūru. Mēs meklējam šo problēmu.
1. Failiem mapē **AlchemyInsights** ir jābūt ar mazajiem burtiem ar defisēm, kas paredzētas atstarpēm. ***padomi par to, kā to iespējot***.
    1. Iekļaujiet kārtulas ID vai kopas ID no [alķīmijas partnera portāla](https://alchemyportal.azurewebsites.net) MS. Custom laukā. //templates.Office.com/. ***MS. Custom: 100021***
1. Izmantojiet pārējos šī faila augšdaļā esošo metadatu veidnes.
1. [Alķīmijas partnera portālā](https://alchemyportal.azurewebsites.net)pārejiet uz leju līdz sadaļas **klientu izpratnes virsrakstam:** un izmantojiet to kā sākumpunktu, lai iegūtu ieskatu. 
    > [!NOTE]
    > Alķīmijas ieskatiem augšdaļā ir jābūt tikai vienam H1, vai tie salūsts ražošanā. H2s neatveido, tāpēc izmantojiet **treknraksta** vai citas konvencijas, lai norādītu atsevišķas sadaļas.
1. Pēc tam aizpildiet pamattekstu, izmantojot melnraksta materiālu, kas atrodas alķīmijas kārtulas lapas sadaļā klientu ieskati
    1. Saraksti ar aizzīmēm ir precīzi
    1. Arī numurētie saraksti
    1. **Treknraksts** un *Slīpraksts* ir a-OK
    1. Saitēm vienmēr jābūt vai nu **"saitēm uz tīmekli"/External** vai **dziļām saitēm uz UI elementiem**, nevis iekšējām saitēm.
    1. Pašlaik attēli nav oficiāli atbalstīti, taču tie ir iekļauti ceļvedī.

Un tas jau ir pārāk garš. Paraugprakse ir par 400 rakstzīmēm---------------------------------

Kad saturs ir gatavs, velciet to uz tiešo zaru. Pēc tam dodieties uz [alķīmijas partnera portālu](https://alchemyportal.azurewebsites.net) un ievadiet faila nosaukumu laukā URL. 