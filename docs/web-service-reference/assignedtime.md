---
title: AssignedTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AssignedTime
api_type:
- schema
ms.assetid: 37b273a4-7595-47d5-87c5-32856d7a045b
description: AssignedTime 要素は、タスクが連絡先に割り当てられる時刻を表します。
ms.openlocfilehash: 26c3fd4e117a962c690d0fff0d4dad5b5c24dd0c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464729"
---
# <a name="assignedtime"></a><span data-ttu-id="be332-103">AssignedTime</span><span class="sxs-lookup"><span data-stu-id="be332-103">AssignedTime</span></span>

<span data-ttu-id="be332-104">**AssignedTime**要素は、タスクが連絡先に割り当てられる時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="be332-104">The **AssignedTime** element represents the time when a task is assigned to a contact.</span></span> 
  
```xml
<AssignedTime/>
```

 <span data-ttu-id="be332-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="be332-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be332-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="be332-106">Attributes and elements</span></span>

<span data-ttu-id="be332-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="be332-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be332-108">属性</span><span class="sxs-lookup"><span data-stu-id="be332-108">Attributes</span></span>

<span data-ttu-id="be332-109">なし。</span><span class="sxs-lookup"><span data-stu-id="be332-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="be332-110">子要素</span><span class="sxs-lookup"><span data-stu-id="be332-110">Child elements</span></span>

<span data-ttu-id="be332-111">なし。</span><span class="sxs-lookup"><span data-stu-id="be332-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="be332-112">親要素</span><span class="sxs-lookup"><span data-stu-id="be332-112">Parent elements</span></span>

|<span data-ttu-id="be332-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="be332-113">**Element**</span></span>|<span data-ttu-id="be332-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="be332-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be332-115">タスク</span><span class="sxs-lookup"><span data-stu-id="be332-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="be332-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="be332-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="be332-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="be332-117">Text value</span></span>

<span data-ttu-id="be332-118">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="be332-118">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="be332-119">注釈</span><span class="sxs-lookup"><span data-stu-id="be332-119">Remarks</span></span>

<span data-ttu-id="be332-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="be332-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be332-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="be332-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be332-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="be332-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="be332-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="be332-123">Schema name</span></span>  <br/> |<span data-ttu-id="be332-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="be332-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="be332-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="be332-125">Validation file</span></span>  <br/> |<span data-ttu-id="be332-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="be332-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="be332-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="be332-127">Can be empty</span></span>  <br/> |<span data-ttu-id="be332-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="be332-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be332-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="be332-129">See also</span></span>

- [<span data-ttu-id="be332-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="be332-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

