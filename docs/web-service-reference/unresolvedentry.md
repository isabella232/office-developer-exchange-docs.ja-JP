---
title: UnresolvedEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnresolvedEntry
api_type:
- schema
ms.assetid: 5ac6116a-3b24-40f8-a877-dbe9a6935919
description: UnresolvedEntry 要素には、解決するのには、連絡先または配布リストの名前が含まれています。
ms.openlocfilehash: 98b447cd49685b49f73f75f12d921a65749be245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839812"
---
# <a name="unresolvedentry"></a><span data-ttu-id="1fda8-103">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="1fda8-103">UnresolvedEntry</span></span>

<span data-ttu-id="1fda8-104">**UnresolvedEntry**要素には、解決するのには、連絡先または配布リストの名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1fda8-104">The **UnresolvedEntry** element contains the name of a contact or distribution list to resolve.</span></span> 
  
[<span data-ttu-id="1fda8-105">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="1fda8-105">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="1fda8-106">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="1fda8-106">UnresolvedEntry</span></span>](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 <span data-ttu-id="1fda8-107">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="1fda8-107">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1fda8-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1fda8-108">Attributes and elements</span></span>

<span data-ttu-id="1fda8-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1fda8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1fda8-110">属性</span><span class="sxs-lookup"><span data-stu-id="1fda8-110">Attributes</span></span>

<span data-ttu-id="1fda8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1fda8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1fda8-112">子要素</span><span class="sxs-lookup"><span data-stu-id="1fda8-112">Child elements</span></span>

<span data-ttu-id="1fda8-113">なし。</span><span class="sxs-lookup"><span data-stu-id="1fda8-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1fda8-114">親要素</span><span class="sxs-lookup"><span data-stu-id="1fda8-114">Parent elements</span></span>

|<span data-ttu-id="1fda8-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="1fda8-115">**Element**</span></span>|<span data-ttu-id="1fda8-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="1fda8-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1fda8-117">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="1fda8-117">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="1fda8-118">あいまいな名前を解決する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="1fda8-118">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1fda8-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1fda8-119">Text value</span></span>

<span data-ttu-id="1fda8-120">テキスト値は、パブリックの連絡先または配布リストの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="1fda8-120">The text value represents the name of a public contact or distribution list.</span></span> <span data-ttu-id="1fda8-121">文字列の長さの最小値は、1 つの文字です。</span><span class="sxs-lookup"><span data-stu-id="1fda8-121">The minimum length of the string is one character.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1fda8-122">備考</span><span class="sxs-lookup"><span data-stu-id="1fda8-122">Remarks</span></span>

<span data-ttu-id="1fda8-123">に対して次のフィールドの名前を解決するのにはこの要素のテキスト値を使用します。</span><span class="sxs-lookup"><span data-stu-id="1fda8-123">The text value of this element is used to resolve names against the following fields:</span></span>
  
- <span data-ttu-id="1fda8-124">名前</span><span class="sxs-lookup"><span data-stu-id="1fda8-124">First name</span></span>
    
- <span data-ttu-id="1fda8-125">名字</span><span class="sxs-lookup"><span data-stu-id="1fda8-125">Last name</span></span>
    
- <span data-ttu-id="1fda8-126">表示名</span><span class="sxs-lookup"><span data-stu-id="1fda8-126">Display name</span></span>
    
- <span data-ttu-id="1fda8-127">氏名</span><span class="sxs-lookup"><span data-stu-id="1fda8-127">Full name</span></span>
    
- <span data-ttu-id="1fda8-128">Office</span><span class="sxs-lookup"><span data-stu-id="1fda8-128">Office</span></span>
    
- <span data-ttu-id="1fda8-129">Alias</span><span class="sxs-lookup"><span data-stu-id="1fda8-129">Alias</span></span>
    
- <span data-ttu-id="1fda8-130">SMTP アドレス</span><span class="sxs-lookup"><span data-stu-id="1fda8-130">SMTP address</span></span>
    
<span data-ttu-id="1fda8-131">プレフィックスが付けられたルーティングなど、smtp または sip、電子メール アドレスは、複数値配列に保存されます。</span><span class="sxs-lookup"><span data-stu-id="1fda8-131">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="1fda8-132">[ResolveNames 操作](resolvenames-operation.md)は、ルーティングの種類を「sip:User1@Contoso.com」など、未解決の名前の先頭に追加するときに、その配列の各値に対して部分的一致を実行します。</span><span class="sxs-lookup"><span data-stu-id="1fda8-132">The [ResolveNames operation](resolvenames-operation.md) performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="1fda8-133">ルーティングの種類を指定しない場合**ResolveNames**操作が既定の smtp ルーティングの種類に、照合するプライマリ SMTP アドレスのプロパティでは、および複数値の配列を検索します。</span><span class="sxs-lookup"><span data-stu-id="1fda8-133">If you don't specify a routing type, the **ResolveNames** operation will default to the routing type of smtp, match it to a primary SMTP address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="1fda8-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1fda8-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1fda8-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="1fda8-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1fda8-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="1fda8-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1fda8-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1fda8-137">Schema Name</span></span>  <br/> |<span data-ttu-id="1fda8-138">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1fda8-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1fda8-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1fda8-139">Validation File</span></span>  <br/> |<span data-ttu-id="1fda8-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1fda8-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1fda8-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1fda8-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="1fda8-142">False</span><span class="sxs-lookup"><span data-stu-id="1fda8-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1fda8-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="1fda8-143">See also</span></span>



[<span data-ttu-id="1fda8-144">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="1fda8-144">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="1fda8-145">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1fda8-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

