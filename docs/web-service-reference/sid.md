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
description: SID 要素では、偽装の使用またはアクセスを委任するようにアカウントのセキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。
ms.openlocfilehash: efcea42c12ec1d26ea31fdb8de337c37a2338a96
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833492"
---
# <a name="sid"></a><span data-ttu-id="21dc9-103">SID</span><span class="sxs-lookup"><span data-stu-id="21dc9-103">SID</span></span>

<span data-ttu-id="21dc9-104">**SID**要素では、偽装の使用またはアクセスを委任するようにアカウントのセキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="21dc9-104">The **SID** element represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation or delegate access.</span></span> 
  
```xml
<SID/>
```

 <span data-ttu-id="21dc9-105">**SIDType**</span><span class="sxs-lookup"><span data-stu-id="21dc9-105">**SIDType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21dc9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="21dc9-106">Attributes and elements</span></span>

<span data-ttu-id="21dc9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="21dc9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21dc9-108">属性</span><span class="sxs-lookup"><span data-stu-id="21dc9-108">Attributes</span></span>

<span data-ttu-id="21dc9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="21dc9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21dc9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="21dc9-110">Child elements</span></span>

<span data-ttu-id="21dc9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="21dc9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="21dc9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="21dc9-112">Parent elements</span></span>

|<span data-ttu-id="21dc9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="21dc9-113">**Element**</span></span>|<span data-ttu-id="21dc9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="21dc9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21dc9-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="21dc9-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="21dc9-116">ExchangeImpersonation SOAP ヘッダーを使用するときに偽装するアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="21dc9-116">Represents an account to impersonate when using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="21dc9-117">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="21dc9-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="21dc9-118">ユーザー Id</span><span class="sxs-lookup"><span data-stu-id="21dc9-118">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="21dc9-119">フォルダーのアクセス許可を持つ代理人のユーザー、またはユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="21dc9-119">Identifies a delegate user or a user with folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="21dc9-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="21dc9-120">Text value</span></span>

<span data-ttu-id="21dc9-121">テキスト値は、SID の文字列表現です。</span><span class="sxs-lookup"><span data-stu-id="21dc9-121">The text value is a string representation of a SID.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="21dc9-122">備考</span><span class="sxs-lookup"><span data-stu-id="21dc9-122">Remarks</span></span>

<span data-ttu-id="21dc9-123">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="21dc9-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21dc9-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="21dc9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21dc9-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="21dc9-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="21dc9-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="21dc9-126">Schema Name</span></span>  <br/> |<span data-ttu-id="21dc9-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="21dc9-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="21dc9-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="21dc9-128">Validation File</span></span>  <br/> |<span data-ttu-id="21dc9-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="21dc9-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="21dc9-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="21dc9-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="21dc9-131">False</span><span class="sxs-lookup"><span data-stu-id="21dc9-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21dc9-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="21dc9-132">See also</span></span>



- [<span data-ttu-id="21dc9-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="21dc9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

