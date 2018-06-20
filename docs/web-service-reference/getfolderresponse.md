---
title: GetFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolderResponse
api_type:
- schema
ms.assetid: 47abeec8-78dd-4297-8525-099174ec880d
description: GetFolderResponse 要素は、GetFolder 要求への応答を定義します。
ms.openlocfilehash: 0831224f1f649f3febf20fac2d7e987de03edcb8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760743"
---
# <a name="getfolderresponse"></a><span data-ttu-id="b48c2-103">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="b48c2-103">GetFolderResponse</span></span>

<span data-ttu-id="b48c2-104">**GetFolderResponse**要素は、GetFolder 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="b48c2-104">The **GetFolderResponse** element defines a response to a GetFolder request.</span></span> 
  
```xml
<GetFolderResponse>
   <ResponseMessages/>
</GetFolderResponse>
```

 <span data-ttu-id="b48c2-105">**GetFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="b48c2-105">**GetFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b48c2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b48c2-106">Attributes and elements</span></span>

<span data-ttu-id="b48c2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b48c2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b48c2-108">属性</span><span class="sxs-lookup"><span data-stu-id="b48c2-108">Attributes</span></span>

<span data-ttu-id="b48c2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b48c2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b48c2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b48c2-110">Child elements</span></span>

|<span data-ttu-id="b48c2-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b48c2-111">**Element**</span></span>|<span data-ttu-id="b48c2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b48c2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b48c2-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b48c2-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b48c2-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b48c2-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b48c2-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b48c2-115">Parent elements</span></span>

<span data-ttu-id="b48c2-116">なし。</span><span class="sxs-lookup"><span data-stu-id="b48c2-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b48c2-117">備考</span><span class="sxs-lookup"><span data-stu-id="b48c2-117">Remarks</span></span>

<span data-ttu-id="b48c2-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="b48c2-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b48c2-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="b48c2-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b48c2-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="b48c2-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b48c2-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b48c2-121">Schema name</span></span>  <br/> |<span data-ttu-id="b48c2-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b48c2-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b48c2-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b48c2-123">Validation file</span></span>  <br/> |<span data-ttu-id="b48c2-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b48c2-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b48c2-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b48c2-125">Can be empty</span></span>  <br/> |<span data-ttu-id="b48c2-126">False</span><span class="sxs-lookup"><span data-stu-id="b48c2-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b48c2-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="b48c2-127">See also</span></span>



[<span data-ttu-id="b48c2-128">GetFolder</span><span class="sxs-lookup"><span data-stu-id="b48c2-128">GetFolder</span></span>](getfolder.md)
  
<span data-ttu-id="b48c2-129">
  [GetFolder 操作](getfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="b48c2-129">[GetFolder operation](getfolder-operation.md)</span></span>
  
[<span data-ttu-id="b48c2-130">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b48c2-130">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)

