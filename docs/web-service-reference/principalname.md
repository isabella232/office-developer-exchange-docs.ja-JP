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
description: PrincipalName 要素は、Exchange の偽装に使用するアカウントのユーザー プリンシパル名 (UPN) を表します。
ms.openlocfilehash: d8557ce0435a11a5602372517db1f576028a9c97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832882"
---
# <a name="principalname"></a><span data-ttu-id="8515a-103">PrincipalName</span><span class="sxs-lookup"><span data-stu-id="8515a-103">PrincipalName</span></span>

<span data-ttu-id="8515a-104">**PrincipalName**要素は、Exchange の偽装に使用するアカウントのユーザー プリンシパル名 (UPN) を表します。</span><span class="sxs-lookup"><span data-stu-id="8515a-104">The **PrincipalName** element represents the user principal name (UPN) of the account to be used for Exchange impersonation.</span></span> 
  
```xml
<PrincipalName/>
```

 <span data-ttu-id="8515a-105">**PrincipalNameType**</span><span class="sxs-lookup"><span data-stu-id="8515a-105">**PrincipalNameType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8515a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8515a-106">Attributes and elements</span></span>

<span data-ttu-id="8515a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8515a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8515a-108">属性</span><span class="sxs-lookup"><span data-stu-id="8515a-108">Attributes</span></span>

<span data-ttu-id="8515a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8515a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8515a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8515a-110">Child elements</span></span>

<span data-ttu-id="8515a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8515a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8515a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8515a-112">Parent elements</span></span>

|<span data-ttu-id="8515a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8515a-113">**Element**</span></span>|<span data-ttu-id="8515a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8515a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8515a-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="8515a-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="8515a-116">ExchangeImpersonation SOAP ヘッダーを使用する際に偽装するアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="8515a-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="8515a-117">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="8515a-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8515a-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8515a-118">Text value</span></span>

<span data-ttu-id="8515a-119">テキスト値は、ユーザーの UPN を表します。</span><span class="sxs-lookup"><span data-stu-id="8515a-119">The text value represents the UPN of a user.</span></span> <span data-ttu-id="8515a-120">この値は、Active Directory ディレクトリ サービス内のユーザー オブジェクトに存在します。</span><span class="sxs-lookup"><span data-stu-id="8515a-120">This value exists on the user object in the Active Directory directory service.</span></span> <span data-ttu-id="8515a-121">ユーザー ログオン名とユーザー アカウントが次の形式で、配置されているドメインを識別するドメイン名が含まれます: `someone@example.com`。</span><span class="sxs-lookup"><span data-stu-id="8515a-121">This contains the user logon name and a domain name that identifies the domain in which the user account is located, in the following format:  `someone@example.com`.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8515a-122">備考</span><span class="sxs-lookup"><span data-stu-id="8515a-122">Remarks</span></span>

<span data-ttu-id="8515a-123">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8515a-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8515a-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="8515a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8515a-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="8515a-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8515a-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8515a-126">Schema Name</span></span>  <br/> |<span data-ttu-id="8515a-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8515a-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="8515a-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8515a-128">Validation File</span></span>  <br/> |<span data-ttu-id="8515a-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8515a-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8515a-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8515a-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="8515a-131">False</span><span class="sxs-lookup"><span data-stu-id="8515a-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8515a-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="8515a-132">See also</span></span>



- [<span data-ttu-id="8515a-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8515a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="8515a-134">EWS でのサーバーからサーバーへの承認</span><span class="sxs-lookup"><span data-stu-id="8515a-134">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

