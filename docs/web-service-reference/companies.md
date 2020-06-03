---
title: 会社名
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
description: '[会社] 要素は、連絡先またはタスクに関連付けられている会社のコレクションを表します。'
ms.openlocfilehash: eda2b92f3ca874aeeceef6a0935a49a98af0ec39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461451"
---
# <a name="companies"></a><span data-ttu-id="a622b-103">会社名</span><span class="sxs-lookup"><span data-stu-id="a622b-103">Companies</span></span>

<span data-ttu-id="a622b-104">[**会社**] 要素は、連絡先またはタスクに関連付けられている会社のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="a622b-104">The **Companies** element represents the collection of companies that are associated with a contact or task.</span></span> 
  
```xml
<Companies>
   <String/>
</Companies>
```

 <span data-ttu-id="a622b-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="a622b-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a622b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a622b-106">Attributes and elements</span></span>

<span data-ttu-id="a622b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a622b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a622b-108">属性</span><span class="sxs-lookup"><span data-stu-id="a622b-108">Attributes</span></span>

<span data-ttu-id="a622b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a622b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a622b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a622b-110">Child elements</span></span>

|<span data-ttu-id="a622b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a622b-111">**Element**</span></span>|<span data-ttu-id="a622b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a622b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a622b-113">String</span><span class="sxs-lookup"><span data-stu-id="a622b-113">String</span></span>](string.md) <br/> |<span data-ttu-id="a622b-114">会社の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="a622b-114">Represents the name of a company.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a622b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="a622b-115">Parent elements</span></span>

|<span data-ttu-id="a622b-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="a622b-116">**Element**</span></span>|<span data-ttu-id="a622b-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="a622b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a622b-118">Contact</span><span class="sxs-lookup"><span data-stu-id="a622b-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="a622b-119">Exchange ストア内の連絡先を表します。</span><span class="sxs-lookup"><span data-stu-id="a622b-119">Represents a contact in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a622b-120">タスク</span><span class="sxs-lookup"><span data-stu-id="a622b-120">Task</span></span>](task.md) <br/> |<span data-ttu-id="a622b-121">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="a622b-121">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a622b-122">注釈</span><span class="sxs-lookup"><span data-stu-id="a622b-122">Remarks</span></span>

<span data-ttu-id="a622b-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a622b-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a622b-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a622b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a622b-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="a622b-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a622b-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a622b-126">Schema name</span></span>  <br/> |<span data-ttu-id="a622b-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a622b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="a622b-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a622b-128">Validation file</span></span>  <br/> |<span data-ttu-id="a622b-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a622b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a622b-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a622b-130">Can be empty</span></span>  <br/> |<span data-ttu-id="a622b-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="a622b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a622b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="a622b-132">See also</span></span>



- [<span data-ttu-id="a622b-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a622b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

