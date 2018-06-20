---
title: OfficeLocation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OfficeLocation
api_type:
- schema
ms.assetid: 88f314a1-b5cb-47aa-bbae-324561e3a5e3
description: 事業所の要素は、連絡先のオフィスの場所を表します。
ms.openlocfilehash: 4c51602b14840ba6d8551f6e324fd0f9ec245782
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832643"
---
# <a name="officelocation"></a><span data-ttu-id="ab49e-103">OfficeLocation</span><span class="sxs-lookup"><span data-stu-id="ab49e-103">OfficeLocation</span></span>

<span data-ttu-id="ab49e-104">**事業所**の要素は、連絡先のオフィスの場所を表します。</span><span class="sxs-lookup"><span data-stu-id="ab49e-104">The **OfficeLocation** element represents the office location of a contact.</span></span> 
  
```xml
<OfficeLocation/>
```

 <span data-ttu-id="ab49e-105">**string**</span><span class="sxs-lookup"><span data-stu-id="ab49e-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ab49e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ab49e-106">Attributes and elements</span></span>

<span data-ttu-id="ab49e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ab49e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ab49e-108">属性</span><span class="sxs-lookup"><span data-stu-id="ab49e-108">Attributes</span></span>

<span data-ttu-id="ab49e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ab49e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ab49e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ab49e-110">Child elements</span></span>

<span data-ttu-id="ab49e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ab49e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ab49e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ab49e-112">Parent elements</span></span>

|<span data-ttu-id="ab49e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ab49e-113">**Element**</span></span>|<span data-ttu-id="ab49e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ab49e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ab49e-115">Contact</span><span class="sxs-lookup"><span data-stu-id="ab49e-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="ab49e-116">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="ab49e-116">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ab49e-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ab49e-117">Text value</span></span>

<span data-ttu-id="ab49e-118">テキスト値は、この要素が使用される場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="ab49e-118">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ab49e-119">備考</span><span class="sxs-lookup"><span data-stu-id="ab49e-119">Remarks</span></span>

<span data-ttu-id="ab49e-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="ab49e-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ab49e-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="ab49e-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ab49e-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="ab49e-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ab49e-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ab49e-123">Schema name</span></span>  <br/> |<span data-ttu-id="ab49e-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ab49e-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="ab49e-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ab49e-125">Validation file</span></span>  <br/> |<span data-ttu-id="ab49e-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ab49e-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ab49e-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ab49e-127">Can be empty</span></span>  <br/> |<span data-ttu-id="ab49e-128">False</span><span class="sxs-lookup"><span data-stu-id="ab49e-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ab49e-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="ab49e-129">See also</span></span>



- [<span data-ttu-id="ab49e-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ab49e-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ab49e-131">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="ab49e-131">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="ab49e-132">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="ab49e-132">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="ab49e-133">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="ab49e-133">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

