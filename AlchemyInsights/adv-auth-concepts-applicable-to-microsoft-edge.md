---
title: Avanserte godkjennings begreper som gjelder for Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573525"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="c52b2-102">Avanserte godkjennings begreper som gjelder for Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="c52b2-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="c52b2-103">Følgende er de avanserte godkjennings konseptene som gjelder for Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="c52b2-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="c52b2-104">**Proaktiv godkjenning**</span><span class="sxs-lookup"><span data-stu-id="c52b2-104">**Proactive Authentication**</span></span>

<span data-ttu-id="c52b2-105">Når du aktiverer [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -policyen, vil Microsoft Edge prøve å godkjenne påloggede brukere via Microsoft-tjenester.</span><span class="sxs-lookup"><span data-stu-id="c52b2-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="c52b2-106">Med regelmessige intervaller vil det bruke en nett BAS ert tjeneste til å se etter et oppdatert manifest som inneholder konfigurasjonen som styrer proaktiv godkjenning.</span><span class="sxs-lookup"><span data-stu-id="c52b2-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="c52b2-107">Fordeler: proaktiv godkjenning muliggjør godkjenning for viktige tjenester, for eksempel siden for ny fane i Office.</span><span class="sxs-lookup"><span data-stu-id="c52b2-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="c52b2-108">Hvis Bing brukes som søke motor, forbedrer proaktivt godkjenning ytelsen på adresse linjen og bidrar til å generere søke resultater tilpasset behovene til bedriften.</span><span class="sxs-lookup"><span data-stu-id="c52b2-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="c52b2-109">**Windows Hello-CredUI for NTLM-godkjenning**</span><span class="sxs-lookup"><span data-stu-id="c52b2-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="c52b2-110">Hvis Single Sign-on (SSO) ikke er tilgjengelig når et nettsted prøver å logge på brukeren gjennom NTLM-eller Negotiate-mekanismen, kan denne funksjonen dele OS-legitimasjonen med nettstedet og oppfylle godkjennings utfordringen ved hjelp av Windows Hello-legitimasjons bruker grensesnittet.</span><span class="sxs-lookup"><span data-stu-id="c52b2-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="c52b2-111">Denne flyten vises bare i Windows 10, og bare for brukere som ikke får SSO under en NTLM eller en Negotiate-utfordring.</span><span class="sxs-lookup"><span data-stu-id="c52b2-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="c52b2-112">**Bruke lagrede passord til å logge på automatisk**</span><span class="sxs-lookup"><span data-stu-id="c52b2-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="c52b2-113">Brukere som lagrer passord i Microsoft Edge, kan aktivere automatisk pålogging til nett steder der de har lagret legitimasjon.</span><span class="sxs-lookup"><span data-stu-id="c52b2-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="c52b2-114">Brukere kan aktivere eller deaktivere denne funksjonen i edge://settings/passwords, og du kan konfigurere den i policyer for [passord behandling](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="c52b2-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
