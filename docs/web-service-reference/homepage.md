---
title: ホームページ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HomePage
api_type:
- schema
ms.assetid: eec2c41e-a975-42f6-8150-caf8c6e26462
description: ホームページの要素は、管理フォルダーの既定のホーム ページとなる URL を指定します。
ms.openlocfilehash: 00dafa225b5200b9feedf8790ed784305dadf03c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831838"
---
# <a name="homepage"></a><span data-ttu-id="9ad36-103">ホームページ</span><span class="sxs-lookup"><span data-stu-id="9ad36-103">HomePage</span></span>

<span data-ttu-id="9ad36-104">**ホームページ**の要素は、管理フォルダーの既定のホーム ページとなる URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ad36-104">The **HomePage** element specifies the URL that will be the default home page for the managed folder.</span></span> 
  
```xml
<HomePage/>
```

 <span data-ttu-id="9ad36-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="9ad36-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ad36-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9ad36-106">Attributes and elements</span></span>

<span data-ttu-id="9ad36-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ad36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ad36-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ad36-108">Attributes</span></span>

<span data-ttu-id="9ad36-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9ad36-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ad36-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9ad36-110">Child elements</span></span>

<span data-ttu-id="9ad36-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9ad36-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9ad36-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9ad36-112">Parent elements</span></span>

|<span data-ttu-id="9ad36-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9ad36-113">**Element**</span></span>|<span data-ttu-id="9ad36-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ad36-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ad36-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="9ad36-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="9ad36-116">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ad36-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9ad36-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9ad36-117">Text value</span></span>

<span data-ttu-id="9ad36-118">テキスト値は、URL を表す文字列値です。</span><span class="sxs-lookup"><span data-stu-id="9ad36-118">The text value is a string value that represents a URL.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9ad36-119">備考</span><span class="sxs-lookup"><span data-stu-id="9ad36-119">Remarks</span></span>

<span data-ttu-id="9ad36-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="9ad36-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ad36-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="9ad36-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ad36-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="9ad36-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ad36-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9ad36-123">Schema name</span></span>  <br/> |<span data-ttu-id="9ad36-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9ad36-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="9ad36-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9ad36-125">Validation file</span></span>  <br/> |<span data-ttu-id="9ad36-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9ad36-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ad36-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9ad36-127">Can be empty</span></span>  <br/> |<span data-ttu-id="9ad36-128">False</span><span class="sxs-lookup"><span data-stu-id="9ad36-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ad36-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9ad36-129">See also</span></span>



[<span data-ttu-id="9ad36-130">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="9ad36-130">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="9ad36-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9ad36-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="9ad36-132">管理フォルダーを追加します。</span><span class="sxs-lookup"><span data-stu-id="9ad36-132">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

