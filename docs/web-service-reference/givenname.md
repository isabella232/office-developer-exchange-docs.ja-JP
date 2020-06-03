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
description: GivenName 要素には、連絡先の指定した名前が含まれています。
ms.openlocfilehash: a22c5ef99844b55fa75f60acb8667ee423420336
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530135"
---
# <a name="givenname"></a><span data-ttu-id="27869-103">GivenName</span><span class="sxs-lookup"><span data-stu-id="27869-103">GivenName</span></span>

<span data-ttu-id="27869-104">**GivenName**要素には、連絡先の指定した名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="27869-104">The **GivenName** element contains a contact's given name.</span></span> 
  
```xml
<GivenName/>
```

 <span data-ttu-id="27869-105">**string**</span><span class="sxs-lookup"><span data-stu-id="27869-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27869-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="27869-106">Attributes and elements</span></span>

<span data-ttu-id="27869-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="27869-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27869-108">属性</span><span class="sxs-lookup"><span data-stu-id="27869-108">Attributes</span></span>

<span data-ttu-id="27869-109">なし。</span><span class="sxs-lookup"><span data-stu-id="27869-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27869-110">子要素</span><span class="sxs-lookup"><span data-stu-id="27869-110">Child elements</span></span>

<span data-ttu-id="27869-111">なし。</span><span class="sxs-lookup"><span data-stu-id="27869-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="27869-112">親要素</span><span class="sxs-lookup"><span data-stu-id="27869-112">Parent elements</span></span>

|<span data-ttu-id="27869-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="27869-113">**Element**</span></span>|<span data-ttu-id="27869-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="27869-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27869-115">Contact</span><span class="sxs-lookup"><span data-stu-id="27869-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="27869-116">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="27869-116">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="27869-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="27869-117">Text value</span></span>

<span data-ttu-id="27869-118">この要素を使用する場合、連絡先の指定された名前を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="27869-118">A text value that represents a contact's given name is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="27869-119">注釈</span><span class="sxs-lookup"><span data-stu-id="27869-119">Remarks</span></span>

<span data-ttu-id="27869-120">特定の名前は、通常、ユーザーの名になります。</span><span class="sxs-lookup"><span data-stu-id="27869-120">A given name is usually a person's first name.</span></span>
  
<span data-ttu-id="27869-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="27869-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27869-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="27869-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27869-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="27869-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="27869-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="27869-124">Schema name</span></span>  <br/> |<span data-ttu-id="27869-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="27869-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="27869-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="27869-126">Validation file</span></span>  <br/> |<span data-ttu-id="27869-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="27869-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="27869-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="27869-128">Can be empty</span></span>  <br/> |<span data-ttu-id="27869-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="27869-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27869-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="27869-130">See also</span></span>



- [<span data-ttu-id="27869-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="27869-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="27869-132">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="27869-132">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="27869-133">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="27869-133">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="27869-134">連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="27869-134">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

