---
title: IncludesLastItemInRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IncludesLastItemInRange
api_type:
- schema
ms.assetid: e7d6c7d3-548e-48b0-a313-bfef81e4832a
description: IncludesLastItemInRange 要素は、最後の項目を同期するが、応答に含まれているかどうかを示します。
ms.openlocfilehash: b4786c5aa81e9b4fee98e7ed4238215ff327443e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831906"
---
# <a name="includeslastiteminrange"></a><span data-ttu-id="31a08-103">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="31a08-103">IncludesLastItemInRange</span></span>

<span data-ttu-id="31a08-104">**IncludesLastItemInRange**要素は、最後の項目を同期するが、応答に含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="31a08-104">The **IncludesLastItemInRange** element indicates whether the last item to synchronize has been included in the response.</span></span> 
  
[<span data-ttu-id="31a08-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="31a08-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="31a08-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="31a08-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="31a08-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="31a08-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="31a08-108">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="31a08-108">IncludesLastItemInRange</span></span>](includeslastiteminrange.md)
  
```xml
<IncludesLastItemInRange/>
```

 <span data-ttu-id="31a08-109">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="31a08-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31a08-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="31a08-110">Attributes and elements</span></span>

<span data-ttu-id="31a08-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="31a08-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31a08-112">属性</span><span class="sxs-lookup"><span data-stu-id="31a08-112">Attributes</span></span>

<span data-ttu-id="31a08-113">なし。</span><span class="sxs-lookup"><span data-stu-id="31a08-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31a08-114">子要素</span><span class="sxs-lookup"><span data-stu-id="31a08-114">Child elements</span></span>

<span data-ttu-id="31a08-115">なし。</span><span class="sxs-lookup"><span data-stu-id="31a08-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="31a08-116">親要素</span><span class="sxs-lookup"><span data-stu-id="31a08-116">Parent elements</span></span>

|<span data-ttu-id="31a08-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="31a08-117">**Element**</span></span>|<span data-ttu-id="31a08-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="31a08-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31a08-119">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="31a08-119">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="31a08-120">SyncFolderItems 要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="31a08-120">Contains the status and result of a SyncFolderItems request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="31a08-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="31a08-121">Text value</span></span>

<span data-ttu-id="31a08-122">ブール値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="31a08-122">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="31a08-123">備考</span><span class="sxs-lookup"><span data-stu-id="31a08-123">Remarks</span></span>

<span data-ttu-id="31a08-124">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="31a08-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31a08-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="31a08-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31a08-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="31a08-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="31a08-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="31a08-127">Schema name</span></span>  <br/> |<span data-ttu-id="31a08-128">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="31a08-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="31a08-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="31a08-129">Validation file</span></span>  <br/> |<span data-ttu-id="31a08-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="31a08-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="31a08-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="31a08-131">Can be empty</span></span>  <br/> |<span data-ttu-id="31a08-132">False</span><span class="sxs-lookup"><span data-stu-id="31a08-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31a08-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="31a08-133">See also</span></span>



[<span data-ttu-id="31a08-134">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="31a08-134">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="31a08-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="31a08-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

