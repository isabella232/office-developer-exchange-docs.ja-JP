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
description: RefreshSharingFolder 要素は、指定したローカルフォルダーを更新する要求を定義します。 これは、RefreshSharingFolder 操作の基本要素です。
ms.openlocfilehash: 4454607fa2c3114cc7279fd7c30f8aee74707baa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467929"
---
# <a name="refreshsharingfolder"></a><span data-ttu-id="8b6bf-104">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="8b6bf-104">RefreshSharingFolder</span></span>

<span data-ttu-id="8b6bf-105">**Refreshsharingfolder**要素は、指定したローカルフォルダーを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="8b6bf-105">The **RefreshSharingFolder** element defines a request to refresh the specified local folder.</span></span> <span data-ttu-id="8b6bf-106">これは、 [Refreshsharingfolder 操作](refreshsharingfolder-operation.md)の基本要素です。</span><span class="sxs-lookup"><span data-stu-id="8b6bf-106">It is the base element for the [RefreshSharingFolder operation](refreshsharingfolder-operation.md).</span></span>
  
```xml
<RefreshSharingFolder>   <SharingFolderId/></RefreshSharingFolder>
```

 <span data-ttu-id="8b6bf-107">**RefreshSharingFolderType**</span><span class="sxs-lookup"><span data-stu-id="8b6bf-107">**RefreshSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b6bf-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8b6bf-108">Attributes and elements</span></span>

<span data-ttu-id="8b6bf-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8b6bf-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b6bf-110">属性</span><span class="sxs-lookup"><span data-stu-id="8b6bf-110">Attributes</span></span>

<span data-ttu-id="8b6bf-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8b6bf-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b6bf-112">子要素</span><span class="sxs-lookup"><span data-stu-id="8b6bf-112">Child elements</span></span>

|<span data-ttu-id="8b6bf-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="8b6bf-113">**Element**</span></span>|<span data-ttu-id="8b6bf-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8b6bf-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b6bf-115">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="8b6bf-115">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="8b6bf-116">共有関係のローカルフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="8b6bf-116">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8b6bf-117">親要素</span><span class="sxs-lookup"><span data-stu-id="8b6bf-117">Parent elements</span></span>

<span data-ttu-id="8b6bf-118">なし。</span><span class="sxs-lookup"><span data-stu-id="8b6bf-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8b6bf-119">注釈</span><span class="sxs-lookup"><span data-stu-id="8b6bf-119">Remarks</span></span>

<span data-ttu-id="8b6bf-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8b6bf-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b6bf-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8b6bf-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b6bf-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="8b6bf-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8b6bf-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8b6bf-123">Schema Name</span></span>  <br/> |<span data-ttu-id="8b6bf-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="8b6bf-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8b6bf-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8b6bf-125">Validation File</span></span>  <br/> |<span data-ttu-id="8b6bf-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="8b6bf-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8b6bf-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8b6bf-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="8b6bf-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="8b6bf-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b6bf-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="8b6bf-129">See also</span></span>



- [<span data-ttu-id="8b6bf-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8b6bf-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

