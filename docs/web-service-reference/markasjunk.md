---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: MarkAsJunk 要素は、アイテムを迷惑メールフォルダーに移動し、送信者を受信拒否リストに追加する要求を指定します。
ms.openlocfilehash: 99adc423864f3096772394ef290df20e158e457d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467082"
---
# <a name="markasjunk"></a><span data-ttu-id="a1684-103">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="a1684-103">MarkAsJunk</span></span>

<span data-ttu-id="a1684-104">**Markasjunk**要素は、アイテムを迷惑メールフォルダーに移動し、送信者を受信拒否リストに追加する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1684-104">The **MarkAsJunk** element specifies the request to move an item to the junk mail folder and to add the sender to the blocked sender list.</span></span> 
  
```XML
<MarkAsJunk IsJunk="true | false" MoveItem="true | false">
   <ItemIds/>
</MarkAsJunk>
```

 <span data-ttu-id="a1684-105">**MarkAsJunkType**</span><span class="sxs-lookup"><span data-stu-id="a1684-105">**MarkAsJunkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1684-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a1684-106">Attributes and elements</span></span>

<span data-ttu-id="a1684-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a1684-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1684-108">属性</span><span class="sxs-lookup"><span data-stu-id="a1684-108">Attributes</span></span>

|<span data-ttu-id="a1684-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="a1684-109">**Attribute**</span></span>|<span data-ttu-id="a1684-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="a1684-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a1684-111">IsJunk</span><span class="sxs-lookup"><span data-stu-id="a1684-111">IsJunk</span></span>  <br/> |<span data-ttu-id="a1684-112">**Isjunk**属性のテキスト値が**true の場合**は、電子メール送信者がブロックされた送信者の一覧に追加されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="a1684-112">A text value of **true** for the **IsJunk** attribute indicates that the email sender is added to the blocked sender list.</span></span> <span data-ttu-id="a1684-113">値が**false**の場合、電子メール送信者が既にリストに含まれている場合は、受信拒否リストから電子メール送信者が削除されることを示します。</span><span class="sxs-lookup"><span data-stu-id="a1684-113">A value of **false** indicates that the email sender is removed from the blocked sender list, if the email sender is already on the list.</span></span>  <br/> |
|<span data-ttu-id="a1684-114">MoveItem</span><span class="sxs-lookup"><span data-stu-id="a1684-114">MoveItem</span></span>  <br/> |<span data-ttu-id="a1684-115">**Moveitem**属性のテキスト値が**true の場合**は、アイテムが既定の迷惑メールフォルダーに移動されることを示します。</span><span class="sxs-lookup"><span data-stu-id="a1684-115">A text value of **true** for the **MoveItem** attribute indicates that the item is moved to the default junk mail folder.</span></span> <span data-ttu-id="a1684-116">値が**false**の場合は、アイテムが既定の迷惑メールフォルダーに移動されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="a1684-116">A value of **false** indicates that the item is not moved to the default junk mail folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a1684-117">子要素</span><span class="sxs-lookup"><span data-stu-id="a1684-117">Child elements</span></span>

[<span data-ttu-id="a1684-118">ItemIds</span><span class="sxs-lookup"><span data-stu-id="a1684-118">ItemIds</span></span>](itemids.md)
  
### <a name="parent-elements"></a><span data-ttu-id="a1684-119">親要素</span><span class="sxs-lookup"><span data-stu-id="a1684-119">Parent elements</span></span>

<span data-ttu-id="a1684-120">なし。</span><span class="sxs-lookup"><span data-stu-id="a1684-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a1684-121">注釈</span><span class="sxs-lookup"><span data-stu-id="a1684-121">Remarks</span></span>

<span data-ttu-id="a1684-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a1684-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a1684-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a1684-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1684-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a1684-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1684-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="a1684-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a1684-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a1684-126">Schema name</span></span>  <br/> |<span data-ttu-id="a1684-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a1684-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a1684-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a1684-128">Validation file</span></span>  <br/> |<span data-ttu-id="a1684-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a1684-129">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a1684-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a1684-130">Can be empty</span></span>  <br/> ||
   

