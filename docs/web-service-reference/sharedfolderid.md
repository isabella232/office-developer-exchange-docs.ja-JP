---
title: SharedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharedFolderId
api_type:
- schema
ms.assetid: 21181ba3-9626-4284-9717-0b1c16948e8f
description: SharedFolderId 要素は、GetSharingFolder 操作要求によって返される必要のあるローカルフォルダー識別子である、共有フォルダーの識別子を表します。
ms.openlocfilehash: 546e148540708725bcf335f39bf69d193124d210
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466123"
---
# <a name="sharedfolderid"></a><span data-ttu-id="c876d-103">SharedFolderId</span><span class="sxs-lookup"><span data-stu-id="c876d-103">SharedFolderId</span></span>

<span data-ttu-id="c876d-104">**SharedFolderId**要素は、 [getsharingfolder 操作](getsharingfolder-operation.md)要求によって返される必要のあるローカルフォルダー識別子である、共有フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="c876d-104">The **SharedFolderId** element represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```xml
<SharedFolderId/>
```

 <span data-ttu-id="c876d-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="c876d-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c876d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c876d-106">Attributes and elements</span></span>

<span data-ttu-id="c876d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c876d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c876d-108">属性</span><span class="sxs-lookup"><span data-stu-id="c876d-108">Attributes</span></span>

<span data-ttu-id="c876d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c876d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c876d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c876d-110">Child elements</span></span>

<span data-ttu-id="c876d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c876d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c876d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c876d-112">Parent elements</span></span>

|<span data-ttu-id="c876d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c876d-113">**Element**</span></span>|<span data-ttu-id="c876d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c876d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c876d-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="c876d-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="c876d-116">指定された共有フォルダーのローカルフォルダー識別子を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="c876d-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c876d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c876d-117">Text value</span></span>

<span data-ttu-id="c876d-118">テキスト値は、 [Getsharingfolder 操作](getsharingfolder-operation.md)要求によって返されるローカルフォルダー識別子である、共有フォルダーの識別子を表す文字列です。</span><span class="sxs-lookup"><span data-stu-id="c876d-118">The text value is a string that represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c876d-119">注釈</span><span class="sxs-lookup"><span data-stu-id="c876d-119">Remarks</span></span>

<span data-ttu-id="c876d-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c876d-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c876d-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c876d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c876d-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="c876d-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c876d-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c876d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="c876d-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c876d-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c876d-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c876d-125">Validation File</span></span>  <br/> |<span data-ttu-id="c876d-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c876d-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c876d-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c876d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="c876d-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="c876d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c876d-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="c876d-129">See also</span></span>



[<span data-ttu-id="c876d-130">GetSharingFolder 操作</span><span class="sxs-lookup"><span data-stu-id="c876d-130">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="c876d-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c876d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

