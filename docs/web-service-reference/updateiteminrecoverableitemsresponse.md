---
title: Updateitemin回復 Ableitemsresponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2f61b038-eba0-40fc-8af2-c3db5cc5a420
description: Updateitemin/Ableableitemsresponse 要素は、Updateitemin回復可能なアイテムの要求への応答を指定します。
ms.openlocfilehash: 02e030774949e895bc89579cb9364d08c7844ce3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466557"
---
# <a name="updateiteminrecoverableitemsresponse"></a><span data-ttu-id="d0892-103">Updateitemin回復 Ableitemsresponse</span><span class="sxs-lookup"><span data-stu-id="d0892-103">UpdateItemInRecoverableItemsResponse</span></span>

<span data-ttu-id="d0892-104">**Updateitemin/Ableableitemsresponse**要素は、 **updateitemin回復**可能なアイテムの要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0892-104">The **UpdateItemInRecoverableItemsResponse** element specifies the response to an **UpdateItemInRecoverableItems** request.</span></span> 
  
```XML
<UpdateItemInRecoverableItemsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
   <Attachments/>
   <ConflictResults/>
</UpdateItemInRecoverableItemsResponse>
```

 <span data-ttu-id="d0892-105">**Updateitemin回復 Ableitemsresponsemessagetype**</span><span class="sxs-lookup"><span data-stu-id="d0892-105">**UpdateItemInRecoverableItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0892-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d0892-106">Attributes and elements</span></span>

<span data-ttu-id="d0892-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d0892-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0892-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0892-108">Attributes</span></span>

<span data-ttu-id="d0892-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d0892-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0892-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d0892-110">Child elements</span></span>

<span data-ttu-id="d0892-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [アイテム](items.md)  | [添付ファイル](attachments-ex15websvcsotherref.md)  | [ConflictResults](conflictresults.md)</span><span class="sxs-lookup"><span data-stu-id="d0892-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Items](items.md) | [Attachments](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d0892-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d0892-112">Parent elements</span></span>

<span data-ttu-id="d0892-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d0892-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d0892-114">注釈</span><span class="sxs-lookup"><span data-stu-id="d0892-114">Remarks</span></span>

<span data-ttu-id="d0892-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d0892-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d0892-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d0892-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0892-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d0892-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0892-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="d0892-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d0892-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d0892-119">Schema name</span></span>  <br/> |<span data-ttu-id="d0892-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d0892-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d0892-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d0892-121">Validation file</span></span>  <br/> |<span data-ttu-id="d0892-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d0892-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d0892-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d0892-123">Can be empty</span></span>  <br/> |<span data-ttu-id="d0892-124">false</span><span class="sxs-lookup"><span data-stu-id="d0892-124">false</span></span>  <br/> |
   

