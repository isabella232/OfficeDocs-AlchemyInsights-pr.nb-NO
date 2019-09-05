---
title: Feilsøking i forbindelse med nektet tilgang
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751285"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Feilsøking i forbindelse med tilgang nektet meldinger i administrasjonssenteret for SharePoint/OneDrive

Hvis du får meldingen ingen tilgang når du prøver å bla til et Administrasjonssenter for SharePoint/OneDrive, må du kontrollere at du [tilordner en lisens til brukeren](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Hvis brukeren har en lisens, bør du også kontrollere at de er [tilordnet en administratorrolle](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) som kan få tilgang til administrasjons sentrene.

Dette problemet kan også oppstå når en bruker er slettet og opprettet på nytt med samme hovednavn for bruker (UPN). Den nye kontoen opprettes ved hjelp av en annen verdi for PUID (Passport Unique ID). Når brukeren prøver å få tilgang til en områdesamling eller deres OneDrive, har brukeren en feil PUID. Et annet scenario omfatter katalogsynkronisering med en organisasjonsenhet for Active Directory (OU). Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen ORGANISASJONSENHET og resynced med SharePoint, kan de oppleve dette problemet.

Hvis du vil løse dette problemet, bør du gjenopprette den opprinnelige UPN med trinnene i artikkelen, [gjenopprette en bruker i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Merk: Hvis et OneDrive eller Administrasjonssenter for SharePoint ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig problem med tjenesten.  [Kontroller instrumentbordet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).


