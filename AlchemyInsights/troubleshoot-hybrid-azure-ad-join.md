---
title: Feilsøk Hybrid Azure AD-sammenføyning
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401916"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Feilsøk Hybrid Azure AD-sammenføyning

Sterkt anbefalt: kontroller at en enhet får tilgang til endepunkter for enhetsregistrering under systemkontoen ved å bruke skriptet [Test tilkobling for enhetsregistrering](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Dersom det er første gang du konfigurerer enhetsregistreringer, husk å se gjennom [Introduksjon til enhetsbehandling i Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) for å lære hvordan du får enheter under kontroll av Azure Active Directory.
1. Dersom du registrerer enheter i Azure Active Directory direkte og melder dem inn i Intune, påse at du har [konfigurert Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) og har [lisensieringen](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) på plass først.
1. Påse at du er autorisert til å utføre operasjoner i Azure Active Directory og lokalt Active Directory. Bare en global administrator i Azure Active Directory kan behandle innstillinger for enhetsregistreringer. I tillegg, dersom du konfigurerer automatiske registreringer in det lokale Active Directory, må du være administrator for Active Directory og AD FS (hvis gjeldende).

Hvis du vil ha flere detaljer om hvordan du løser potensielle problemer med hybrid-sammenføyning, kan du se [Feilsøk hybrid-sammenføyning](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for konfigurering av hybrid Azure AD-sammenføyde og behandle enheter med Azure Active Directory-portal, se [Konfigurere hybrid Azure AD-sammenføyde (lokalt domene-sammenføyde) enheter](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) og [Behandle enheter med Azure-portalen](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

For å løse vanlige problemer med Hybrid Azure Active Directory (AD), se [Hybrid Azure AD-sammenføyning - vanlige spørsmål](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
