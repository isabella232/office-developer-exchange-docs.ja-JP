---
title: DeleteFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderResponse
api_type:
- schema
ms.assetid: 27578bda-ef0a-4a33-bccc-2c1bc1735424
description: DeleteFolderResponse 要素は、DeleteFolder 要求への応答を定義します。
ms.openlocfilehash: ca6d12c847de4cfb46c4c680558ed7b256f1ecaf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759977"
---
# <a name="deletefolderresponse"></a><span data-ttu-id="66953-103">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="66953-103">DeleteFolderResponse</span></span>

<span data-ttu-id="66953-104">**DeleteFolderResponse**要素は、DeleteFolder 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="66953-104">The **DeleteFolderResponse** element defines a response to a DeleteFolder request.</span></span> 
  
```xml
<DeleteFolderResponse>
   <ResponseMessages/>
</DeleteFolderResponse>
```

 <span data-ttu-id="66953-105">**DeleteFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="66953-105">**DeleteFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66953-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="66953-106">Attributes and elements</span></span>

<span data-ttu-id="66953-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="66953-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66953-108">属性</span><span class="sxs-lookup"><span data-stu-id="66953-108">Attributes</span></span>

<span data-ttu-id="66953-109">なし。</span><span class="sxs-lookup"><span data-stu-id="66953-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66953-110">子要素</span><span class="sxs-lookup"><span data-stu-id="66953-110">Child elements</span></span>

|<span data-ttu-id="66953-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="66953-111">**Element**</span></span>|<span data-ttu-id="66953-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="66953-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66953-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="66953-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="66953-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="66953-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="66953-115">親要素</span><span class="sxs-lookup"><span data-stu-id="66953-115">Parent elements</span></span>

<span data-ttu-id="66953-116">なし。</span><span class="sxs-lookup"><span data-stu-id="66953-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="66953-117">備考</span><span class="sxs-lookup"><span data-stu-id="66953-117">Remarks</span></span>

<span data-ttu-id="66953-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="66953-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66953-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="66953-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66953-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="66953-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="66953-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="66953-121">Schema name</span></span>  <br/> |<span data-ttu-id="66953-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="66953-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="66953-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="66953-123">Validation file</span></span>  <br/> |<span data-ttu-id="66953-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="66953-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="66953-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="66953-125">Can be empty</span></span>  <br/> |<span data-ttu-id="66953-126">False</span><span class="sxs-lookup"><span data-stu-id="66953-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66953-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="66953-127">See also</span></span>

- [<span data-ttu-id="66953-128">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="66953-128">DeleteFolder operation</span></span>](deletefolder-operation.md) 
- [<span data-ttu-id="66953-129">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="66953-129">DeleteFolder</span></span>](deletefolder.md)
- [<span data-ttu-id="66953-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="66953-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

