---
title: PhysicalAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhysicalAddresses
api_type:
- schema
ms.assetid: 5276c5f2-9e08-43af-a0b2-da4ff1dcae2d
description: PhysicalAddresses 要素には、連絡先に関連付けられている物理アドレスのコレクションが含まれています。
ms.openlocfilehash: d4d5232312c735e389e9f5b0dbcb74f8614b6906
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832814"
---
# <a name="physicaladdresses"></a><span data-ttu-id="6be49-103">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="6be49-103">PhysicalAddresses</span></span>

<span data-ttu-id="6be49-104">**PhysicalAddresses**要素には、連絡先に関連付けられている物理アドレスのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6be49-104">The **PhysicalAddresses** element contains a collection of physical addresses that are associated with a contact.</span></span> 
  
```xml
<PhysicalAddresses>
   <Entry/>
</PhysicalAddresses>
```

 <span data-ttu-id="6be49-105">**PhysicalAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="6be49-105">**PhysicalAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6be49-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6be49-106">Attributes and elements</span></span>

<span data-ttu-id="6be49-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6be49-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6be49-108">属性</span><span class="sxs-lookup"><span data-stu-id="6be49-108">Attributes</span></span>

<span data-ttu-id="6be49-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6be49-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6be49-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6be49-110">Child elements</span></span>

|<span data-ttu-id="6be49-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6be49-111">**Element**</span></span>|<span data-ttu-id="6be49-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6be49-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6be49-113">エントリ (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="6be49-113">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md) <br/> |<span data-ttu-id="6be49-114">連絡先アイテムの 1 つの物理アドレスをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6be49-114">Describes a single physical address for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6be49-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6be49-115">Parent elements</span></span>

|<span data-ttu-id="6be49-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6be49-116">**Element**</span></span>|<span data-ttu-id="6be49-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6be49-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6be49-118">Contact</span><span class="sxs-lookup"><span data-stu-id="6be49-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="6be49-119">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6be49-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6be49-120">備考</span><span class="sxs-lookup"><span data-stu-id="6be49-120">Remarks</span></span>

<span data-ttu-id="6be49-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="6be49-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6be49-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="6be49-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6be49-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="6be49-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6be49-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6be49-124">Schema name</span></span>  <br/> |<span data-ttu-id="6be49-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6be49-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="6be49-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6be49-126">Validation file</span></span>  <br/> |<span data-ttu-id="6be49-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6be49-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6be49-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6be49-128">Can be empty</span></span>  <br/> |<span data-ttu-id="6be49-129">False</span><span class="sxs-lookup"><span data-stu-id="6be49-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6be49-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="6be49-130">See also</span></span>



- [<span data-ttu-id="6be49-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6be49-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="6be49-132">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="6be49-132">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="6be49-133">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="6be49-133">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="6be49-134">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="6be49-134">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

