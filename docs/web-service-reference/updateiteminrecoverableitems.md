---
title: UpdateItemInRecoverableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c49816b1-dbb5-4716-86c7-30790e86f30e
description: UpdateItemInRecoverableItems 要素は、回復可能な項目の項目を更新する要求を指定します。
ms.openlocfilehash: 768de4bb8abe4780ab520405bae3149b8f17637c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839861"
---
# <a name="updateiteminrecoverableitems"></a><span data-ttu-id="af8d3-103">UpdateItemInRecoverableItems</span><span class="sxs-lookup"><span data-stu-id="af8d3-103">UpdateItemInRecoverableItems</span></span>

<span data-ttu-id="af8d3-104">**UpdateItemInRecoverableItems**要素は、回復可能な項目の項目を更新する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="af8d3-104">The **UpdateItemInRecoverableItems** element specifies a request to update an item in recoverable items.</span></span> 
  
```XML
<UpdateItemInRecoverableItems>
   <ItemId/>
   <Updates/>
   <Attachments/>
   <MakeItemImmutable/>
</UpdateItemInRecoverableItems>
```

 <span data-ttu-id="af8d3-105">**UpdateItemInRecoverableItemsType**</span><span class="sxs-lookup"><span data-stu-id="af8d3-105">**UpdateItemInRecoverableItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af8d3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="af8d3-106">Attributes and elements</span></span>

<span data-ttu-id="af8d3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="af8d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af8d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="af8d3-108">Attributes</span></span>

<span data-ttu-id="af8d3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="af8d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af8d3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="af8d3-110">Child elements</span></span>

<span data-ttu-id="af8d3-111">[ItemId](itemid.md) | [(項目) の更新プログラム](updates-item.md) | [添付ファイル](attachments-ex15websvcsotherref.md) | [MakeItemImmutable](makeitemimmutable.md)</span><span class="sxs-lookup"><span data-stu-id="af8d3-111">[ItemId](itemid.md) | [Updates (Item)](updates-item.md) | [Attachments](attachments-ex15websvcsotherref.md) | [MakeItemImmutable](makeitemimmutable.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="af8d3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="af8d3-112">Parent elements</span></span>

<span data-ttu-id="af8d3-113">なし。</span><span class="sxs-lookup"><span data-stu-id="af8d3-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="af8d3-114">備考</span><span class="sxs-lookup"><span data-stu-id="af8d3-114">Remarks</span></span>

<span data-ttu-id="af8d3-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="af8d3-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="af8d3-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="af8d3-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af8d3-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="af8d3-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af8d3-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="af8d3-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="af8d3-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="af8d3-119">Schema name</span></span>  <br/> |<span data-ttu-id="af8d3-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="af8d3-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="af8d3-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="af8d3-121">Validation file</span></span>  <br/> |<span data-ttu-id="af8d3-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="af8d3-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="af8d3-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="af8d3-123">Can be empty</span></span>  <br/> |<span data-ttu-id="af8d3-124">false</span><span class="sxs-lookup"><span data-stu-id="af8d3-124">false</span></span>  <br/> |
   

