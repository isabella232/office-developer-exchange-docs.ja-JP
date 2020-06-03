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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458608"
---
# <a name="getmailtipsresponse"></a><span data-ttu-id="90113-103">Getmailヒント応答</span><span class="sxs-lookup"><span data-stu-id="90113-103">GetMailTipsResponse</span></span>

<span data-ttu-id="90113-104">**Getmailヒント response**要素は、 [getメールヒント操作](getmailtips-operation.md)の応答メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="90113-104">The **GetMailTipsResponse** element represents the response message for a [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<GetMailTipsResponse>
   <ResponseMessages/>
</GetMailTipsResponse>
```

 <span data-ttu-id="90113-105">**Getmailヒント Responsemessagetype**</span><span class="sxs-lookup"><span data-stu-id="90113-105">**GetMailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90113-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="90113-106">Attributes and elements</span></span>

<span data-ttu-id="90113-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="90113-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90113-108">属性</span><span class="sxs-lookup"><span data-stu-id="90113-108">Attributes</span></span>

<span data-ttu-id="90113-109">なし。</span><span class="sxs-lookup"><span data-stu-id="90113-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90113-110">子要素</span><span class="sxs-lookup"><span data-stu-id="90113-110">Child elements</span></span>

|<span data-ttu-id="90113-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="90113-111">**Element**</span></span>|<span data-ttu-id="90113-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="90113-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90113-113">ResponseMessages (Arrayofmailヒント Responsemessages)</span><span class="sxs-lookup"><span data-stu-id="90113-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="90113-114">メールヒント応答メッセージのリストを表します。</span><span class="sxs-lookup"><span data-stu-id="90113-114">Represents a list of mail tips response messages.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90113-115">親要素</span><span class="sxs-lookup"><span data-stu-id="90113-115">Parent elements</span></span>

<span data-ttu-id="90113-116">なし。</span><span class="sxs-lookup"><span data-stu-id="90113-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="90113-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="90113-117">Text value</span></span>

<span data-ttu-id="90113-118">なし。</span><span class="sxs-lookup"><span data-stu-id="90113-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="90113-119">注釈</span><span class="sxs-lookup"><span data-stu-id="90113-119">Remarks</span></span>

<span data-ttu-id="90113-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="90113-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90113-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="90113-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90113-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="90113-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="90113-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="90113-123">Schema Name</span></span>  <br/> |<span data-ttu-id="90113-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="90113-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="90113-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="90113-125">Validation File</span></span>  <br/> |<span data-ttu-id="90113-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="90113-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="90113-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="90113-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="90113-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="90113-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90113-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="90113-129">See also</span></span>



[<span data-ttu-id="90113-130">GetMailTips ヒント操作</span><span class="sxs-lookup"><span data-stu-id="90113-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="90113-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="90113-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

