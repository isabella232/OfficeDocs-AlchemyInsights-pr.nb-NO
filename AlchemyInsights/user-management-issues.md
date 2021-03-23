---
title: Problemer med brukeradministrasjon
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036287"
---
# <a name="user-management-issues"></a><span data-ttu-id="ea1ec-102">Problemer med brukeradministrasjon</span><span class="sxs-lookup"><span data-stu-id="ea1ec-102">User management issues</span></span>

<span data-ttu-id="ea1ec-103">**Hva skjer med gjeldende tilordnede brukere til programmet hvis jeg deaktiverer egenskapen Brukertilordning kreves (angi denne egenskapen til Nei)?**</span><span class="sxs-lookup"><span data-stu-id="ea1ec-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="ea1ec-104">Deaktivering av **brukertilordning kreves** påvirker IKKE de tilordnede brukerne.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="ea1ec-105">Hvis du deaktiverer denne egenskapen, får bare alle brukere tilgang til programmet.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="ea1ec-106">Alle de oppførte brukerne og de brukerne som er tilordnet til grupper i programmet, vil fortsatt være gyldige.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="ea1ec-107">Hvis du vil begrense appen til et bestemt sett med brukere, kan du se – Begrense Azure AD-appen til et sett med brukere [– Microsofts identitetsplattform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span><span class="sxs-lookup"><span data-stu-id="ea1ec-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="ea1ec-108">Hvis du vil tilordne brukere og grupper, til bedriftsprogrammer i Azure Active Directory (Azure AD), enten fra Azure-portalen eller ved hjelp av PowerShell, kan du se Administrere brukertilordning for en app i [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span><span class="sxs-lookup"><span data-stu-id="ea1ec-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="ea1ec-109">Hvis du vil delegere tillatelser for oppretting og administrasjon av programmer, kan du se Delegere administratortillatelser for programadministrasjon [– Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span><span class="sxs-lookup"><span data-stu-id="ea1ec-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="ea1ec-110">**Skjul bestemte bedriftsapper for brukere** – Bruk fremgangsmåten nedenfor til å skjule alle Microsoft 365-apper fra **MyApps-panelet.**</span><span class="sxs-lookup"><span data-stu-id="ea1ec-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="ea1ec-111">Appene vil fortsatt være synlige i Office 365-portalen.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="ea1ec-112">Logg på Azure-portalen som global administrator for katalogen.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="ea1ec-113">Velg **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="ea1ec-114">Velg **Brukere**.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="ea1ec-115">Velg **Brukerinnstillinger**.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="ea1ec-116">Klikk **Administrer hvordan** sluttbrukere starter og viser programmene under **Virksomhetsprogrammer**.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="ea1ec-117">For **Brukere kan bare se Office 365-apper i Office 365-portalen,** klikker du **Ja**.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="ea1ec-118">Klikk på **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="ea1ec-119">Hvis du vil ha mer informasjon, kan du se Skjule et [Enterprise-program fra brukeropplevelsen i Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span><span class="sxs-lookup"><span data-stu-id="ea1ec-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="ea1ec-120">Hvis du tilbyr en Programvare som tjenesteapp (SaaS) til mange organisasjoner, kan du konfigurere appen til å godta pålogginger fra en hvilken som helst Azure Active Directory-leier (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ea1ec-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="ea1ec-121">Denne konfigurasjonen kalles «å gjøre programmet ditt til flere leiere».</span><span class="sxs-lookup"><span data-stu-id="ea1ec-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="ea1ec-122">Brukere i enhver Azure AD-leier kan logge på appen etter at de har samtykket til å bruke kontoen sin med appen.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="ea1ec-123">Hvis du vil ha mer informasjon, kan du se Bygge [apper som logger på Azure AD-brukere – Microsofts identitetsplattform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span><span class="sxs-lookup"><span data-stu-id="ea1ec-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="ea1ec-124">**Hvordan får en sluttbruker tilgang til programmet når han/hun er tilordnet til programmet?**</span><span class="sxs-lookup"><span data-stu-id="ea1ec-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="ea1ec-125">Hver app i Enterprise-programbladet har en kobling som sluttbrukerne kan få tilgang til.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="ea1ec-126">Brukere kan også få tilgang til appen via **Myapps-portalen** på en enkel måte.</span><span class="sxs-lookup"><span data-stu-id="ea1ec-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="ea1ec-127">**Vil du vite hvilke programmer og hvilken type programmer som brukes av brukere?**</span><span class="sxs-lookup"><span data-stu-id="ea1ec-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="ea1ec-128">Du kan laste ned påloggingsrapporter for de siste 30 dagene fra portal.azure.com > Azure Active Directory> **Signins> laste ned rapporter.**</span><span class="sxs-lookup"><span data-stu-id="ea1ec-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="ea1ec-129">Finn ut hvordan [du gir hele leieren tillatelse til](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) et program og Konfigurerer hvordan [sluttbrukere samtykker i programmer.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)</span><span class="sxs-lookup"><span data-stu-id="ea1ec-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="ea1ec-130">Forstå [hvordan samtykke fungerer og](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) Administrere samtykke til [programmer.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)</span><span class="sxs-lookup"><span data-stu-id="ea1ec-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>


