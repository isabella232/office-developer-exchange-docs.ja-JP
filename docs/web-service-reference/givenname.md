---
title: GivenName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GivenName
api_type:
- schema
ms.assetid: 8efc46fd-6056-4439-9af3-fc9e13ee6d9a
description: GivenName の要素には、連絡先の名前が含まれています。
ms.openlocfilehash: a9c8e6b075a480bc54414d0ead11918a50223b56
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831710"
---
# <a name="givenname"></a><span data-ttu-id="9929f-103">GivenName</span><span class="sxs-lookup"><span data-stu-id="9929f-103">GivenName</span></span>

<span data-ttu-id="9929f-104">**GivenName**の要素には、連絡先の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9929f-104">The **GivenName** element contains a contact's given name.</span></span> 
  
```xml
<GivenName/>
```

 <span data-ttu-id="9929f-105">**string**</span><span class="sxs-lookup"><span data-stu-id="9929f-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9929f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9929f-106">Attributes and elements</span></span>

<span data-ttu-id="9929f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9929f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9929f-108">属性</span><span class="sxs-lookup"><span data-stu-id="9929f-108">Attributes</span></span>

<span data-ttu-id="9929f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9929f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9929f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9929f-110">Child elements</span></span>

<span data-ttu-id="9929f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9929f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9929f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9929f-112">Parent elements</span></span>

|<span data-ttu-id="9929f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9929f-113">**Element**</span></span>|<span data-ttu-id="9929f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9929f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9929f-115">Contact</span><span class="sxs-lookup"><span data-stu-id="9929f-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="9929f-116">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="9929f-116">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9929f-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9929f-117">Text value</span></span>

<span data-ttu-id="9929f-118">連絡先の名前を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="9929f-118">A text value that represents a contact's given name is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9929f-119">備考</span><span class="sxs-lookup"><span data-stu-id="9929f-119">Remarks</span></span>

<span data-ttu-id="9929f-120">指定された名前は、通常、ユーザーの名です。</span><span class="sxs-lookup"><span data-stu-id="9929f-120">A given name is usually a person's first name.</span></span>
  
<span data-ttu-id="9929f-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="9929f-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9929f-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="9929f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9929f-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="9929f-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9929f-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9929f-124">Schema name</span></span>  <br/> |<span data-ttu-id="9929f-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9929f-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="9929f-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9929f-126">Validation file</span></span>  <br/> |<span data-ttu-id="9929f-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9929f-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9929f-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9929f-128">Can be empty</span></span>  <br/> |<span data-ttu-id="9929f-129">False</span><span class="sxs-lookup"><span data-stu-id="9929f-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9929f-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="9929f-130">See also</span></span>



- [<span data-ttu-id="9929f-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9929f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="9929f-132">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="9929f-132">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="9929f-133">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="9929f-133">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="9929f-134">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="9929f-134">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

