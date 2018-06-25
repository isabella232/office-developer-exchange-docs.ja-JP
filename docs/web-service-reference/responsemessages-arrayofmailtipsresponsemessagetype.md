---
title: ResponseMessages (ArrayOfMailTipsResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 00878187-fac2-45b9-ba1c-df7ffac71089
description: ResponseMessages 要素は、メール ヒントの応答メッセージの一覧を表します。
ms.openlocfilehash: 80610af191f3fa600abe2ba8dbba2aac63f3ab1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833192"
---
# <a name="responsemessages-arrayofmailtipsresponsemessagetype"></a><span data-ttu-id="0b7d0-103">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="0b7d0-103">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>

<span data-ttu-id="0b7d0-104">**ResponseMessages**要素は、メール ヒントの応答メッセージの一覧を表します。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-104">The **ResponseMessages** element represents a list of mail tips response messages.</span></span> 
  
```XML
<ResponseMessages>
   <MailTipsResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="0b7d0-105">**ArrayOfMailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0b7d0-105">**ArrayOfMailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b7d0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0b7d0-106">Attributes and elements</span></span>

<span data-ttu-id="0b7d0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b7d0-108">属性</span><span class="sxs-lookup"><span data-stu-id="0b7d0-108">Attributes</span></span>

<span data-ttu-id="0b7d0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b7d0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0b7d0-110">Child elements</span></span>

|<span data-ttu-id="0b7d0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="0b7d0-111">**Element**</span></span>|<span data-ttu-id="0b7d0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0b7d0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b7d0-113">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="0b7d0-113">MailTipsResponseMessageType</span></span>](mailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="0b7d0-114">メールのヒントの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-114">Represents mail tips settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b7d0-115">親要素</span><span class="sxs-lookup"><span data-stu-id="0b7d0-115">Parent elements</span></span>

|<span data-ttu-id="0b7d0-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="0b7d0-116">**Element**</span></span>|<span data-ttu-id="0b7d0-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="0b7d0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b7d0-118">GetMailTipsResponse</span><span class="sxs-lookup"><span data-stu-id="0b7d0-118">GetMailTipsResponse</span></span>](getmailtipsresponse.md) <br/> |<span data-ttu-id="0b7d0-119">[GetMailTips 操作](getmailtips-operation.md)の応答メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-119">Represents the response message for the [GetMailTips operation](getmailtips-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0b7d0-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0b7d0-120">Text value</span></span>

<span data-ttu-id="0b7d0-121">なし。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0b7d0-122">備考</span><span class="sxs-lookup"><span data-stu-id="0b7d0-122">Remarks</span></span>

<span data-ttu-id="0b7d0-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b7d0-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="0b7d0-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b7d0-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="0b7d0-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0b7d0-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0b7d0-126">Schema Name</span></span>  <br/> |<span data-ttu-id="0b7d0-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="0b7d0-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0b7d0-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0b7d0-128">Validation File</span></span>  <br/> |<span data-ttu-id="0b7d0-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0b7d0-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0b7d0-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0b7d0-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b7d0-131">False</span><span class="sxs-lookup"><span data-stu-id="0b7d0-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b7d0-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="0b7d0-132">See also</span></span>



[<span data-ttu-id="0b7d0-133">GetMailTips 操作</span><span class="sxs-lookup"><span data-stu-id="0b7d0-133">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="0b7d0-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0b7d0-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

