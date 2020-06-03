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
description: GetDelegateResponse 要素には、GetDelegate 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 81c5033cd67b79baa131d71ea0b866c788ae5e82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462025"
---
# <a name="getdelegateresponse"></a><span data-ttu-id="71aa7-103">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="71aa7-103">GetDelegateResponse</span></span>

<span data-ttu-id="71aa7-104">**GetDelegateResponse**要素には、 [getdelegate 操作](getdelegate-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="71aa7-104">The **GetDelegateResponse** element contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span> 
  
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

 <span data-ttu-id="71aa7-105">**GetDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="71aa7-105">**GetDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71aa7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="71aa7-106">Attributes and elements</span></span>

<span data-ttu-id="71aa7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="71aa7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71aa7-108">属性</span><span class="sxs-lookup"><span data-stu-id="71aa7-108">Attributes</span></span>

<span data-ttu-id="71aa7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="71aa7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71aa7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="71aa7-110">Child elements</span></span>

|<span data-ttu-id="71aa7-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="71aa7-111">**Element**</span></span>|<span data-ttu-id="71aa7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="71aa7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71aa7-113">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="71aa7-113">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="71aa7-114">代理人とプリンシパルの間で会議出席依頼を処理する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="71aa7-114">Defines how meeting requests are handled between the delegate and the principal.</span></span>  <br/> |
|[<span data-ttu-id="71aa7-115">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="71aa7-115">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="71aa7-116">Exchange Web サービスの委任管理要求に対する応答メッセージが保存されています。</span><span class="sxs-lookup"><span data-stu-id="71aa7-116">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="71aa7-117">MessageText</span><span class="sxs-lookup"><span data-stu-id="71aa7-117">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="71aa7-118">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="71aa7-118">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="71aa7-119">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="71aa7-119">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="71aa7-120">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="71aa7-120">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="71aa7-121">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="71aa7-121">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="71aa7-122">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="71aa7-122">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="71aa7-123">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="71aa7-123">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="71aa7-124">MessageXml</span><span class="sxs-lookup"><span data-stu-id="71aa7-124">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="71aa7-125">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="71aa7-125">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71aa7-126">親要素</span><span class="sxs-lookup"><span data-stu-id="71aa7-126">Parent elements</span></span>

<span data-ttu-id="71aa7-127">なし。</span><span class="sxs-lookup"><span data-stu-id="71aa7-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="71aa7-128">注釈</span><span class="sxs-lookup"><span data-stu-id="71aa7-128">Remarks</span></span>

<span data-ttu-id="71aa7-129">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="71aa7-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71aa7-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="71aa7-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71aa7-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="71aa7-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="71aa7-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="71aa7-132">Schema Name</span></span>  <br/> |<span data-ttu-id="71aa7-133">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="71aa7-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="71aa7-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="71aa7-134">Validation File</span></span>  <br/> |<span data-ttu-id="71aa7-135">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="71aa7-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="71aa7-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="71aa7-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="71aa7-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="71aa7-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71aa7-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="71aa7-138">See also</span></span>



[<span data-ttu-id="71aa7-139">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="71aa7-139">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="71aa7-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="71aa7-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

