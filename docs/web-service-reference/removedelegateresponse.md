---
title: RemoveDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegateResponse
api_type:
- schema
ms.assetid: eef56c53-d0a7-4342-9ce6-4dbb6b1a1369
description: RemoveDelegateResponse 要素には、ステータスおよび RemoveDelegate 操作要求の結果が含まれています。
ms.openlocfilehash: 45d0bcfaeb4d453f50cce8449f5cb7fdb70512a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833092"
---
# <a name="removedelegateresponse"></a><span data-ttu-id="f33a6-103">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="f33a6-103">RemoveDelegateResponse</span></span>

<span data-ttu-id="f33a6-104">**RemoveDelegateResponse**要素には、ステータスおよび[RemoveDelegate 操作](removedelegate-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f33a6-104">The **RemoveDelegateResponse** element contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span> 
  
```xml
<RemoveDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RemoveDelegateResponse>
```

 <span data-ttu-id="f33a6-105">**RemoveDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f33a6-105">**RemoveDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f33a6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f33a6-106">Attributes and elements</span></span>

<span data-ttu-id="f33a6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f33a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f33a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="f33a6-108">Attributes</span></span>

<span data-ttu-id="f33a6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f33a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f33a6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f33a6-110">Child elements</span></span>

|<span data-ttu-id="f33a6-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f33a6-111">**Element**</span></span>|<span data-ttu-id="f33a6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f33a6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f33a6-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="f33a6-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="f33a6-114">Exchange Web サービス代理人の管理要求の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f33a6-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="f33a6-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="f33a6-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f33a6-116">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="f33a6-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f33a6-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f33a6-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f33a6-118">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="f33a6-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f33a6-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f33a6-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f33a6-120">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="f33a6-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="f33a6-121">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f33a6-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f33a6-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f33a6-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f33a6-123">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="f33a6-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f33a6-124">親要素</span><span class="sxs-lookup"><span data-stu-id="f33a6-124">Parent elements</span></span>

<span data-ttu-id="f33a6-125">なし。</span><span class="sxs-lookup"><span data-stu-id="f33a6-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f33a6-126">備考</span><span class="sxs-lookup"><span data-stu-id="f33a6-126">Remarks</span></span>

<span data-ttu-id="f33a6-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f33a6-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f33a6-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="f33a6-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f33a6-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="f33a6-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f33a6-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f33a6-130">Schema Name</span></span>  <br/> |<span data-ttu-id="f33a6-131">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f33a6-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f33a6-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f33a6-132">Validation File</span></span>  <br/> |<span data-ttu-id="f33a6-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f33a6-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f33a6-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f33a6-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="f33a6-135">False</span><span class="sxs-lookup"><span data-stu-id="f33a6-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f33a6-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="f33a6-136">See also</span></span>



[<span data-ttu-id="f33a6-137">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="f33a6-137">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="f33a6-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f33a6-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

