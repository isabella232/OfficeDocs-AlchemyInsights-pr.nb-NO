---
title: Feilsøke ingen meldinger om tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758483"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Feilsøke ingen tilgang i administrasjonssenteret for Sharepoint/OneDrive

Hvis du mottar en melding om ingen tilgang når du prøver å bla til et administrasjonssenter for Sharepoint/OneDrive, må du kontrollere at du [tilordner en lisens til brukeren](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Hvis brukeren har en lisens, bør du også kontrollere at de er [tilordnet en administratorrolle](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) som har tilgang til administrasjonssentrene.

Dette problemet kan også oppstå når en bruker slettes og opprettes på nytt med samme brukerhovednavn (UPN). Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (Passport Unique ID). Når brukeren prøver å få tilgang til en områdesamling eller OneDrive, har brukeren en feil PUID. Et annet scenario innebærer katalogsynkronisering med en Active Directory-organisasjonsenhet (OU). Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen ORGANISASJON og synkroniseres på nytt med SharePoint, kan de oppleve dette problemet.

Hvis du vil løse dette problemet, bør du gjenopprette den opprinnelige UPN med trinnene i artikkelen, [Gjenopprette en bruker i Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Merk: Hvis et administrasjonssenter for OneDrive eller SharePoint ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig tjenesteproblem.  [Kontroller instrumentbordet for servicetilstand](https://portal.office.com/adminportal/home#/servicehealth).


