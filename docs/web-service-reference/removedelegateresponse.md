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
description: RemoveDelegateResponse 要素には、RemoveDelegate 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 4c7a8b81528435b72576c116bc97f611544c24d6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468937"
---
# <a name="removedelegateresponse"></a><span data-ttu-id="4a86a-103">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="4a86a-103">RemoveDelegateResponse</span></span>

<span data-ttu-id="4a86a-104">**RemoveDelegateResponse**要素には、 [removedelegate 操作](removedelegate-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4a86a-104">The **RemoveDelegateResponse** element contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span> 
  
```xml
<RemoveDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RemoveDelegateResponse>
```

 <span data-ttu-id="4a86a-105">**RemoveDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="4a86a-105">**RemoveDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a86a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4a86a-106">Attributes and elements</span></span>

<span data-ttu-id="4a86a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4a86a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a86a-108">属性</span><span class="sxs-lookup"><span data-stu-id="4a86a-108">Attributes</span></span>

<span data-ttu-id="4a86a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4a86a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a86a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4a86a-110">Child elements</span></span>

|<span data-ttu-id="4a86a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="4a86a-111">**Element**</span></span>|<span data-ttu-id="4a86a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4a86a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a86a-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="4a86a-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="4a86a-114">Exchange Web サービスの委任管理要求に対する応答メッセージが保存されています。</span><span class="sxs-lookup"><span data-stu-id="4a86a-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="4a86a-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="4a86a-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4a86a-116">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="4a86a-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4a86a-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4a86a-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4a86a-118">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="4a86a-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4a86a-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4a86a-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4a86a-120">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="4a86a-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4a86a-121">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4a86a-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4a86a-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4a86a-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4a86a-123">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="4a86a-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4a86a-124">親要素</span><span class="sxs-lookup"><span data-stu-id="4a86a-124">Parent elements</span></span>

<span data-ttu-id="4a86a-125">なし。</span><span class="sxs-lookup"><span data-stu-id="4a86a-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4a86a-126">注釈</span><span class="sxs-lookup"><span data-stu-id="4a86a-126">Remarks</span></span>

<span data-ttu-id="4a86a-127">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="4a86a-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a86a-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4a86a-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a86a-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="4a86a-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4a86a-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4a86a-130">Schema Name</span></span>  <br/> |<span data-ttu-id="4a86a-131">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4a86a-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4a86a-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4a86a-132">Validation File</span></span>  <br/> |<span data-ttu-id="4a86a-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4a86a-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4a86a-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4a86a-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a86a-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="4a86a-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a86a-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="4a86a-136">See also</span></span>



[<span data-ttu-id="4a86a-137">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="4a86a-137">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="4a86a-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4a86a-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

