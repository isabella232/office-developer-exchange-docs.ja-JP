---
title: Getmailヒント応答
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTipsResponse
api_type:
- schema
ms.assetid: fe270e34-566e-4f9e-9e73-fbf38e06436d
description: Getmailヒント Response 要素は、Getメールヒント操作の応答メッセージを表します。
ms.openlocfilehash: 2c0dcfe4e2deddcf9a6f4bb9d68d59115c171796
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458608"
---
# <a name="getmailtipsresponse"></a><span data-ttu-id="9d412-103">Getmailヒント応答</span><span class="sxs-lookup"><span data-stu-id="9d412-103">GetMailTipsResponse</span></span>

<span data-ttu-id="9d412-104">**Getmailヒント response**要素は、 [getメールヒント操作](getmailtips-operation.md)の応答メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="9d412-104">The **GetMailTipsResponse** element represents the response message for a [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<GetMailTipsResponse>
   <ResponseMessages/>
</GetMailTipsResponse>
```

 <span data-ttu-id="9d412-105">**Getmailヒント Responsemessagetype**</span><span class="sxs-lookup"><span data-stu-id="9d412-105">**GetMailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d412-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9d412-106">Attributes and elements</span></span>

<span data-ttu-id="9d412-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9d412-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d412-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d412-108">Attributes</span></span>

<span data-ttu-id="9d412-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9d412-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d412-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9d412-110">Child elements</span></span>

|<span data-ttu-id="9d412-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9d412-111">**Element**</span></span>|<span data-ttu-id="9d412-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9d412-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d412-113">ResponseMessages (Arrayofmailヒント Responsemessages)</span><span class="sxs-lookup"><span data-stu-id="9d412-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="9d412-114">メールヒント応答メッセージのリストを表します。</span><span class="sxs-lookup"><span data-stu-id="9d412-114">Represents a list of mail tips response messages.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d412-115">親要素</span><span class="sxs-lookup"><span data-stu-id="9d412-115">Parent elements</span></span>

<span data-ttu-id="9d412-116">なし。</span><span class="sxs-lookup"><span data-stu-id="9d412-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9d412-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9d412-117">Text value</span></span>

<span data-ttu-id="9d412-118">なし。</span><span class="sxs-lookup"><span data-stu-id="9d412-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9d412-119">注釈</span><span class="sxs-lookup"><span data-stu-id="9d412-119">Remarks</span></span>

<span data-ttu-id="9d412-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9d412-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d412-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9d412-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d412-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="9d412-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9d412-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9d412-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9d412-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="9d412-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9d412-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9d412-125">Validation File</span></span>  <br/> |<span data-ttu-id="9d412-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9d412-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9d412-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9d412-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d412-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="9d412-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d412-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9d412-129">See also</span></span>



[<span data-ttu-id="9d412-130">GetMailTips ヒント操作</span><span class="sxs-lookup"><span data-stu-id="9d412-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="9d412-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9d412-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

