---
title: Konfigurere tjenestetilkoblingspunkt (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036147"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="9937c-102">Konfigurere tjenestetilkoblingspunkt (SCP)</span><span class="sxs-lookup"><span data-stu-id="9937c-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="9937c-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="9937c-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="9937c-104">**Årsak:** Kan ikke lese SCP-objektet og få informasjon om Azure AD-leieren</span><span class="sxs-lookup"><span data-stu-id="9937c-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="9937c-105">**Løsning:** Se delen Konfigurere [et tjenestetilkoblingspunkt](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="9937c-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="9937c-106">**Handlingsplan**</span><span class="sxs-lookup"><span data-stu-id="9937c-106">**Action plan**</span></span>

- <span data-ttu-id="9937c-107">Kontroller om enheten har mottatt gruppepolicyobjektet for den kontrollerte valideringen.</span><span class="sxs-lookup"><span data-stu-id="9937c-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="9937c-108">Kontroller at gruppepolicyobjektet har opprettet registernøklene.</span><span class="sxs-lookup"><span data-stu-id="9937c-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="9937c-109">Kontroller at du har to nøkler opprettet med katalog-ID-en og onmicrosoft-domenet.</span><span class="sxs-lookup"><span data-stu-id="9937c-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="9937c-110">**Konfigurere registerinnstilling for klientsiden for SCP**</span><span class="sxs-lookup"><span data-stu-id="9937c-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="9937c-111">Bruk følgende eksempel til å opprette et gruppepolicyobjekt (GPO) til å distribuere en registerinnstilling som konfigurerer en SCP-oppføring i registeret på enhetene.</span><span class="sxs-lookup"><span data-stu-id="9937c-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="9937c-112">Åpne en konsoll for gruppepolicybehandling, og opprett et nytt gruppepolicyobjekt i domenet.</span><span class="sxs-lookup"><span data-stu-id="9937c-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="9937c-113">Gi det nyopprettede gruppepolicyobjektet et navn (for eksempel ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="9937c-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="9937c-114">Rediger gruppepolicyobjektet, og finn følgende bane: Datamaskinkonfigurasjon > **Innstillinger > Windows-innstillinger > registeret**.</span><span class="sxs-lookup"><span data-stu-id="9937c-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="9937c-115">Høyreklikk **registeret, og** velg **Nytt > registerelement**.</span><span class="sxs-lookup"><span data-stu-id="9937c-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="9937c-116">Konfigurer følgende **på** Generelt-fanen:</span><span class="sxs-lookup"><span data-stu-id="9937c-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="9937c-117">**Handling:** Oppdater</span><span class="sxs-lookup"><span data-stu-id="9937c-117">**Action**: Update</span></span>
    
- <span data-ttu-id="9937c-118">**Struktur:** HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="9937c-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="9937c-119">**Nøkkelbane:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="9937c-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="9937c-120">**Verdinavn:** TenantId</span><span class="sxs-lookup"><span data-stu-id="9937c-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="9937c-121">**Verditype**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="9937c-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="9937c-122">**Verdidata:** GUID- eller katalog-ID-en for Azure AD-forekomsten (Denne verdien finnes i **Azure Portal > Azure Active Directory > Egenskaper > Katalog-ID**)</span><span class="sxs-lookup"><span data-stu-id="9937c-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="9937c-123">Klikk **OK**.</span><span class="sxs-lookup"><span data-stu-id="9937c-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="9937c-124">Høyreklikk **registeret, og** velg **Nytt > registerelement**.</span><span class="sxs-lookup"><span data-stu-id="9937c-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="9937c-125">Konfigurer følgende **på** Generelt-fanen:</span><span class="sxs-lookup"><span data-stu-id="9937c-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="9937c-126">**Handling:** Oppdater</span><span class="sxs-lookup"><span data-stu-id="9937c-126">**Action**: Update</span></span>
    
- <span data-ttu-id="9937c-127">**Struktur:** HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="9937c-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="9937c-128">**Nøkkelbane:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="9937c-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="9937c-129">**Verdinavn:** TenantName</span><span class="sxs-lookup"><span data-stu-id="9937c-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="9937c-130">**Verditype**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="9937c-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="9937c-131">**Verdidata:** Det bekreftede domenenavnet hvis du bruker et forbundsmiljø, for eksempel AD FS.</span><span class="sxs-lookup"><span data-stu-id="9937c-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="9937c-132">Det bekreftede domenenavnet eller onmicrosoft.com domenenavnet (for eksempel contoso.onmicrosoft).com hvis du bruker administrert miljø</span><span class="sxs-lookup"><span data-stu-id="9937c-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="9937c-133">Klikk **OK**.</span><span class="sxs-lookup"><span data-stu-id="9937c-133">Click **OK**.</span></span>

7. <span data-ttu-id="9937c-134">Lukk redigeringsprogrammet for det nylig opprettede gruppepolicyobjektet.</span><span class="sxs-lookup"><span data-stu-id="9937c-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="9937c-135">Koble det nylig opprettede gruppepolicyobjektet til den ønskede organisasjonsenheten som inneholder domenekretserte datamaskiner som tilhører den kontrollerte utrullingspopulasjonen.</span><span class="sxs-lookup"><span data-stu-id="9937c-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="9937c-136">Hvis du vil ha mer informasjon, kan du se [Kontrollert validering av hybrid Azure AD-sammenføyning – Azure AD | Microsoft Docs og](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)  [Feilsøking av hybrid Azure Active Directory-sammenføyde enheter | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="9937c-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









