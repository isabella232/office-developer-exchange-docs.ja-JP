---
title: SID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SID
api_type:
- schema
ms.assetid: 2f33b29b-163b-4106-a74d-6fb76ec38951
description: SID 要素は、偽装または代理人アクセスに使用するアカウントのセキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。
ms.openlocfilehash: 0e3f740e9a056f7c0042049d97757b5f2d3c441d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468048"
---
# <a name="sid"></a><span data-ttu-id="16098-103">SID</span><span class="sxs-lookup"><span data-stu-id="16098-103">SID</span></span>

<span data-ttu-id="16098-104">**Sid**要素は、偽装または代理人アクセスに使用するアカウントのセキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="16098-104">The **SID** element represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation or delegate access.</span></span> 
  
```xml
<SID/>
```

 <span data-ttu-id="16098-105">**SIDType**</span><span class="sxs-lookup"><span data-stu-id="16098-105">**SIDType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16098-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="16098-106">Attributes and elements</span></span>

<span data-ttu-id="16098-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="16098-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16098-108">属性</span><span class="sxs-lookup"><span data-stu-id="16098-108">Attributes</span></span>

<span data-ttu-id="16098-109">なし。</span><span class="sxs-lookup"><span data-stu-id="16098-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16098-110">子要素</span><span class="sxs-lookup"><span data-stu-id="16098-110">Child elements</span></span>

<span data-ttu-id="16098-111">なし。</span><span class="sxs-lookup"><span data-stu-id="16098-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="16098-112">親要素</span><span class="sxs-lookup"><span data-stu-id="16098-112">Parent elements</span></span>

|<span data-ttu-id="16098-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="16098-113">**Element**</span></span>|<span data-ttu-id="16098-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="16098-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16098-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="16098-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="16098-116">ExchangeImpersonation SOAP ヘッダーを使用する場合に偽装するアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="16098-116">Represents an account to impersonate when using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="16098-117">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="16098-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="16098-118">UserId</span><span class="sxs-lookup"><span data-stu-id="16098-118">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="16098-119">代理ユーザーまたはフォルダーアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="16098-119">Identifies a delegate user or a user with folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="16098-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="16098-120">Text value</span></span>

<span data-ttu-id="16098-121">テキスト値は、SID の文字列表現です。</span><span class="sxs-lookup"><span data-stu-id="16098-121">The text value is a string representation of a SID.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="16098-122">注釈</span><span class="sxs-lookup"><span data-stu-id="16098-122">Remarks</span></span>

<span data-ttu-id="16098-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="16098-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16098-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="16098-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16098-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="16098-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="16098-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="16098-126">Schema Name</span></span>  <br/> |<span data-ttu-id="16098-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="16098-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="16098-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="16098-128">Validation File</span></span>  <br/> |<span data-ttu-id="16098-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="16098-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="16098-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="16098-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="16098-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="16098-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16098-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="16098-132">See also</span></span>



- [<span data-ttu-id="16098-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="16098-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

