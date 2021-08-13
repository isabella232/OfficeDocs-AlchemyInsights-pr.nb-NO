---
title: Feilsøking Avslått meldinger til OneDrive for Business nettsteder
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957802"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Feilsøking Avslått meldinger til OneDrive for Business nettsteder

Dette problemet oppstår oftest når en bruker slettes og opprettes på nytt med samme brukerprinsippnavn (UPN). Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (Passport Unique ID). Når brukeren prøver å få tilgang til en nettstedssamling eller OneDrive, har brukeren feil PUID. Et annet scenario innebærer katalogsynkronisering med en Active Directory-organisasjonsenhet (OU). Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen organisasjonsenheten og synkroniseres på nytt med SharePoint, kan de oppleve dette problemet.

1. Du kan løse dette problemet ved å gjenopprette det opprinnelige UPN-nummeret med fremgangsmåten i artikkelen Gjenopprette [en bruker i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Hvis du ikke kan gjenopprette den opprinnelige brukeren, bør du fjerne den gamle brukeren fra OneDrive nettstedet ved hjelp av disse trinnene, Fjerne en bruker fra [brukerinformasjonslisten](). 
3. Når dette er gjort, kan du bekrefte at brukeren har administratorrettigheter til OneDrive-nettstedet ved å følge fremgangsmåten for å legge til administratorer for en [brukers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Hvis du vil ha mer informasjon om tilgangsnivåer, kan du se artikkelen Forstå [tilgangsnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
