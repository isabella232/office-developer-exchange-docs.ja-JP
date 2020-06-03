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
description: この要素は、最後に同期する項目が応答に含まれているかどうかを示します。
ms.openlocfilehash: bc526a38c7320609915864507f715890bedd0c9d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530051"
---
# <a name="includeslastiteminrange"></a><span data-ttu-id="6cf4b-103">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="6cf4b-103">IncludesLastItemInRange</span></span>

<span data-ttu-id="6cf4b-104">この**要素は**、最後に同期する項目が応答に含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6cf4b-104">The **IncludesLastItemInRange** element indicates whether the last item to synchronize has been included in the response.</span></span> 
  
[<span data-ttu-id="6cf4b-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="6cf4b-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="6cf4b-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6cf4b-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="6cf4b-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6cf4b-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="6cf4b-108">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="6cf4b-108">IncludesLastItemInRange</span></span>](includeslastiteminrange.md)
  
```xml
<IncludesLastItemInRange/>
```

 <span data-ttu-id="6cf4b-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6cf4b-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6cf4b-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6cf4b-110">Attributes and elements</span></span>

<span data-ttu-id="6cf4b-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6cf4b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6cf4b-112">属性</span><span class="sxs-lookup"><span data-stu-id="6cf4b-112">Attributes</span></span>

<span data-ttu-id="6cf4b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6cf4b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6cf4b-114">子要素</span><span class="sxs-lookup"><span data-stu-id="6cf4b-114">Child elements</span></span>

<span data-ttu-id="6cf4b-115">なし。</span><span class="sxs-lookup"><span data-stu-id="6cf4b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6cf4b-116">親要素</span><span class="sxs-lookup"><span data-stu-id="6cf4b-116">Parent elements</span></span>

|<span data-ttu-id="6cf4b-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="6cf4b-117">**Element**</span></span>|<span data-ttu-id="6cf4b-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cf4b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cf4b-119">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6cf4b-119">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="6cf4b-120">SyncFolderItems 要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="6cf4b-120">Contains the status and result of a SyncFolderItems request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6cf4b-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6cf4b-121">Text value</span></span>

<span data-ttu-id="6cf4b-122">ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="6cf4b-122">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6cf4b-123">注釈</span><span class="sxs-lookup"><span data-stu-id="6cf4b-123">Remarks</span></span>

<span data-ttu-id="6cf4b-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6cf4b-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6cf4b-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6cf4b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6cf4b-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="6cf4b-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6cf4b-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6cf4b-127">Schema name</span></span>  <br/> |<span data-ttu-id="6cf4b-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6cf4b-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6cf4b-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6cf4b-129">Validation file</span></span>  <br/> |<span data-ttu-id="6cf4b-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6cf4b-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6cf4b-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6cf4b-131">Can be empty</span></span>  <br/> |<span data-ttu-id="6cf4b-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="6cf4b-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6cf4b-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="6cf4b-133">See also</span></span>



[<span data-ttu-id="6cf4b-134">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="6cf4b-134">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="6cf4b-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6cf4b-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

