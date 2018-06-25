---
title: CopyFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolderResponse
api_type:
- schema
ms.assetid: 5bfbb4d3-e2ed-4b84-96f7-2175f1947aed
description: CopyFolderResponse 要素は、CopyFolder 要求への応答を定義します。
ms.openlocfilehash: 2f95089b9cb61e9e0047d02968d59d483fd7cdba
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759782"
---
# <a name="copyfolderresponse"></a><span data-ttu-id="01a7b-103">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="01a7b-103">CopyFolderResponse</span></span>

<span data-ttu-id="01a7b-104">**CopyFolderResponse**要素は、CopyFolder 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="01a7b-104">The **CopyFolderResponse** element defines a response to a CopyFolder request.</span></span> 
  
```xml
<CopyFolderResponse>
   <ResponseMessages/>
</CopyFolderResponse>
```

 <span data-ttu-id="01a7b-105">**CopyFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="01a7b-105">**CopyFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01a7b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="01a7b-106">Attributes and elements</span></span>

<span data-ttu-id="01a7b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="01a7b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01a7b-108">属性</span><span class="sxs-lookup"><span data-stu-id="01a7b-108">Attributes</span></span>

<span data-ttu-id="01a7b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="01a7b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01a7b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="01a7b-110">Child elements</span></span>

|<span data-ttu-id="01a7b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="01a7b-111">**Element**</span></span>|<span data-ttu-id="01a7b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="01a7b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01a7b-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="01a7b-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="01a7b-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="01a7b-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01a7b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="01a7b-115">Parent elements</span></span>

<span data-ttu-id="01a7b-116">なし。</span><span class="sxs-lookup"><span data-stu-id="01a7b-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="01a7b-117">備考</span><span class="sxs-lookup"><span data-stu-id="01a7b-117">Remarks</span></span>

<span data-ttu-id="01a7b-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="01a7b-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01a7b-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="01a7b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01a7b-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="01a7b-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="01a7b-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="01a7b-121">Schema name</span></span>  <br/> |<span data-ttu-id="01a7b-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="01a7b-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="01a7b-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="01a7b-123">Validation file</span></span>  <br/> |<span data-ttu-id="01a7b-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="01a7b-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="01a7b-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="01a7b-125">Can be empty</span></span>  <br/> |<span data-ttu-id="01a7b-126">False</span><span class="sxs-lookup"><span data-stu-id="01a7b-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01a7b-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="01a7b-127">See also</span></span>



[<span data-ttu-id="01a7b-128">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="01a7b-128">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="01a7b-129">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="01a7b-129">CopyFolder</span></span>](copyfolder.md)


- [<span data-ttu-id="01a7b-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="01a7b-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

