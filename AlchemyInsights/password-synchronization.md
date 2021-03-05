---
title: Synkronisering av passord
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482040"
---
# <a name="password-synchronization"></a><span data-ttu-id="c8cad-102">Synkronisering av passord</span><span class="sxs-lookup"><span data-stu-id="c8cad-102">Password synchronization</span></span>

<span data-ttu-id="c8cad-103">**Synkronisering av hash for passord fungerer ikke i det hele tatt**</span><span class="sxs-lookup"><span data-stu-id="c8cad-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="c8cad-104">Her er noen vanlige problemer kundene støter på når synkronisering av hash for passord ikke fungerer:</span><span class="sxs-lookup"><span data-stu-id="c8cad-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="c8cad-105">Active Directory-kontoen som brukes av Azure AD Connect til  å kommunisere med  lokal Active Directory, får ikke replikat katalogendringer og replikeringskatalogen endrer alle tillatelser, som er nødvendige for passordsynkronisering – du må løse dette ved å gi disse tillatelsene til Active Directory-kontoen.</span><span class="sxs-lookup"><span data-stu-id="c8cad-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="c8cad-106">Synkronisering av hash for passord deaktiveres når en  administrator har endret Bruker-Sign-In-metoden fra passordsynkronisering til et annet alternativ, for eksempel forbund med **AD FS** i veiviseren for Azure AD Connect . Du kan løse dette ved å aktivere funksjonen for synkronisering av **hash** for passord på nytt i veiviseren azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c8cad-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="c8cad-107">Tilkoblingsproblem med lokal Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c8cad-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="c8cad-108">Enkelte domenekontrollere er for eksempel ikke tilgjengelige med Azure AD Connect, eller portene som kreves, [blokkeres](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) av brannmuren . Du må løse dette ved å sikre at tilkoblingen mellom Azure AD Connect-serveren og den lokale Active Directory fungerer på riktig måte.</span><span class="sxs-lookup"><span data-stu-id="c8cad-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="c8cad-109">Azure AD Connect-serveren er for øyeblikket i feilsøkingsmodus, noe som fører til at serveren ikke får tilgang til hash-passordene . Hvis du vil feilsøke problemet, følger du fremgangsmåten i delen Feilsøke passordsynkronisering med Azure AD Connect-synkronisering – ingen passord [synkroniseres.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="c8cad-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="c8cad-110">**Synkronisering av hash for passord fungerer ikke for noen av brukerne mine**</span><span class="sxs-lookup"><span data-stu-id="c8cad-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="c8cad-111">Hvis du oppdaget at hash for passord ikke  synkroniseres for en bruker, kan du bruke feilsøkingsoppgaven i Azure AD Connect til å undersøke og løse problemet.</span><span class="sxs-lookup"><span data-stu-id="c8cad-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="c8cad-112">Utfør følgende oppgaver:</span><span class="sxs-lookup"><span data-stu-id="c8cad-112">Perform the following tasks:</span></span>

    <span data-ttu-id="c8cad-113">a.</span><span class="sxs-lookup"><span data-stu-id="c8cad-113">a.</span></span> [<span data-ttu-id="c8cad-114">Kjør feilsøkingsoppgaven i veiviseren</span><span class="sxs-lookup"><span data-stu-id="c8cad-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="c8cad-115">b.</span><span class="sxs-lookup"><span data-stu-id="c8cad-115">b.</span></span> [<span data-ttu-id="c8cad-116">Bruke cmdleten for feilsøking til å undersøke problemet med hashsynkronisering av passord for en bestemt bruk</span><span class="sxs-lookup"><span data-stu-id="c8cad-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="c8cad-117">Det lokale Active Directory User-objektet er aktivert for **brukeren, og brukeren må endre passord ved neste påloggingsalternativ.**</span><span class="sxs-lookup"><span data-stu-id="c8cad-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="c8cad-118">Når dette alternativet er aktivert, tilordnes brukeren et midlertidig passord, og brukeren blir bedt om å endre passordet ved neste pålogging.</span><span class="sxs-lookup"><span data-stu-id="c8cad-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="c8cad-119">Azure AD Connect synkroniserer ikke midlertidige passord til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c8cad-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="c8cad-120">Du kan løse problemet ovenfor ved å utføre en av følgende oppgaver:</span><span class="sxs-lookup"><span data-stu-id="c8cad-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="c8cad-121">Be brukeren om å logge på det lokale programmet (for eksempel Windows-skrivebord) og endre passordet.</span><span class="sxs-lookup"><span data-stu-id="c8cad-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="c8cad-122">Det nye passordet synkroniseres til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c8cad-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="c8cad-123">Be en administrator oppdatere brukerens passord uten å aktivere alternativet Brukeren må endre passordet ved neste pålogging **og** dele det nye passordet med brukeren.</span><span class="sxs-lookup"><span data-stu-id="c8cad-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="c8cad-124">Det lokale Active Directory User-objektet **er ikke riktig** konfigurert for objektsynkronisering eller passordsynkronisering.</span><span class="sxs-lookup"><span data-stu-id="c8cad-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="c8cad-125">Følg fremgangsmåten i feilsøking av hash-synkronisering av passord med [Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)for å feilsøke dette problemet.</span><span class="sxs-lookup"><span data-stu-id="c8cad-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







