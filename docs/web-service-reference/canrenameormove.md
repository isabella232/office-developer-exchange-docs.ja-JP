---
title: CanRenameOrMove
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanRenameOrMove
api_type:
- schema
ms.assetid: fe0cdb04-5f2b-4f1d-9d12-7ace0883cd86
description: CanRenameOrMove 要素は、管理フォルダーの名前を変更するか、または顧客によって移動できるかどうかを示します。
ms.openlocfilehash: eb6aaeb8b0edcab5b67212c426a44daf32a0cf73
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463364"
---
# <a name="canrenameormove"></a><span data-ttu-id="19068-103">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="19068-103">CanRenameOrMove</span></span>

<span data-ttu-id="19068-104">**Canrenameormove**要素は、管理フォルダーの名前を変更するか、または顧客によって移動できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="19068-104">The **CanRenameOrMove** element indicates whether a managed folder can be renamed or moved by the customer.</span></span> 
  
```xml
<CanRenameOrMove/>
```

 <span data-ttu-id="19068-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="19068-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19068-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="19068-106">Attributes and elements</span></span>

<span data-ttu-id="19068-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="19068-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19068-108">属性</span><span class="sxs-lookup"><span data-stu-id="19068-108">Attributes</span></span>

<span data-ttu-id="19068-109">なし。</span><span class="sxs-lookup"><span data-stu-id="19068-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19068-110">子要素</span><span class="sxs-lookup"><span data-stu-id="19068-110">Child elements</span></span>

<span data-ttu-id="19068-111">なし。</span><span class="sxs-lookup"><span data-stu-id="19068-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19068-112">親要素</span><span class="sxs-lookup"><span data-stu-id="19068-112">Parent elements</span></span>

|<span data-ttu-id="19068-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="19068-113">**Element**</span></span>|<span data-ttu-id="19068-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="19068-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19068-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="19068-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="19068-116">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="19068-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="19068-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="19068-117">Text value</span></span>

<span data-ttu-id="19068-118">テキスト値は、ブール値を表します。</span><span class="sxs-lookup"><span data-stu-id="19068-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="19068-119">値が**true の場合**は、フォルダーの名前を変更するか、移動することができます。値が**false**の場合、フォルダーの名前を変更または移動することはできません。</span><span class="sxs-lookup"><span data-stu-id="19068-119">A value of **true** indicates that the folder can be renamed or moved; a value of **false** indicates that the folder cannot be renamed or moved.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="19068-120">注釈</span><span class="sxs-lookup"><span data-stu-id="19068-120">Remarks</span></span>

<span data-ttu-id="19068-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="19068-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19068-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="19068-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19068-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="19068-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19068-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="19068-124">Schema name</span></span>  <br/> |<span data-ttu-id="19068-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="19068-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="19068-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="19068-126">Validation file</span></span>  <br/> |<span data-ttu-id="19068-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="19068-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="19068-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="19068-128">Can be empty</span></span>  <br/> |<span data-ttu-id="19068-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="19068-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19068-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="19068-130">See also</span></span>



- [<span data-ttu-id="19068-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="19068-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

