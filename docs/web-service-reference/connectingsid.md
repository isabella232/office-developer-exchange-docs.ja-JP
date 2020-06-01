---
title: ConnectingSID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectingSID
api_type:
- schema
ms.assetid: 56d6aa52-8fa6-4773-9046-44a6f4f5d97c
description: ConnectingSID 要素は、ExchangeImpersonation SOAP ヘッダーを使用しているときに偽装するアカウントを表します。
ms.openlocfilehash: f4edf63f129fc769f4a2d710a505b40da4057fab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459280"
---
# <a name="connectingsid"></a><span data-ttu-id="041fd-103">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="041fd-103">ConnectingSID</span></span>

<span data-ttu-id="041fd-104">**ConnectingSID**要素は、EXCHANGEIMPERSONATION SOAP ヘッダーを使用しているときに偽装するアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="041fd-104">The **ConnectingSID** element represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span> 
  
- [<span data-ttu-id="041fd-105">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="041fd-105">ExchangeImpersonation</span></span>](exchangeimpersonation.md) 
- [<span data-ttu-id="041fd-106">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="041fd-106">ConnectingSID</span></span>](connectingsid.md)
  
```xml
<ConnectingSID>
   <PrincipalName/>
</ConnectingSID>
```

```xml
<ConnectingSID>
   <SmtpAddress/>
</ConnectingSID>
```

```xml
<ConnectingSID>
    <SID/> 
</ConnectingSID>
```

```xml
<ConnectingSID>
   <PrimarySmtpAddress/>
</ConnectingSID>
```

<span data-ttu-id="041fd-107">**ConnectingSIDType**</span><span class="sxs-lookup"><span data-stu-id="041fd-107">**ConnectingSIDType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="041fd-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="041fd-108">Attributes and elements</span></span>

<span data-ttu-id="041fd-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="041fd-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="041fd-110">属性</span><span class="sxs-lookup"><span data-stu-id="041fd-110">Attributes</span></span>

<span data-ttu-id="041fd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="041fd-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="041fd-112">子要素</span><span class="sxs-lookup"><span data-stu-id="041fd-112">Child elements</span></span>

|<span data-ttu-id="041fd-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="041fd-113">**Element**</span></span>|<span data-ttu-id="041fd-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="041fd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="041fd-115">PrincipalName</span><span class="sxs-lookup"><span data-stu-id="041fd-115">PrincipalName</span></span>](principalname.md) <br/> |<span data-ttu-id="041fd-116">偽装に使用するアカウントのユーザープリンシパル名 (UPN) を表します。</span><span class="sxs-lookup"><span data-stu-id="041fd-116">Represents the user principal name (UPN) of the account to use for impersonation.</span></span> <span data-ttu-id="041fd-117">これは、ユーザーアカウントが存在するドメインの UPN である必要があります。</span><span class="sxs-lookup"><span data-stu-id="041fd-117">This should be the UPN for the domain where the user account exists.</span></span>  <br/> |
|[<span data-ttu-id="041fd-118">SID</span><span class="sxs-lookup"><span data-stu-id="041fd-118">SID</span></span>](sid.md) <br/> |<span data-ttu-id="041fd-119">偽装に使用するアカウントのセキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="041fd-119">Represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation.</span></span>  <br/> |
|[<span data-ttu-id="041fd-120">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="041fd-120">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="041fd-121">Exchange の偽装に使用するアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="041fd-121">Represents the primary Simple Mail Transfer Protocol (SMTP) address of the account to use for Exchange impersonation.</span></span> <span data-ttu-id="041fd-122">プライマリ SMTP アドレスが指定されている場合は、ユーザーの SID を取得するために、さらに Active Directory ディレクトリサービス参照にコストがかかります。</span><span class="sxs-lookup"><span data-stu-id="041fd-122">If the primary SMTP address is supplied, it will cost an extra Active Directory directory service lookup in order to obtain the SID of the user.</span></span> <span data-ttu-id="041fd-123">使用可能な場合は、SID または UPN を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="041fd-123">We recommend that you use the SID or UPN if they are available.</span></span>  <br/> |
|[<span data-ttu-id="041fd-124">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="041fd-124">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="041fd-125">Exchange 偽装に使用するアカウントの簡易メール転送プロトコル (SMTP) アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="041fd-125">Represents the Simple Mail Transfer Protocol (SMTP) address of the account to use for Exchange Impersonation.</span></span> <span data-ttu-id="041fd-126">SMTP アドレスが指定されている場合は、ユーザーの SID を取得するために、さらに Active Directory 参照にコストがかかります。</span><span class="sxs-lookup"><span data-stu-id="041fd-126">If the SMTP address is supplied, it will cost an extra Active Directory lookup in order to obtain the SID of the user.</span></span> <span data-ttu-id="041fd-127">使用可能な場合は、SID または UPN を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="041fd-127">We recommend that you use the SID or UPN if they are available.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="041fd-128">親要素</span><span class="sxs-lookup"><span data-stu-id="041fd-128">Parent elements</span></span>

|<span data-ttu-id="041fd-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="041fd-129">**Element**</span></span>|<span data-ttu-id="041fd-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="041fd-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="041fd-131">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="041fd-131">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="041fd-132">要求の SOAP ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="041fd-132">Used in the SOAP header of a request.</span></span> <span data-ttu-id="041fd-133">この要素が存在する場合、発信者は**Exchangeimpersonation**要素内に含まれるアカウントを偽装しようとしています。</span><span class="sxs-lookup"><span data-stu-id="041fd-133">When this element is present, the caller is trying to impersonate the account that is contained within the **ExchangeImpersonation** element.</span></span>  <br/> <span data-ttu-id="041fd-134">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="041fd-134">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="041fd-135">注釈</span><span class="sxs-lookup"><span data-stu-id="041fd-135">Remarks</span></span>

<span data-ttu-id="041fd-136">呼び出し元のアカウントには、偽装するメールボックスを含むメールボックスデータベース、または Active Directory ユーザーまたは連絡先オブジェクトのいずれかで、クライアントアクセスサーバーおよび**exch-** **exch**権限が必要です。</span><span class="sxs-lookup"><span data-stu-id="041fd-136">The calling account must have the **ms-exch-impersonation** right on the Client Access server and the **ms-exch-MayImpersonate** right on either the mailbox database that contains the mailbox to impersonate or the Active Directory user or contact object.</span></span> 
  
<span data-ttu-id="041fd-137">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="041fd-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="041fd-138">要素の情報</span><span class="sxs-lookup"><span data-stu-id="041fd-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="041fd-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="041fd-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="041fd-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="041fd-140">Schema name</span></span>  <br/> |<span data-ttu-id="041fd-141">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="041fd-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="041fd-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="041fd-142">Validation file</span></span>  <br/> |<span data-ttu-id="041fd-143">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="041fd-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="041fd-144">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="041fd-144">Can be empty</span></span>  <br/> |<span data-ttu-id="041fd-145">正しくない</span><span class="sxs-lookup"><span data-stu-id="041fd-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="041fd-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="041fd-146">See also</span></span>

- [<span data-ttu-id="041fd-147">EWS でのサーバー間認証</span><span class="sxs-lookup"><span data-stu-id="041fd-147">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

