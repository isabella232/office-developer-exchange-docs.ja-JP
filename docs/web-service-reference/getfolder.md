---
title: GetFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolder
api_type:
- schema
ms.assetid: 34e4c9ea-adcd-46bd-ae8f-7abb256c585a
description: GetFolder 要素は、Exchange ストア内のメールボックスからフォルダーを取得する要求を定義します。
ms.openlocfilehash: 41d2b1ab5fcd5d2d60c399e8070ca957ee4b66e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458706"
---
# <a name="getfolder"></a><span data-ttu-id="63fc6-103">GetFolder</span><span class="sxs-lookup"><span data-stu-id="63fc6-103">GetFolder</span></span>

<span data-ttu-id="63fc6-104">**Getfolder**要素は、Exchange ストア内のメールボックスからフォルダーを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="63fc6-104">The **GetFolder** element defines a request to get a folder from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetFolder>
   <FolderShape/>
   <FolderIds/>
</GetFolder>
```

 <span data-ttu-id="63fc6-105">**GetFolderType**</span><span class="sxs-lookup"><span data-stu-id="63fc6-105">**GetFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63fc6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="63fc6-106">Attributes and elements</span></span>

<span data-ttu-id="63fc6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="63fc6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63fc6-108">属性</span><span class="sxs-lookup"><span data-stu-id="63fc6-108">Attributes</span></span>

<span data-ttu-id="63fc6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="63fc6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63fc6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="63fc6-110">Child elements</span></span>

|<span data-ttu-id="63fc6-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="63fc6-111">**Element**</span></span>|<span data-ttu-id="63fc6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="63fc6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63fc6-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="63fc6-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="63fc6-114">[FolderIds](folderids.md)要素で識別された各フォルダーで取得するプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="63fc6-114">Identifies the properties to get for each folder identified in the [FolderIds](folderids.md) element.</span></span>  <br/> |
|[<span data-ttu-id="63fc6-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="63fc6-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="63fc6-116">Exchange ストア内のメールボックスから取得するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="63fc6-116">Contains an array of folder identifiers that are used to identify folders to get from a mailbox in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="63fc6-117">親要素</span><span class="sxs-lookup"><span data-stu-id="63fc6-117">Parent elements</span></span>

<span data-ttu-id="63fc6-118">なし。</span><span class="sxs-lookup"><span data-stu-id="63fc6-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="63fc6-119">注釈</span><span class="sxs-lookup"><span data-stu-id="63fc6-119">Remarks</span></span>

<span data-ttu-id="63fc6-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="63fc6-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63fc6-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="63fc6-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63fc6-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="63fc6-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="63fc6-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="63fc6-123">Schema Name</span></span>  <br/> |<span data-ttu-id="63fc6-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="63fc6-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="63fc6-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="63fc6-125">Validation File</span></span>  <br/> |<span data-ttu-id="63fc6-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="63fc6-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="63fc6-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="63fc6-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="63fc6-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="63fc6-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63fc6-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="63fc6-129">See also</span></span>



[<span data-ttu-id="63fc6-130">GetFolder 操作</span><span class="sxs-lookup"><span data-stu-id="63fc6-130">GetFolder operation</span></span>](getfolder-operation.md)

