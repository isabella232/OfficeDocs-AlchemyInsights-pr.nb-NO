---
title: Får ikke tilgang SharePoint eller OneDrive administrasjonssenteret
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: afb28ccae2c9f087f1e1417cb6594cedc908e1cf759a5d1e6d92c4ee9a75527d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020453"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Får ikke tilgang SharePoint eller OneDrive administrasjonssenteret

- Hvis SharePoint- eller OneDrive-administrasjonssenteret er utilgjengelig eller utilgjengelig, kan det være et midlertidig tjenesteproblem der brukere opplever uregelmessig forsinkelser eller navigasjonsfeil når de får tilgang til SharePoint nettsteder eller OneDrive innhold. Kontroller [instrumentbordet for tjenestetilstand](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) for å se om organisasjonen påvirkes.

- Globale og SharePoint må tilordnes en SharePoint lisens. Nylig opprettede kontoer som nettopp er tilordnet med en SharePoint-lisens eller administratorrolle, kan oppleve problemer med å få tilgang til SharePoint, for eksempel «ingen tilgang» eller «brukeren ble ikke funnet». Gi minst 24 timer for synkronisering for å fullføre på tvers av systemene våre. Vi forstår at 24 timer kan virke som en lang tid. I mange tilfeller arbeider vi allerede med en løsning.

- Privileged Identity Management[(PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)brukere kan få tilgang nektet hvis tidsvinduet for tillatt tilgang er svært lite, kan du se Ingen tilgang [til PIM-kontoer](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).