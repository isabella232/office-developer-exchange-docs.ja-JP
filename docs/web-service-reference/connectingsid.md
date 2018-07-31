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
description: ConnectingSID 要素は、ExchangeImpersonation SOAP ヘッダーを使用する際に偽装するアカウントを表します。
ms.openlocfilehash: a30f11721506989a84f52dd04c328974f4483956
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354338"
---
# <a name="connectingsid"></a><span data-ttu-id="1f64b-103">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="1f64b-103">ConnectingSID</span></span>

<span data-ttu-id="1f64b-104">**ConnectingSID**要素は、ExchangeImpersonation SOAP ヘッダーを使用する際に偽装するアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="1f64b-104">The **ConnectingSID** element represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span> 
  
- [<span data-ttu-id="1f64b-105">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="1f64b-105">ExchangeImpersonation</span></span>](exchangeimpersonation.md) 
- [<span data-ttu-id="1f64b-106">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="1f64b-106">ConnectingSID</span></span>](connectingsid.md)
  
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

<span data-ttu-id="1f64b-107">**ConnectingSIDType**</span><span class="sxs-lookup"><span data-stu-id="1f64b-107">**ConnectingSIDType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1f64b-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1f64b-108">Attributes and elements</span></span>

<span data-ttu-id="1f64b-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f64b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f64b-110">属性</span><span class="sxs-lookup"><span data-stu-id="1f64b-110">Attributes</span></span>

<span data-ttu-id="1f64b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1f64b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f64b-112">子要素</span><span class="sxs-lookup"><span data-stu-id="1f64b-112">Child elements</span></span>

|<span data-ttu-id="1f64b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f64b-113">**Element**</span></span>|<span data-ttu-id="1f64b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f64b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f64b-115">PrincipalName</span><span class="sxs-lookup"><span data-stu-id="1f64b-115">PrincipalName</span></span>](principalname.md) <br/> |<span data-ttu-id="1f64b-116">偽装のために使用するアカウントのユーザー プリンシパル名 (UPN) を表します。</span><span class="sxs-lookup"><span data-stu-id="1f64b-116">Represents the user principal name (UPN) of the account to use for impersonation.</span></span> <span data-ttu-id="1f64b-117">UPN ドメイン ユーザー アカウントが存在する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1f64b-117">This should be the UPN for the domain where the user account exists.</span></span>  <br/> |
|[<span data-ttu-id="1f64b-118">SID</span><span class="sxs-lookup"><span data-stu-id="1f64b-118">SID</span></span>](sid.md) <br/> |<span data-ttu-id="1f64b-119">偽装に使用するアカウントのセキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="1f64b-119">Represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation.</span></span>  <br/> |
|[<span data-ttu-id="1f64b-120">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1f64b-120">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="1f64b-121">Exchange 偽装のために使用するアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="1f64b-121">Represents the primary Simple Mail Transfer Protocol (SMTP) address of the account to use for Exchange impersonation.</span></span> <span data-ttu-id="1f64b-122">プライマリ SMTP アドレスが指定されている場合、ユーザーの SID を取得するために Active Directory ディレクトリ サービスの参照は、追加のコストがかかります。</span><span class="sxs-lookup"><span data-stu-id="1f64b-122">If the primary SMTP address is supplied, it will cost an extra Active Directory directory service lookup in order to obtain the SID of the user.</span></span> <span data-ttu-id="1f64b-123">可能な場合、SID または UPN を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="1f64b-123">We recommend that you use the SID or UPN if they are available.</span></span>  <br/> |
|[<span data-ttu-id="1f64b-124">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1f64b-124">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="1f64b-125">Exchange 偽装のために使用するアカウントの簡易メール転送プロトコル (SMTP) アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="1f64b-125">Represents the Simple Mail Transfer Protocol (SMTP) address of the account to use for Exchange Impersonation.</span></span> <span data-ttu-id="1f64b-126">SMTP アドレスが指定されている場合、ユーザーの SID を取得するために、追加の Active Directory 検索のコストがかかります。</span><span class="sxs-lookup"><span data-stu-id="1f64b-126">If the SMTP address is supplied, it will cost an extra Active Directory lookup in order to obtain the SID of the user.</span></span> <span data-ttu-id="1f64b-127">可能な場合、SID または UPN を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="1f64b-127">We recommend that you use the SID or UPN if they are available.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f64b-128">親要素</span><span class="sxs-lookup"><span data-stu-id="1f64b-128">Parent elements</span></span>

|<span data-ttu-id="1f64b-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f64b-129">**Element**</span></span>|<span data-ttu-id="1f64b-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f64b-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f64b-131">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="1f64b-131">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="1f64b-132">要求の SOAP ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="1f64b-132">Used in the SOAP header of a request.</span></span> <span data-ttu-id="1f64b-133">この要素が存在する場合、呼び出し元が**ExchangeImpersonation**要素内に含まれているアカウントを偽装するとしています。</span><span class="sxs-lookup"><span data-stu-id="1f64b-133">When this element is present, the caller is trying to impersonate the account that is contained within the **ExchangeImpersonation** element.</span></span>  <br/> <span data-ttu-id="1f64b-134">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="1f64b-134">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1f64b-135">注釈</span><span class="sxs-lookup"><span data-stu-id="1f64b-135">Remarks</span></span>

<span data-ttu-id="1f64b-136">呼び出し元のアカウントが必要でクライアント アクセス サーバーと**ms-exch-MayImpersonate** **ms の偽装 exch**上かを偽装するメールボックスを含むメールボックス データベースまたは Active Directory のユーザーまたは連絡先オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1f64b-136">The calling account must have the **ms-exch-impersonation** right on the Client Access server and the **ms-exch-MayImpersonate** right on either the mailbox database that contains the mailbox to impersonate or the Active Directory user or contact object.</span></span> 
  
<span data-ttu-id="1f64b-137">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1f64b-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f64b-138">要素情報</span><span class="sxs-lookup"><span data-stu-id="1f64b-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f64b-139">名前空間</span><span class="sxs-lookup"><span data-stu-id="1f64b-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1f64b-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1f64b-140">Schema name</span></span>  <br/> |<span data-ttu-id="1f64b-141">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1f64b-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="1f64b-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1f64b-142">Validation file</span></span>  <br/> |<span data-ttu-id="1f64b-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1f64b-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1f64b-144">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1f64b-144">Can be empty</span></span>  <br/> |<span data-ttu-id="1f64b-145">False</span><span class="sxs-lookup"><span data-stu-id="1f64b-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f64b-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f64b-146">See also</span></span>

- [<span data-ttu-id="1f64b-147">EWS でのサーバーからサーバーへの承認</span><span class="sxs-lookup"><span data-stu-id="1f64b-147">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

