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
ms.openlocfilehash: b609abed481359fa6562f41a551645eb613ddfa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468881"
---
# <a name="physicaladdresses"></a><span data-ttu-id="379fb-103">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="379fb-103">PhysicalAddresses</span></span>

<span data-ttu-id="379fb-104">**Physicaladdresses**要素には、連絡先に関連付けられている物理アドレスのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="379fb-104">The **PhysicalAddresses** element contains a collection of physical addresses that are associated with a contact.</span></span> 
  
```xml
<PhysicalAddresses>
   <Entry/>
</PhysicalAddresses>
```

 <span data-ttu-id="379fb-105">**PhysicalAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="379fb-105">**PhysicalAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="379fb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="379fb-106">Attributes and elements</span></span>

<span data-ttu-id="379fb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="379fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="379fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="379fb-108">Attributes</span></span>

<span data-ttu-id="379fb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="379fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="379fb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="379fb-110">Child elements</span></span>

|<span data-ttu-id="379fb-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="379fb-111">**Element**</span></span>|<span data-ttu-id="379fb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="379fb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="379fb-113">Entry (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="379fb-113">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md) <br/> |<span data-ttu-id="379fb-114">連絡先アイテムの単一の物理アドレスを記述します。</span><span class="sxs-lookup"><span data-stu-id="379fb-114">Describes a single physical address for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="379fb-115">親要素</span><span class="sxs-lookup"><span data-stu-id="379fb-115">Parent elements</span></span>

|<span data-ttu-id="379fb-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="379fb-116">**Element**</span></span>|<span data-ttu-id="379fb-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="379fb-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="379fb-118">Contact</span><span class="sxs-lookup"><span data-stu-id="379fb-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="379fb-119">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="379fb-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="379fb-120">注釈</span><span class="sxs-lookup"><span data-stu-id="379fb-120">Remarks</span></span>

<span data-ttu-id="379fb-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="379fb-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="379fb-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="379fb-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="379fb-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="379fb-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="379fb-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="379fb-124">Schema name</span></span>  <br/> |<span data-ttu-id="379fb-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="379fb-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="379fb-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="379fb-126">Validation file</span></span>  <br/> |<span data-ttu-id="379fb-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="379fb-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="379fb-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="379fb-128">Can be empty</span></span>  <br/> |<span data-ttu-id="379fb-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="379fb-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="379fb-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="379fb-130">See also</span></span>



- [<span data-ttu-id="379fb-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="379fb-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="379fb-132">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="379fb-132">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="379fb-133">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="379fb-133">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="379fb-134">連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="379fb-134">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

