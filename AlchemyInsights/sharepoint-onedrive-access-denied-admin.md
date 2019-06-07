---
title: Feilsøking i forbindelse med tilgang til meldinger
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760349"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Feilsøking i forbindelse med tilgang meldinger i administrasjonssenteret for Sharepoint/OneDrive

Hvis du mottar meldingen Ingen tilgang når du forsøker å gå til administrasjonssenteret en Sharepoint/OneDrive, må du kontrollere at du [tilordner en lisens for brukeren](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Hvis brukeren har en lisens, bør du også kontrollere at de er [tilordnet en administrator-rolle](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) som har tilgang til admin-sentre.

Dette problemet kan også oppstå når en bruker slettes og opprettes på nytt med samme brukerhovednavnet (UPN). Den nye kontoen er opprettet ved hjelp av en annen verdi for PUID (unik ID for Passport). Når brukeren prøver å få tilgang til en områdesamling eller sin OneDrive, har brukeren en feil PUID. Andre scenariet omfatter directory-synkronisering med en Active Directory-organisasjonsenhet (OU). Hvis brukere har allerede logget på SharePoint, er flyttet til en annen Organisasjonsenhet og resynced med SharePoint, kan de oppleve dette problemet.

Hvis du vil løse dette problemet, bør du gjenopprette den opprinnelige UPN med trinnene i artikkelen, [gjenopprette en brukers i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Merk: Hvis en OneDrive eller en SharePoint-administrator center ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være en midlertidig tjeneste problem.  [Kontroller service helse instrumentbordet](https://portal.office.com/adminportal/home#/servicehealth).


