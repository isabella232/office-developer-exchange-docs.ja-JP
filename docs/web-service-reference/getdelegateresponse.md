---
title: GetDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegateResponse
api_type:
- schema
ms.assetid: 71a418a5-5652-40e1-8f84-fe4f7c9f86af
description: GetDelegateResponse 要素には、ステータスおよび GetDelegate 操作要求の結果が含まれています。
ms.openlocfilehash: 52731ea66420c21cf3fb8d19082aef65551c2af2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760686"
---
# <a name="getdelegateresponse"></a><span data-ttu-id="e24c4-103">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="e24c4-103">GetDelegateResponse</span></span>

<span data-ttu-id="e24c4-104">**GetDelegateResponse**要素には、ステータスおよび[GetDelegate 操作](getdelegate-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e24c4-104">The **GetDelegateResponse** element contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span> 
  
```xml
<GetDelegateResponse>
   <DeliverMeetingRequests/>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</GetDelegateResponse>
```

 <span data-ttu-id="e24c4-105">**GetDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e24c4-105">**GetDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e24c4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e24c4-106">Attributes and elements</span></span>

<span data-ttu-id="e24c4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e24c4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e24c4-108">属性</span><span class="sxs-lookup"><span data-stu-id="e24c4-108">Attributes</span></span>

<span data-ttu-id="e24c4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e24c4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e24c4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e24c4-110">Child elements</span></span>

|<span data-ttu-id="e24c4-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e24c4-111">**Element**</span></span>|<span data-ttu-id="e24c4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e24c4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e24c4-113">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="e24c4-113">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="e24c4-114">主体と代理人の間で会議出席依頼を処理する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="e24c4-114">Defines how meeting requests are handled between the delegate and the principal.</span></span>  <br/> |
|[<span data-ttu-id="e24c4-115">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="e24c4-115">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="e24c4-116">Exchange Web サービス代理人の管理要求の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e24c4-116">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="e24c4-117">MessageText</span><span class="sxs-lookup"><span data-stu-id="e24c4-117">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e24c4-118">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="e24c4-118">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e24c4-119">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e24c4-119">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e24c4-120">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="e24c4-120">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="e24c4-121">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e24c4-121">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e24c4-122">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="e24c4-122">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="e24c4-123">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e24c4-123">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e24c4-124">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e24c4-124">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e24c4-125">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="e24c4-125">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e24c4-126">親要素</span><span class="sxs-lookup"><span data-stu-id="e24c4-126">Parent elements</span></span>

<span data-ttu-id="e24c4-127">なし。</span><span class="sxs-lookup"><span data-stu-id="e24c4-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e24c4-128">備考</span><span class="sxs-lookup"><span data-stu-id="e24c4-128">Remarks</span></span>

<span data-ttu-id="e24c4-129">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e24c4-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e24c4-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="e24c4-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e24c4-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="e24c4-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e24c4-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e24c4-132">Schema Name</span></span>  <br/> |<span data-ttu-id="e24c4-133">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e24c4-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e24c4-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e24c4-134">Validation File</span></span>  <br/> |<span data-ttu-id="e24c4-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e24c4-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e24c4-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e24c4-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="e24c4-137">False</span><span class="sxs-lookup"><span data-stu-id="e24c4-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e24c4-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="e24c4-138">See also</span></span>



[<span data-ttu-id="e24c4-139">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="e24c4-139">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="e24c4-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e24c4-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

