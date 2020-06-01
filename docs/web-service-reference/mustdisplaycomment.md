---
title: On Displaycomment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MustDisplayComment
api_type:
- schema
ms.assetid: 11d4d3c3-4652-4ed4-9b29-a0b5f85b82b7
description: Displaydisplaycomment 要素は、管理フォルダーコメントを表示する必要があるかどうかを示します。
ms.openlocfilehash: e86b0c6e2c1d7c3cc00561c17c82b3be82d81242
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463210"
---
# <a name="mustdisplaycomment"></a><span data-ttu-id="acea8-103">On Displaycomment</span><span class="sxs-lookup"><span data-stu-id="acea8-103">MustDisplayComment</span></span>

<span data-ttu-id="acea8-104">**Displaydisplaycomment**要素は、管理フォルダーコメントを表示する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="acea8-104">The **MustDisplayComment** element indicates whether the managed folder comment must be displayed.</span></span> 
  
```xml
<MustDisplayComment/>
```

 <span data-ttu-id="acea8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="acea8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="acea8-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="acea8-106">Attributes and elements</span></span>

<span data-ttu-id="acea8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="acea8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="acea8-108">属性</span><span class="sxs-lookup"><span data-stu-id="acea8-108">Attributes</span></span>

<span data-ttu-id="acea8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="acea8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="acea8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="acea8-110">Child elements</span></span>

<span data-ttu-id="acea8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="acea8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="acea8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="acea8-112">Parent elements</span></span>

|<span data-ttu-id="acea8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="acea8-113">**Element**</span></span>|<span data-ttu-id="acea8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="acea8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="acea8-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="acea8-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="acea8-116">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="acea8-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="acea8-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="acea8-117">Text value</span></span>

<span data-ttu-id="acea8-118">テキスト値は、ブール値を表します。</span><span class="sxs-lookup"><span data-stu-id="acea8-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="acea8-119">値が**true の場合**は、コメントを表示する必要があることを示します。値が**false**の場合は、コメントを表示する必要がないことを示します。</span><span class="sxs-lookup"><span data-stu-id="acea8-119">A value of **true** indicates that the comment must be displayed; a value of **false** indicates that the comment does not have to be displayed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="acea8-120">注釈</span><span class="sxs-lookup"><span data-stu-id="acea8-120">Remarks</span></span>

<span data-ttu-id="acea8-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="acea8-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="acea8-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="acea8-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="acea8-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="acea8-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="acea8-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="acea8-124">Schema name</span></span>  <br/> |<span data-ttu-id="acea8-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="acea8-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="acea8-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="acea8-126">Validation file</span></span>  <br/> |<span data-ttu-id="acea8-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="acea8-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="acea8-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="acea8-128">Can be empty</span></span>  <br/> |<span data-ttu-id="acea8-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="acea8-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="acea8-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="acea8-130">See also</span></span>



[<span data-ttu-id="acea8-131">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="acea8-131">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="acea8-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="acea8-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

