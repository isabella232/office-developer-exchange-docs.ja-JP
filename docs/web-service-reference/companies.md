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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461451"
---
# <a name="companies"></a><span data-ttu-id="926b7-103">会社名</span><span class="sxs-lookup"><span data-stu-id="926b7-103">Companies</span></span>

<span data-ttu-id="926b7-104">[**会社**] 要素は、連絡先またはタスクに関連付けられている会社のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="926b7-104">The **Companies** element represents the collection of companies that are associated with a contact or task.</span></span> 
  
```xml
<Companies>
   <String/>
</Companies>
```

 <span data-ttu-id="926b7-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="926b7-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="926b7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="926b7-106">Attributes and elements</span></span>

<span data-ttu-id="926b7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="926b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="926b7-108">属性</span><span class="sxs-lookup"><span data-stu-id="926b7-108">Attributes</span></span>

<span data-ttu-id="926b7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="926b7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="926b7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="926b7-110">Child elements</span></span>

|<span data-ttu-id="926b7-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="926b7-111">**Element**</span></span>|<span data-ttu-id="926b7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="926b7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="926b7-113">String</span><span class="sxs-lookup"><span data-stu-id="926b7-113">String</span></span>](string.md) <br/> |<span data-ttu-id="926b7-114">会社の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="926b7-114">Represents the name of a company.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="926b7-115">親要素</span><span class="sxs-lookup"><span data-stu-id="926b7-115">Parent elements</span></span>

|<span data-ttu-id="926b7-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="926b7-116">**Element**</span></span>|<span data-ttu-id="926b7-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="926b7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="926b7-118">連絡先</span><span class="sxs-lookup"><span data-stu-id="926b7-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="926b7-119">Exchange ストア内の連絡先を表します。</span><span class="sxs-lookup"><span data-stu-id="926b7-119">Represents a contact in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="926b7-120">Task</span><span class="sxs-lookup"><span data-stu-id="926b7-120">Task</span></span>](task.md) <br/> |<span data-ttu-id="926b7-121">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="926b7-121">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="926b7-122">注釈</span><span class="sxs-lookup"><span data-stu-id="926b7-122">Remarks</span></span>

<span data-ttu-id="926b7-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="926b7-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="926b7-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="926b7-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="926b7-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="926b7-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="926b7-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="926b7-126">Schema name</span></span>  <br/> |<span data-ttu-id="926b7-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="926b7-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="926b7-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="926b7-128">Validation file</span></span>  <br/> |<span data-ttu-id="926b7-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="926b7-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="926b7-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="926b7-130">Can be empty</span></span>  <br/> |<span data-ttu-id="926b7-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="926b7-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="926b7-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="926b7-132">See also</span></span>



- [<span data-ttu-id="926b7-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="926b7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

