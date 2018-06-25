---
title: AddDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegateResponse
api_type:
- schema
ms.assetid: d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429
description: AddDelegateResponse 要素には、ステータスおよび AddDelegate 操作要求の結果が含まれています。
ms.openlocfilehash: a1d56e9994b3a7916fe0fbe40be1e6d8ff473730
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759276"
---
# <a name="adddelegateresponse"></a><span data-ttu-id="5d7af-103">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="5d7af-103">AddDelegateResponse</span></span>

<span data-ttu-id="5d7af-104">**AddDelegateResponse**要素には、ステータスおよび[AddDelegate 操作](adddelegate-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5d7af-104">The **AddDelegateResponse** element contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span> 
  
```xml
<AddDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</AddDelegateResponse>
```

 <span data-ttu-id="5d7af-105">**AddDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5d7af-105">**AddDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d7af-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5d7af-106">Attributes and elements</span></span>

<span data-ttu-id="5d7af-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5d7af-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d7af-108">属性</span><span class="sxs-lookup"><span data-stu-id="5d7af-108">Attributes</span></span>

<span data-ttu-id="5d7af-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5d7af-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d7af-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5d7af-110">Child elements</span></span>

|<span data-ttu-id="5d7af-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="5d7af-111">**Element**</span></span>|<span data-ttu-id="5d7af-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5d7af-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d7af-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="5d7af-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="5d7af-114">Exchange Web サービス代理人の管理要求の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5d7af-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="5d7af-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="5d7af-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="5d7af-116">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="5d7af-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="5d7af-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5d7af-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="5d7af-118">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="5d7af-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="5d7af-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5d7af-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="5d7af-120">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="5d7af-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="5d7af-121">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5d7af-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="5d7af-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5d7af-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="5d7af-123">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="5d7af-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5d7af-124">親要素</span><span class="sxs-lookup"><span data-stu-id="5d7af-124">Parent elements</span></span>

<span data-ttu-id="5d7af-125">なし。</span><span class="sxs-lookup"><span data-stu-id="5d7af-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5d7af-126">備考</span><span class="sxs-lookup"><span data-stu-id="5d7af-126">Remarks</span></span>

<span data-ttu-id="5d7af-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5d7af-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d7af-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="5d7af-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d7af-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="5d7af-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5d7af-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5d7af-130">Schema Name</span></span>  <br/> |<span data-ttu-id="5d7af-131">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="5d7af-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5d7af-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5d7af-132">Validation File</span></span>  <br/> |<span data-ttu-id="5d7af-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5d7af-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5d7af-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5d7af-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d7af-135">False</span><span class="sxs-lookup"><span data-stu-id="5d7af-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d7af-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="5d7af-136">See also</span></span>

- [<span data-ttu-id="5d7af-137">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="5d7af-137">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="5d7af-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5d7af-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="5d7af-139">デリゲートを追加します。</span><span class="sxs-lookup"><span data-stu-id="5d7af-139">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

