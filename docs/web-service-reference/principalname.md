---
title: PrincipalName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrincipalName
api_type:
- schema
ms.assetid: 88c142d4-0bc7-43ea-a997-d7200664d900
description: PrincipalName 要素は、Exchange の偽装に使用されるアカウントのユーザープリンシパル名 (UPN) を表します。
ms.openlocfilehash: 31412c1461264e28bf8d52c957a457e8d1e847ef
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44440191"
---
# <a name="principalname"></a><span data-ttu-id="86816-103">PrincipalName</span><span class="sxs-lookup"><span data-stu-id="86816-103">PrincipalName</span></span>

<span data-ttu-id="86816-104">**PrincipalName**要素は、Exchange の偽装に使用されるアカウントのユーザープリンシパル名 (UPN) を表します。</span><span class="sxs-lookup"><span data-stu-id="86816-104">The **PrincipalName** element represents the user principal name (UPN) of the account to be used for Exchange impersonation.</span></span> 
  
```xml
<PrincipalName/>
```

 <span data-ttu-id="86816-105">**PrincipalNameType**</span><span class="sxs-lookup"><span data-stu-id="86816-105">**PrincipalNameType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86816-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="86816-106">Attributes and elements</span></span>

<span data-ttu-id="86816-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="86816-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86816-108">属性</span><span class="sxs-lookup"><span data-stu-id="86816-108">Attributes</span></span>

<span data-ttu-id="86816-109">なし。</span><span class="sxs-lookup"><span data-stu-id="86816-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86816-110">子要素</span><span class="sxs-lookup"><span data-stu-id="86816-110">Child elements</span></span>

<span data-ttu-id="86816-111">なし。</span><span class="sxs-lookup"><span data-stu-id="86816-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="86816-112">親要素</span><span class="sxs-lookup"><span data-stu-id="86816-112">Parent elements</span></span>

|<span data-ttu-id="86816-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="86816-113">**Element**</span></span>|<span data-ttu-id="86816-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="86816-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86816-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="86816-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="86816-116">ExchangeImpersonation SOAP ヘッダーを使用しているときに偽装するアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="86816-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="86816-117">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="86816-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="86816-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="86816-118">Text value</span></span>

<span data-ttu-id="86816-119">Text 値は、ユーザーの UPN を表します。</span><span class="sxs-lookup"><span data-stu-id="86816-119">The text value represents the UPN of a user.</span></span> <span data-ttu-id="86816-120">この値は、Active Directory ディレクトリサービスのユーザーオブジェクトに存在します。</span><span class="sxs-lookup"><span data-stu-id="86816-120">This value exists on the user object in the Active Directory directory service.</span></span> <span data-ttu-id="86816-121">これには、次の形式で、ユーザーアカウントが存在するドメインを識別するユーザーログオン名とドメイン名が含まれています `someone@example.com` 。</span><span class="sxs-lookup"><span data-stu-id="86816-121">This contains the user logon name and a domain name that identifies the domain in which the user account is located, in the following format:  `someone@example.com`.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="86816-122">注釈</span><span class="sxs-lookup"><span data-stu-id="86816-122">Remarks</span></span>

<span data-ttu-id="86816-123">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="86816-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86816-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="86816-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86816-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="86816-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="86816-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="86816-126">Schema Name</span></span>  <br/> |<span data-ttu-id="86816-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="86816-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="86816-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="86816-128">Validation File</span></span>  <br/> |<span data-ttu-id="86816-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="86816-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="86816-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="86816-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="86816-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="86816-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86816-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="86816-132">See also</span></span>



- [<span data-ttu-id="86816-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="86816-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="86816-134">EWS でのサーバー間認証</span><span class="sxs-lookup"><span data-stu-id="86816-134">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

