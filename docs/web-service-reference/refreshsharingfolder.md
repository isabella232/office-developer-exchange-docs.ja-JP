---
title: RefreshSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolder
api_type:
- schema
ms.assetid: 14571c28-effa-430a-802e-82fb99bafa7f
description: RefreshSharingFolder 要素は、指定したローカル フォルダーを更新する要求を定義します。 それは、RefreshSharingFolder 操作の基本要素です。
ms.openlocfilehash: b09e311d0ba38b0cdcc9fe0864ed3e2b0151b0fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833043"
---
# <a name="refreshsharingfolder"></a><span data-ttu-id="21607-104">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="21607-104">RefreshSharingFolder</span></span>

<span data-ttu-id="21607-105">**RefreshSharingFolder**要素は、指定したローカル フォルダーを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="21607-105">The **RefreshSharingFolder** element defines a request to refresh the specified local folder.</span></span> <span data-ttu-id="21607-106">それは、 [RefreshSharingFolder 操作](refreshsharingfolder-operation.md)の基本要素です。</span><span class="sxs-lookup"><span data-stu-id="21607-106">It is the base element for the [RefreshSharingFolder operation](refreshsharingfolder-operation.md).</span></span>
  
```xml
<RefreshSharingFolder>   <SharingFolderId/></RefreshSharingFolder>
```

 <span data-ttu-id="21607-107">**RefreshSharingFolderType**</span><span class="sxs-lookup"><span data-stu-id="21607-107">**RefreshSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21607-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="21607-108">Attributes and elements</span></span>

<span data-ttu-id="21607-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="21607-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21607-110">属性</span><span class="sxs-lookup"><span data-stu-id="21607-110">Attributes</span></span>

<span data-ttu-id="21607-111">なし。</span><span class="sxs-lookup"><span data-stu-id="21607-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21607-112">子要素</span><span class="sxs-lookup"><span data-stu-id="21607-112">Child elements</span></span>

|<span data-ttu-id="21607-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="21607-113">**Element**</span></span>|<span data-ttu-id="21607-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="21607-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21607-115">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="21607-115">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="21607-116">共有関係では、ローカル フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="21607-116">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21607-117">親要素</span><span class="sxs-lookup"><span data-stu-id="21607-117">Parent elements</span></span>

<span data-ttu-id="21607-118">なし。</span><span class="sxs-lookup"><span data-stu-id="21607-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="21607-119">備考</span><span class="sxs-lookup"><span data-stu-id="21607-119">Remarks</span></span>

<span data-ttu-id="21607-120">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="21607-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21607-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="21607-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21607-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="21607-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="21607-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="21607-123">Schema Name</span></span>  <br/> |<span data-ttu-id="21607-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="21607-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="21607-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="21607-125">Validation File</span></span>  <br/> |<span data-ttu-id="21607-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="21607-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="21607-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="21607-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="21607-128">False</span><span class="sxs-lookup"><span data-stu-id="21607-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21607-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="21607-129">See also</span></span>



- [<span data-ttu-id="21607-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="21607-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

