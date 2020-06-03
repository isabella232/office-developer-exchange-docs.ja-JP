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
description: UnresolvedEntry 要素には、解決する連絡先または配布リストの名前が含まれています。
ms.openlocfilehash: 0f157c1be6c327187456a795c4c1000b8c35b620
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459841"
---
# <a name="unresolvedentry"></a><span data-ttu-id="82c36-103">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="82c36-103">UnresolvedEntry</span></span>

<span data-ttu-id="82c36-104">**UnresolvedEntry**要素には、解決する連絡先または配布リストの名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="82c36-104">The **UnresolvedEntry** element contains the name of a contact or distribution list to resolve.</span></span> 
  
[<span data-ttu-id="82c36-105">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="82c36-105">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="82c36-106">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="82c36-106">UnresolvedEntry</span></span>](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 <span data-ttu-id="82c36-107">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="82c36-107">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="82c36-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="82c36-108">Attributes and elements</span></span>

<span data-ttu-id="82c36-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="82c36-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="82c36-110">属性</span><span class="sxs-lookup"><span data-stu-id="82c36-110">Attributes</span></span>

<span data-ttu-id="82c36-111">なし。</span><span class="sxs-lookup"><span data-stu-id="82c36-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="82c36-112">子要素</span><span class="sxs-lookup"><span data-stu-id="82c36-112">Child elements</span></span>

<span data-ttu-id="82c36-113">なし。</span><span class="sxs-lookup"><span data-stu-id="82c36-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="82c36-114">親要素</span><span class="sxs-lookup"><span data-stu-id="82c36-114">Parent elements</span></span>

|<span data-ttu-id="82c36-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="82c36-115">**Element**</span></span>|<span data-ttu-id="82c36-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="82c36-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="82c36-117">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="82c36-117">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="82c36-118">あいまいな名前を解決する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="82c36-118">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="82c36-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="82c36-119">Text value</span></span>

<span data-ttu-id="82c36-120">テキスト値は、パブリック連絡先または配布リストの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="82c36-120">The text value represents the name of a public contact or distribution list.</span></span> <span data-ttu-id="82c36-121">文字列の最小の長さは1文字です。</span><span class="sxs-lookup"><span data-stu-id="82c36-121">The minimum length of the string is one character.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="82c36-122">注釈</span><span class="sxs-lookup"><span data-stu-id="82c36-122">Remarks</span></span>

<span data-ttu-id="82c36-123">この要素のテキスト値は、次のフィールドに対して名前を解決するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="82c36-123">The text value of this element is used to resolve names against the following fields:</span></span>
  
- <span data-ttu-id="82c36-124">名</span><span class="sxs-lookup"><span data-stu-id="82c36-124">First name</span></span>
    
- <span data-ttu-id="82c36-125">姓</span><span class="sxs-lookup"><span data-stu-id="82c36-125">Last name</span></span>
    
- <span data-ttu-id="82c36-126">表示名</span><span class="sxs-lookup"><span data-stu-id="82c36-126">Display name</span></span>
    
- <span data-ttu-id="82c36-127">フル ネーム</span><span class="sxs-lookup"><span data-stu-id="82c36-127">Full name</span></span>
    
- <span data-ttu-id="82c36-128">Office</span><span class="sxs-lookup"><span data-stu-id="82c36-128">Office</span></span>
    
- <span data-ttu-id="82c36-129">エイリアス</span><span class="sxs-lookup"><span data-stu-id="82c36-129">Alias</span></span>
    
- <span data-ttu-id="82c36-130">SMTP アドレス</span><span class="sxs-lookup"><span data-stu-id="82c36-130">SMTP address</span></span>
    
<span data-ttu-id="82c36-131">Smtp、sip などのプレフィックス付きルーティングタイプを持つ電子メールアドレスは、複数値配列に保存されます。</span><span class="sxs-lookup"><span data-stu-id="82c36-131">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="82c36-132">[ResolveNames 操作](resolvenames-operation.md)は、未解決の名前の先頭 ("sip:User1@Contoso.com" など) にルーティングの種類を追加するときに、その配列の各値に対して部分一致を実行します。</span><span class="sxs-lookup"><span data-stu-id="82c36-132">The [ResolveNames operation](resolvenames-operation.md) performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="82c36-133">ルーティングの種類を指定しない場合、 **ResolveNames**操作は既定で smtp のルーティングの種類を使用し、それをプライマリ smtp アドレスプロパティに一致させます。複数値配列は検索しません。</span><span class="sxs-lookup"><span data-stu-id="82c36-133">If you don't specify a routing type, the **ResolveNames** operation will default to the routing type of smtp, match it to a primary SMTP address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="82c36-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="82c36-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="82c36-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="82c36-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="82c36-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="82c36-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="82c36-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="82c36-137">Schema Name</span></span>  <br/> |<span data-ttu-id="82c36-138">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="82c36-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="82c36-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="82c36-139">Validation File</span></span>  <br/> |<span data-ttu-id="82c36-140">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="82c36-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="82c36-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="82c36-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="82c36-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="82c36-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="82c36-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="82c36-143">See also</span></span>



[<span data-ttu-id="82c36-144">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="82c36-144">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="82c36-145">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="82c36-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

