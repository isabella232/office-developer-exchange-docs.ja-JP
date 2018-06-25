---
title: UpdateDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegateResponse
api_type:
- schema
ms.assetid: cd336add-fbcc-4f61-9867-d4c08a60e142
description: UpdateDelegateResponse 要素には、ステータスおよび UpdateDelegate 操作要求の結果が含まれています。
ms.openlocfilehash: b90dd7d8011cf75831481b8f2b92df80d9a67d31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839822"
---
# <a name="updatedelegateresponse"></a><span data-ttu-id="32699-103">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="32699-103">UpdateDelegateResponse</span></span>

<span data-ttu-id="32699-104">**UpdateDelegateResponse**要素には、ステータスおよび[UpdateDelegate 操作](updatedelegate-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="32699-104">The **UpdateDelegateResponse** element contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span> 
  
```xml
<UpdateDelegateResponseMessage>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UpdateDelegateResponseMessage>
```

 <span data-ttu-id="32699-105">**UpdateDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="32699-105">**UpdateDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32699-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="32699-106">Attributes and elements</span></span>

<span data-ttu-id="32699-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="32699-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32699-108">属性</span><span class="sxs-lookup"><span data-stu-id="32699-108">Attributes</span></span>

<span data-ttu-id="32699-109">なし。</span><span class="sxs-lookup"><span data-stu-id="32699-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32699-110">子要素</span><span class="sxs-lookup"><span data-stu-id="32699-110">Child elements</span></span>

|<span data-ttu-id="32699-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="32699-111">**Element**</span></span>|<span data-ttu-id="32699-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="32699-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32699-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="32699-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="32699-114">Exchange Web サービス代理人の管理要求の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="32699-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="32699-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="32699-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="32699-116">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="32699-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="32699-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="32699-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="32699-118">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="32699-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="32699-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="32699-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="32699-120">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="32699-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="32699-121">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="32699-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="32699-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="32699-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="32699-123">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="32699-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="32699-124">親要素</span><span class="sxs-lookup"><span data-stu-id="32699-124">Parent elements</span></span>

<span data-ttu-id="32699-125">なし。</span><span class="sxs-lookup"><span data-stu-id="32699-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="32699-126">備考</span><span class="sxs-lookup"><span data-stu-id="32699-126">Remarks</span></span>

<span data-ttu-id="32699-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="32699-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32699-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="32699-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32699-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="32699-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="32699-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="32699-130">Schema Name</span></span>  <br/> |<span data-ttu-id="32699-131">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="32699-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="32699-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="32699-132">Validation File</span></span>  <br/> |<span data-ttu-id="32699-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="32699-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="32699-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="32699-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="32699-135">False</span><span class="sxs-lookup"><span data-stu-id="32699-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32699-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="32699-136">See also</span></span>



[<span data-ttu-id="32699-137">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="32699-137">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="32699-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="32699-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

