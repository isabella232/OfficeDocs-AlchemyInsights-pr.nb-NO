---
title: Feilsøke problemer med Azure AD-sammenføyning
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405131"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Feilsøke problemer med Azure AD-sammenføyning

1. Hvis du konfigurerer enhetsregistreringer for første gang, må du kontrollere at du har gjennomgått Innføring i enhetsbehandling i [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) som veileder deg om hvordan du får enheter under kontrollen til Azure AD. 
1. Hvis du registrerer enheter i Azure AD direkte og registrerer dem i Intune, må du kontrollere at [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) du har konfigurert [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) og ha lisensiering på plass først.
1. Kontroller at du er autorisert til å utføre operasjoner i Azure AD. Bare en global administrator i Azure AD kan administrere innstillinger for enhetsregistreringer.
1. Hvis du vil gjøre implementering av Azure AD-sammenføyning, kan [du se Planlegge Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Hvis du vil ha mer informasjon om hvordan du løser vanlige problemer med Azure AD-sammenføyning, kan du se Vanlige spørsmål om Azure [Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) og for Windows 10 pro-enheter i Kan ikke bli med i [Windows 10 Pro-maskinen](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) til Azure AD – Må oppgradere til – Microsoft Community
