---
title: ServerReplyWithMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerReplyWithMessage
api_type:
- schema
ms.assetid: 113c6ff2-9592-44f0-b542-54e4d5122ccb
description: ServerReplyWithMessage 要素は、受信メッセージへの返信として送信されるテンプレートメッセージの ID を示します。
ms.openlocfilehash: faaa054018a17be3ff59b9fc385b3d846d39c3f1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461976"
---
# <a name="serverreplywithmessage"></a><span data-ttu-id="e3745-103">ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="e3745-103">ServerReplyWithMessage</span></span>

<span data-ttu-id="e3745-104">**ServerReplyWithMessage**要素は、受信メッセージへの返信として送信されるテンプレートメッセージの ID を示します。</span><span class="sxs-lookup"><span data-stu-id="e3745-104">The **ServerReplyWithMessage** element indicates the ID of the template message that is to be sent as a reply to incoming messages.</span></span> 
  
```XML
<ServerReplyWithMessage>
    <ItemId>
</ServerReplyWithMessage>
```

 <span data-ttu-id="e3745-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="e3745-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3745-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e3745-106">Attributes and elements</span></span>

<span data-ttu-id="e3745-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e3745-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3745-108">属性</span><span class="sxs-lookup"><span data-stu-id="e3745-108">Attributes</span></span>

<span data-ttu-id="e3745-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e3745-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3745-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e3745-110">Child elements</span></span>

|<span data-ttu-id="e3745-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="e3745-111">**Element**</span></span>|<span data-ttu-id="e3745-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e3745-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3745-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="e3745-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="e3745-114">Exchange ストア内のアイテムの一意識別子および変更キーを表します。</span><span class="sxs-lookup"><span data-stu-id="e3745-114">Represents the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3745-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e3745-115">Parent elements</span></span>

|<span data-ttu-id="e3745-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="e3745-116">**Element**</span></span>|<span data-ttu-id="e3745-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e3745-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3745-118">Actions</span><span class="sxs-lookup"><span data-stu-id="e3745-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="e3745-119">条件が満たされたときに、メッセージに対して実行できるアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="e3745-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e3745-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e3745-120">Text value</span></span>

<span data-ttu-id="e3745-121">なし。</span><span class="sxs-lookup"><span data-stu-id="e3745-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e3745-122">注釈</span><span class="sxs-lookup"><span data-stu-id="e3745-122">Remarks</span></span>

<span data-ttu-id="e3745-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e3745-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3745-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e3745-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3745-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="e3745-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e3745-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e3745-126">Schema Name</span></span>  <br/> |<span data-ttu-id="e3745-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="e3745-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e3745-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e3745-128">Validation File</span></span>  <br/> |<span data-ttu-id="e3745-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="e3745-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e3745-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e3745-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="e3745-131">正しい</span><span class="sxs-lookup"><span data-stu-id="e3745-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3745-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="e3745-132">See also</span></span>



- [<span data-ttu-id="e3745-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e3745-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

