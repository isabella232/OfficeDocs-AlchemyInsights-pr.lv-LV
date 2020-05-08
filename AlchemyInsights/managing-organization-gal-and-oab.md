---
title: Organizācijas globālā adrešu saraksta un bezsaistes adrešu grāmatas pārvaldība
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022524"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="45811-102">Organizācijas globālā adrešu saraksta (GAL) un bezsaistes adrešu grāmatas (OAB) pārvaldība</span><span class="sxs-lookup"><span data-stu-id="45811-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="45811-103">Globālais adrešu saraksts (GAL) ir pasta iespējotu objektu saraksts (jebkāda tipa abonements, kas svar saņemt e-pasta ziņojumus) organizācijā.</span><span class="sxs-lookup"><span data-stu-id="45811-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="45811-104">Viens GAL saraksts tiek automātiski izveidots katrā organizācijā.</span><span class="sxs-lookup"><span data-stu-id="45811-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="45811-105">Jūs varat veidot papildu GAL sarakstus, lai grupētu lietotājus pēc organizācijas vai atrašanās vietas, bet viens lietotājs vienlaicīgi var apskatīt un izmantot tikai vienu GAL sarakstu.</span><span class="sxs-lookup"><span data-stu-id="45811-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="45811-106">Atsevišķi e-pasta klienti, piemēram, Outlook darbam ar Windows, lejupielādē GAL izmantošanai bezsaistē.</span><span class="sxs-lookup"><span data-stu-id="45811-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="45811-107">Lejupielādētos sarakstus sauc par bezsaistes adrešu grāmatām (OAB).</span><span class="sxs-lookup"><span data-stu-id="45811-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="45811-108">Pakalpojumā Exchange Online OAB atjaunināšana notiek reizi 8 stundās un klientiem ir jālejupielādē un jāatjaunina OAB lokālā kopija.</span><span class="sxs-lookup"><span data-stu-id="45811-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="45811-109">Jebkurām adresātu izmaiņām ir vispirms jābūt redzamām GAL sarakstā, lai vēlāk tās būtu redzamas OAB.</span><span class="sxs-lookup"><span data-stu-id="45811-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="45811-110">Tālāk ir aprakstītas biežāk izmantotās GAL un OAB procedūras:</span><span class="sxs-lookup"><span data-stu-id="45811-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="45811-111">Iespējams, ka vēlēsities, lai atsevišķi objekti būtu slēpti GAL sarakstā.</span><span class="sxs-lookup"><span data-stu-id="45811-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="45811-112">Lasiet rakstu [Adresātu slēpšana adrešu sarakstos](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="45811-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="45811-113">Ja vēlaties piešķirt konkrētai lietotāju grupai pielāgotus organizācijas GAL sarakstu skatus, lasiet rakstu [Exchange Online adrešu grāmatu politikas](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="45811-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="45811-114">[Izveidojiet Exchange Online globālo adrešu sarakstu](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) un lasiet [Exchange Online adrešu saraksti](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists), lai uzzinātu vairāk par darbu ar GAL atļaujām.</span><span class="sxs-lookup"><span data-stu-id="45811-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="45811-115">Ņemiet vērā, ka, ja veidojat jaunus GAL sarakstus, tad jums var noderēt arī jauns OAB.</span><span class="sxs-lookup"><span data-stu-id="45811-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="45811-116">Lasiet [Bezsaistes adrešu grāmatas procedūras](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="45811-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
