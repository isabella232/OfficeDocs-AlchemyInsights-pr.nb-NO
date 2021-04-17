---
title: Administrasjonssenter for Teams
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
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826388"
---
# <a name="teams-admin-center"></a><span data-ttu-id="75f30-102">Administrasjonssenter for Teams</span><span class="sxs-lookup"><span data-stu-id="75f30-102">Teams Admin Center</span></span>

<span data-ttu-id="75f30-103">Finn ut om administrasjon av Teams med [administrasjonssenteret for Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="75f30-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="75f30-104">Hvis du ikke får tilgang til administrasjonssenteret for Teams, må du kontrollere følgende elementer:</span><span class="sxs-lookup"><span data-stu-id="75f30-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="75f30-105">Kontroller at du har tillatt de riktige [Office 365-IP-adressene og nettadressene](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på eventuelle perimeterenheter (brannmurer osv.) eller i brannmurreglene på den lokale datamaskinen.</span><span class="sxs-lookup"><span data-stu-id="75f30-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="75f30-106">Kontroller at påloggingen du bruker for å få tilgang til administrasjonsportalen for Teams, samsvarer med brukernavnet som er oppført i [administrasjonsportalen for Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="75f30-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="75f30-107">Hvis brukerne ikke vises i administrasjonssenteret for Teams, må du kontrollere følgende:</span><span class="sxs-lookup"><span data-stu-id="75f30-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="75f30-108">Har du opprettet brukere eller tilordnet lisenser de siste 24 timene?</span><span class="sxs-lookup"><span data-stu-id="75f30-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="75f30-109">Kontroller at du venter minst 24 timer før du åpner en støtteforespørsel.</span><span class="sxs-lookup"><span data-stu-id="75f30-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="75f30-110">Kontroller at du har tildelt riktige lisenser?</span><span class="sxs-lookup"><span data-stu-id="75f30-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="75f30-111">Hvis du har en lokal Active Directory, må du kontrollere at verdien av [msRTCSIP-PrimaryUserAddress eller SIP-adressen i ProxyAddresses-feltet](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) i den lokale Active Directory er unik, og at formatet samsvarer med sip:**Brukernavnet** til brukeren fra administrasjonssenteret [for Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="75f30-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="75f30-112">Hvis du har tenkt å beholde en Skype for Business Server-distribusjon og få brukerne til å være hjemmebruk lokalt og på Nettet: følg «Konfigurer hybrid med Teams og **Skype for Business Online»** i kontrollpanelet for Skype for Business Server og flytt brukere på Nettet.</span><span class="sxs-lookup"><span data-stu-id="75f30-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
