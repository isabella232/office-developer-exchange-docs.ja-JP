---
title: Updateitemin回復可能アイテム
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c49816b1-dbb5-4716-86c7-30790e86f30e
description: UpdateItemInRecoverableItems 要素は、回復可能なアイテム内のアイテムを更新する要求を指定します。
ms.openlocfilehash: f3dae55097c613b84a80795185baad559e312b90
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459785"
---
# <a name="updateiteminrecoverableitems"></a><span data-ttu-id="4ac41-103">Updateitemin回復可能アイテム</span><span class="sxs-lookup"><span data-stu-id="4ac41-103">UpdateItemInRecoverableItems</span></span>

<span data-ttu-id="4ac41-104">**Updateiteminrecoverableitems**要素は、回復可能なアイテム内のアイテムを更新する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="4ac41-104">The **UpdateItemInRecoverableItems** element specifies a request to update an item in recoverable items.</span></span> 
  
```XML
<UpdateItemInRecoverableItems>
   <ItemId/>
   <Updates/>
   <Attachments/>
   <MakeItemImmutable/>
</UpdateItemInRecoverableItems>
```

 <span data-ttu-id="4ac41-105">**Updateitemin回復 Ableitemstype**</span><span class="sxs-lookup"><span data-stu-id="4ac41-105">**UpdateItemInRecoverableItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ac41-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4ac41-106">Attributes and elements</span></span>

<span data-ttu-id="4ac41-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4ac41-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ac41-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ac41-108">Attributes</span></span>

<span data-ttu-id="4ac41-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4ac41-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ac41-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4ac41-110">Child elements</span></span>

<span data-ttu-id="4ac41-111">[ItemId](itemid.md)  | [Updates (Item)](updates-item.md)  | [添付ファイル](attachments-ex15websvcsotherref.md)  | [Makeitemimmutable](makeitemimmutable.md)</span><span class="sxs-lookup"><span data-stu-id="4ac41-111">[ItemId](itemid.md) | [Updates (Item)](updates-item.md) | [Attachments](attachments-ex15websvcsotherref.md) | [MakeItemImmutable](makeitemimmutable.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ac41-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4ac41-112">Parent elements</span></span>

<span data-ttu-id="4ac41-113">なし。</span><span class="sxs-lookup"><span data-stu-id="4ac41-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4ac41-114">注釈</span><span class="sxs-lookup"><span data-stu-id="4ac41-114">Remarks</span></span>

<span data-ttu-id="4ac41-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4ac41-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4ac41-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4ac41-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ac41-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4ac41-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ac41-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ac41-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4ac41-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4ac41-119">Schema name</span></span>  <br/> |<span data-ttu-id="4ac41-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4ac41-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4ac41-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4ac41-121">Validation file</span></span>  <br/> |<span data-ttu-id="4ac41-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4ac41-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4ac41-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4ac41-123">Can be empty</span></span>  <br/> |<span data-ttu-id="4ac41-124">false</span><span class="sxs-lookup"><span data-stu-id="4ac41-124">false</span></span>  <br/> |
   

