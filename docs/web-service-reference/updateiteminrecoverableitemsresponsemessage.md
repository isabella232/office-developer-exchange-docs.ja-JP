---
title: UpdateItemInRecoverableItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96259756-322e-4c24-ac76-0cd9c32e0d6d
description: UpdateItemInRecoverableItemsResponseMessage 要素は、Updateitemin Ableitems 要求への応答を指定します。
ms.openlocfilehash: 021631f5c30eebbf4d7ae0aad35a85b99a23925f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466536"
---
# <a name="updateiteminrecoverableitemsresponsemessage"></a><span data-ttu-id="9b5cc-103">UpdateItemInRecoverableItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9b5cc-103">UpdateItemInRecoverableItemsResponseMessage</span></span>

<span data-ttu-id="9b5cc-104">**UpdateItemInRecoverableItemsResponseMessage**要素は、 **Updateitemin ableitems**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b5cc-104">The **UpdateItemInRecoverableItemsResponseMessage** element specifies the response to an **UpdateItemInRecoverableItems** request.</span></span> 
  
```XML
<UpdateItemInRecoverableItemsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKet/>
   <MessageXml/>
   <Items/>
   <Attachments/>
   <ConflictResults/>
</UpdateItemInRecoverableItemsResponseMessage>
```

 <span data-ttu-id="9b5cc-105">**Updateitemin回復 Ableitemsresponsemessagetype**</span><span class="sxs-lookup"><span data-stu-id="9b5cc-105">**UpdateItemInRecoverableItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b5cc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9b5cc-106">Attributes and elements</span></span>

<span data-ttu-id="9b5cc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9b5cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b5cc-108">属性</span><span class="sxs-lookup"><span data-stu-id="9b5cc-108">Attributes</span></span>

<span data-ttu-id="9b5cc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9b5cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b5cc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9b5cc-110">Child elements</span></span>

<span data-ttu-id="9b5cc-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [アイテム](items.md)  | [添付ファイル](attachments-ex15websvcsotherref.md)  | [ConflictResults](conflictresults.md)</span><span class="sxs-lookup"><span data-stu-id="9b5cc-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Items](items.md) | [Attachments](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9b5cc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9b5cc-112">Parent elements</span></span>

<span data-ttu-id="9b5cc-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9b5cc-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9b5cc-114">注釈</span><span class="sxs-lookup"><span data-stu-id="9b5cc-114">Remarks</span></span>

<span data-ttu-id="9b5cc-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9b5cc-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9b5cc-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9b5cc-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b5cc-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9b5cc-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b5cc-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="9b5cc-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|<span data-ttu-id="9b5cc-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9b5cc-119">Schema name</span></span>  <br/> |<span data-ttu-id="9b5cc-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="9b5cc-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="9b5cc-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9b5cc-121">Validation file</span></span>  <br/> |<span data-ttu-id="9b5cc-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9b5cc-122">Message.xsd</span></span>  <br/> |
|<span data-ttu-id="9b5cc-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9b5cc-123">Can be empty</span></span>  <br/> |<span data-ttu-id="9b5cc-124">false</span><span class="sxs-lookup"><span data-stu-id="9b5cc-124">false</span></span>  <br/> |
   

