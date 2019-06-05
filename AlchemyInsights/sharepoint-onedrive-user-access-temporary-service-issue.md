---
title: Ytelse problemer-SharePoint eller OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719525"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive langsom, utilgjengelig eller ikke tilgjengelig for flere brukere

Hvis et OneDrive eller SharePoint-område ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et problem med tjenesten midlertidig. [Kontroller service helse instrumentbordet](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>Legg til og lisensier brukeren

Forsikre deg om at du [tilordne lisenser til brukere i Office 365 for bedrifter](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>Tilordne tillatelser

Hvis brukeren har blitt tilordnet en lisens for Sharepoint og fortsatt mottar meldingen Ingen tilgang, pass på at de har [riktig tillatelsesnivå](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) som er tilordnet.

## <a name="consider-using-the-access-request-feature"></a>Vurder å bruke funksjonen for forespørsel

[Forespørsel om funksjonen](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) kan personer til å be om tilgang til innhold som de ikke har tillatelse til å se.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>Tillat egendefinert skript kan føre til problemer med tilgang

Det finnes visse scenarier der funksjonen *Tillat egendefinert skript* kan presentere en tilgang. For en liste over funksjoner som påvirkes, Sikkerhetsvurderinger og muligheten til å deaktivere funksjonen. Besøk [Tillat eller forby egendefinert skript](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

