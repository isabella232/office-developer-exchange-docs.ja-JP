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
description: SharedFolderId 要素は、GetSharingFolder 操作の要求で返されます、ローカル フォルダーの識別子を共有フォルダーの識別子を表します。
ms.openlocfilehash: 6d4e541ef3cae89e413efa8cc5f1beaf651dc4dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833477"
---
# <a name="sharedfolderid"></a><span data-ttu-id="094b8-103">SharedFolderId</span><span class="sxs-lookup"><span data-stu-id="094b8-103">SharedFolderId</span></span>

<span data-ttu-id="094b8-104">**SharedFolderId**要素は、 [GetSharingFolder 操作](getsharingfolder-operation.md)の要求で返されます、ローカル フォルダーの識別子を共有フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="094b8-104">The **SharedFolderId** element represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```xml
<SharedFolderId/>
```

 <span data-ttu-id="094b8-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="094b8-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="094b8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="094b8-106">Attributes and elements</span></span>

<span data-ttu-id="094b8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="094b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="094b8-108">属性</span><span class="sxs-lookup"><span data-stu-id="094b8-108">Attributes</span></span>

<span data-ttu-id="094b8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="094b8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="094b8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="094b8-110">Child elements</span></span>

<span data-ttu-id="094b8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="094b8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="094b8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="094b8-112">Parent elements</span></span>

|<span data-ttu-id="094b8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="094b8-113">**Element**</span></span>|<span data-ttu-id="094b8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="094b8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="094b8-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="094b8-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="094b8-116">指定した共有フォルダーのローカル フォルダーの識別子を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="094b8-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="094b8-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="094b8-117">Text value</span></span>

<span data-ttu-id="094b8-118">テキスト値は、 [GetSharingFolder 操作](getsharingfolder-operation.md)の要求で返されます、ローカル フォルダーの識別子を共有フォルダーの識別子を表す文字列です。</span><span class="sxs-lookup"><span data-stu-id="094b8-118">The text value is a string that represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="094b8-119">備考</span><span class="sxs-lookup"><span data-stu-id="094b8-119">Remarks</span></span>

<span data-ttu-id="094b8-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="094b8-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="094b8-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="094b8-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="094b8-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="094b8-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="094b8-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="094b8-123">Schema Name</span></span>  <br/> |<span data-ttu-id="094b8-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="094b8-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="094b8-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="094b8-125">Validation File</span></span>  <br/> |<span data-ttu-id="094b8-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="094b8-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="094b8-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="094b8-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="094b8-128">False</span><span class="sxs-lookup"><span data-stu-id="094b8-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="094b8-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="094b8-129">See also</span></span>



[<span data-ttu-id="094b8-130">GetSharingFolder 操作</span><span class="sxs-lookup"><span data-stu-id="094b8-130">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="094b8-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="094b8-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

