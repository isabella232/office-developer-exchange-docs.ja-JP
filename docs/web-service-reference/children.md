---
title: Children
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Children
api_type:
- schema
ms.assetid: ceaffddd-f9bc-43ea-b348-a20fdade738f
description: 子要素には、連絡先の子供の名前が含まれています。
ms.openlocfilehash: 9b1e06529fcf74850755daefc299242cfbf81f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759620"
---
# <a name="children"></a><span data-ttu-id="c1329-103">Children</span><span class="sxs-lookup"><span data-stu-id="c1329-103">Children</span></span>

<span data-ttu-id="c1329-104">**子**要素には、連絡先の子供の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c1329-104">The **Children** element contains the names of a contact's children.</span></span> 
  
```xml
<Children>
   <String/>
</Children>
```

 <span data-ttu-id="c1329-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="c1329-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c1329-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c1329-106">Attributes and elements</span></span>

<span data-ttu-id="c1329-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c1329-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1329-108">属性</span><span class="sxs-lookup"><span data-stu-id="c1329-108">Attributes</span></span>

<span data-ttu-id="c1329-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c1329-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1329-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c1329-110">Child elements</span></span>

|<span data-ttu-id="c1329-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="c1329-111">**Element**</span></span>|<span data-ttu-id="c1329-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c1329-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1329-113">String</span><span class="sxs-lookup"><span data-stu-id="c1329-113">String</span></span>](string.md) <br/> |<span data-ttu-id="c1329-114">メンバーの子の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c1329-114">Contains the name of a contact's child.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c1329-115">親要素</span><span class="sxs-lookup"><span data-stu-id="c1329-115">Parent elements</span></span>

|<span data-ttu-id="c1329-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="c1329-116">**Element**</span></span>|<span data-ttu-id="c1329-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="c1329-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1329-118">Contact</span><span class="sxs-lookup"><span data-stu-id="c1329-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c1329-119">Exchange ストア内の連絡先を表します。</span><span class="sxs-lookup"><span data-stu-id="c1329-119">Represents a contact in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c1329-120">備考</span><span class="sxs-lookup"><span data-stu-id="c1329-120">Remarks</span></span>

<span data-ttu-id="c1329-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="c1329-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1329-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="c1329-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1329-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="c1329-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c1329-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c1329-124">Schema name</span></span>  <br/> |<span data-ttu-id="c1329-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c1329-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c1329-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c1329-126">Validation file</span></span>  <br/> |<span data-ttu-id="c1329-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c1329-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c1329-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c1329-128">Can be empty</span></span>  <br/> |<span data-ttu-id="c1329-129">False</span><span class="sxs-lookup"><span data-stu-id="c1329-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1329-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="c1329-130">See also</span></span>



- [<span data-ttu-id="c1329-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c1329-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

