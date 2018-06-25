---
title: Companies
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Companies
api_type:
- schema
ms.assetid: 5d9ea76f-e14d-4424-8842-0c3cc3305119
description: 企業の要素は、連絡先またはタスクに関連付けられている企業のコレクションを表します。
ms.openlocfilehash: 5b8ac20d4a02017881f941d12380fe29078f51cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759632"
---
# <a name="companies"></a><span data-ttu-id="04389-103">Companies</span><span class="sxs-lookup"><span data-stu-id="04389-103">Companies</span></span>

<span data-ttu-id="04389-104">**企業**の要素は、連絡先またはタスクに関連付けられている企業のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="04389-104">The **Companies** element represents the collection of companies that are associated with a contact or task.</span></span> 
  
```xml
<Companies>
   <String/>
</Companies>
```

 <span data-ttu-id="04389-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="04389-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04389-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="04389-106">Attributes and elements</span></span>

<span data-ttu-id="04389-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="04389-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04389-108">属性</span><span class="sxs-lookup"><span data-stu-id="04389-108">Attributes</span></span>

<span data-ttu-id="04389-109">なし。</span><span class="sxs-lookup"><span data-stu-id="04389-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04389-110">子要素</span><span class="sxs-lookup"><span data-stu-id="04389-110">Child elements</span></span>

|<span data-ttu-id="04389-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="04389-111">**Element**</span></span>|<span data-ttu-id="04389-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="04389-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04389-113">String</span><span class="sxs-lookup"><span data-stu-id="04389-113">String</span></span>](string.md) <br/> |<span data-ttu-id="04389-114">会社の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="04389-114">Represents the name of a company.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04389-115">親要素</span><span class="sxs-lookup"><span data-stu-id="04389-115">Parent elements</span></span>

|<span data-ttu-id="04389-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="04389-116">**Element**</span></span>|<span data-ttu-id="04389-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="04389-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04389-118">Contact</span><span class="sxs-lookup"><span data-stu-id="04389-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="04389-119">Exchange ストア内の連絡先を表します。</span><span class="sxs-lookup"><span data-stu-id="04389-119">Represents a contact in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="04389-120">タスク</span><span class="sxs-lookup"><span data-stu-id="04389-120">Task</span></span>](task.md) <br/> |<span data-ttu-id="04389-121">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="04389-121">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="04389-122">備考</span><span class="sxs-lookup"><span data-stu-id="04389-122">Remarks</span></span>

<span data-ttu-id="04389-123">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="04389-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04389-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="04389-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04389-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="04389-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04389-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="04389-126">Schema name</span></span>  <br/> |<span data-ttu-id="04389-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="04389-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="04389-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="04389-128">Validation file</span></span>  <br/> |<span data-ttu-id="04389-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="04389-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04389-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="04389-130">Can be empty</span></span>  <br/> |<span data-ttu-id="04389-131">False</span><span class="sxs-lookup"><span data-stu-id="04389-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04389-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="04389-132">See also</span></span>



- [<span data-ttu-id="04389-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="04389-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

