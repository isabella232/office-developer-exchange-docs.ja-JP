---
title: UpdateItemInRecoverableItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96259756-322e-4c24-ac76-0cd9c32e0d6d
description: UpdateItemInRecoverableItemsResponseMessage 要素は、UpdateItemInRecoverableItems 要求への応答を指定します。
ms.openlocfilehash: 598d91a4fbd4d241b75aea4c155caca68f120b3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839868"
---
# <a name="updateiteminrecoverableitemsresponsemessage"></a><span data-ttu-id="6017b-103">UpdateItemInRecoverableItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6017b-103">UpdateItemInRecoverableItemsResponseMessage</span></span>

<span data-ttu-id="6017b-104">**UpdateItemInRecoverableItemsResponseMessage**要素は、 **UpdateItemInRecoverableItems**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="6017b-104">The **UpdateItemInRecoverableItemsResponseMessage** element specifies the response to an **UpdateItemInRecoverableItems** request.</span></span> 
  
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

 <span data-ttu-id="6017b-105">**UpdateItemInRecoverableItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6017b-105">**UpdateItemInRecoverableItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6017b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6017b-106">Attributes and elements</span></span>

<span data-ttu-id="6017b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6017b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6017b-108">属性</span><span class="sxs-lookup"><span data-stu-id="6017b-108">Attributes</span></span>

<span data-ttu-id="6017b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6017b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6017b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6017b-110">Child elements</span></span>

<span data-ttu-id="6017b-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [アイテム](items.md) | [添付ファイル](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span><span class="sxs-lookup"><span data-stu-id="6017b-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Items](items.md) | [Attachments](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6017b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6017b-112">Parent elements</span></span>

<span data-ttu-id="6017b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6017b-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6017b-114">備考</span><span class="sxs-lookup"><span data-stu-id="6017b-114">Remarks</span></span>

<span data-ttu-id="6017b-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6017b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6017b-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6017b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6017b-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="6017b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6017b-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="6017b-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|<span data-ttu-id="6017b-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6017b-119">Schema name</span></span>  <br/> |<span data-ttu-id="6017b-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6017b-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="6017b-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6017b-121">Validation file</span></span>  <br/> |<span data-ttu-id="6017b-122">Message.xsd</span><span class="sxs-lookup"><span data-stu-id="6017b-122">Message.xsd</span></span>  <br/> |
|<span data-ttu-id="6017b-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6017b-123">Can be empty</span></span>  <br/> |<span data-ttu-id="6017b-124">false</span><span class="sxs-lookup"><span data-stu-id="6017b-124">false</span></span>  <br/> |
   

