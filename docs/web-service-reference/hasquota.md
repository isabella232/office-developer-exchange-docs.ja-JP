---
title: HasQuota
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasQuota
api_type:
- schema
ms.assetid: b6e4fef0-92a9-415f-81ae-0c5ecb7c12ad
description: HasQuota 要素は、管理フォルダーにクォータがあるかどうかを示します。
ms.openlocfilehash: 6e32aa4c69943774be928339936cca5016c58d85
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462753"
---
# <a name="hasquota"></a><span data-ttu-id="26fab-103">HasQuota</span><span class="sxs-lookup"><span data-stu-id="26fab-103">HasQuota</span></span>

<span data-ttu-id="26fab-104">**Hasquota**要素は、管理フォルダーにクォータがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="26fab-104">The **HasQuota** element indicates whether the managed folder has a quota.</span></span> 
  
```xml
<HasQuota/>
```

 <span data-ttu-id="26fab-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="26fab-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26fab-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="26fab-106">Attributes and elements</span></span>

<span data-ttu-id="26fab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="26fab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26fab-108">属性</span><span class="sxs-lookup"><span data-stu-id="26fab-108">Attributes</span></span>

<span data-ttu-id="26fab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="26fab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26fab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="26fab-110">Child elements</span></span>

<span data-ttu-id="26fab-111">なし。</span><span class="sxs-lookup"><span data-stu-id="26fab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="26fab-112">親要素</span><span class="sxs-lookup"><span data-stu-id="26fab-112">Parent elements</span></span>

|<span data-ttu-id="26fab-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="26fab-113">**Element**</span></span>|<span data-ttu-id="26fab-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="26fab-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26fab-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="26fab-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="26fab-116">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="26fab-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="26fab-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="26fab-117">Text value</span></span>

<span data-ttu-id="26fab-118">テキスト値は、ブール値を表します。</span><span class="sxs-lookup"><span data-stu-id="26fab-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="26fab-119">値が**true の場合**は、フォルダーにクォータがあることを示します。値が**false**の場合は、フォルダーにクォータがないことを示します。</span><span class="sxs-lookup"><span data-stu-id="26fab-119">A value of **true** indicates that the folder has a quota; a value of **false** indicates that the folder does not have a quota.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="26fab-120">注釈</span><span class="sxs-lookup"><span data-stu-id="26fab-120">Remarks</span></span>

<span data-ttu-id="26fab-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="26fab-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26fab-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="26fab-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26fab-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="26fab-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="26fab-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="26fab-124">Schema name</span></span>  <br/> |<span data-ttu-id="26fab-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="26fab-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="26fab-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="26fab-126">Validation file</span></span>  <br/> |<span data-ttu-id="26fab-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="26fab-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="26fab-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="26fab-128">Can be empty</span></span>  <br/> |<span data-ttu-id="26fab-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="26fab-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26fab-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="26fab-130">See also</span></span>



- [<span data-ttu-id="26fab-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="26fab-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

