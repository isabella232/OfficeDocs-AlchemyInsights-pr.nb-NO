---
title: Avanserte godkjenningskonsepter som gjelder for Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398594"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="a0c5f-102">Avanserte godkjenningskonsepter som gjelder for Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a0c5f-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="a0c5f-103">Nedenfor finner du de avanserte godkjenningskonseptene som gjelder for Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="a0c5f-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="a0c5f-104">**Proaktiv godkjenning**</span><span class="sxs-lookup"><span data-stu-id="a0c5f-104">**Proactive Authentication**</span></span>

<span data-ttu-id="a0c5f-105">Når du aktiverer [ProactiveAuthEnabled-policyen,](https://go.microsoft.com/fwlink/?linkid=2134621) prøver Microsoft Edge å proaktivt godkjenne påloggede brukere via Microsoft-tjenester.</span><span class="sxs-lookup"><span data-stu-id="a0c5f-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="a0c5f-106">Med jevne mellomrom bruker den en nettbasert tjeneste til å se etter et oppdatert manifest som inneholder konfigurasjonen som styrer Proaktiv godkjenning.</span><span class="sxs-lookup"><span data-stu-id="a0c5f-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="a0c5f-107">Fordeler: Proaktiv godkjenning gjør det mulig å godkjenning til viktige tjenester, for eksempel Office Ny fane-siden.</span><span class="sxs-lookup"><span data-stu-id="a0c5f-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="a0c5f-108">Hvis Bing brukes som søkemotor, forbedrer proaktiv godkjenning også ytelsen til adresselinjen og bidrar til å generere søkeresultater tilpasset behovene til bedriften.</span><span class="sxs-lookup"><span data-stu-id="a0c5f-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="a0c5f-109">**Windows Hello CredUI for NTLM-godkjenning**</span><span class="sxs-lookup"><span data-stu-id="a0c5f-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="a0c5f-110">Hvis enkel pålogging (SSO) ikke er tilgjengelig når et nettsted prøver å logge på brukeren via NTLM- eller Negotiate-mekanismen, lar denne funksjonen brukeren dele OS-legitimasjonen med nettstedet og oppfylle godkjenningsutfordringen ved hjelp av Windows Hello Cred-brukergrensesnittet.</span><span class="sxs-lookup"><span data-stu-id="a0c5f-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="a0c5f-111">Denne påloggingsflyten vises bare i Windows 10 og bare for brukere som ikke får SSO under en NTLM- eller Forhandlingsutfordring.</span><span class="sxs-lookup"><span data-stu-id="a0c5f-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="a0c5f-112">**Bruke lagrede passord til å logge på automatisk**</span><span class="sxs-lookup"><span data-stu-id="a0c5f-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="a0c5f-113">Brukere som lagrer passord i Microsoft Edge, kan aktivere automatisk pålogging på nettsteder der de har lagret legitimasjon.</span><span class="sxs-lookup"><span data-stu-id="a0c5f-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="a0c5f-114">Brukere kan aktivere eller deaktivere denne funksjonen i edge://settings/passwords, og du kan konfigurere den i [policyene for passordbehandling.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="a0c5f-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
