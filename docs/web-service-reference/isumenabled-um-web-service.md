---
title: IsUMEnabled (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: 33810bbd-837f-4a71-9ed9-cb4b8c52186d
description: IsUMEnabled 要素は、ユニファイド メッセージングのメールボックスが有効になっているかどうかを示します。
ms.openlocfilehash: 5f4d59c5497158e5afbc8bb5db4900bd129df50b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832113"
---
# <a name="isumenabled-um-web-service"></a><span data-ttu-id="38f9a-103">IsUMEnabled (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="38f9a-103">IsUMEnabled (UM web service)</span></span>

<span data-ttu-id="38f9a-104">**IsUMEnabled**要素は、ユニファイド メッセージングのメールボックスが有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="38f9a-104">The **IsUMEnabled** element indicates whether a mailbox is enabled for Unified Messaging.</span></span> 
  
```xml
<IsUMEnabled/>
```

 <span data-ttu-id="38f9a-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="38f9a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38f9a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="38f9a-106">Attributes and elements</span></span>

<span data-ttu-id="38f9a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="38f9a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38f9a-108">属性</span><span class="sxs-lookup"><span data-stu-id="38f9a-108">Attributes</span></span>

<span data-ttu-id="38f9a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="38f9a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38f9a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="38f9a-110">Child elements</span></span>

<span data-ttu-id="38f9a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="38f9a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="38f9a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="38f9a-112">Parent elements</span></span>

<span data-ttu-id="38f9a-113">なし。</span><span class="sxs-lookup"><span data-stu-id="38f9a-113">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="38f9a-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="38f9a-114">Text value</span></span>

<span data-ttu-id="38f9a-115">ブール値を表す文字列値は、この要素が含まれている場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="38f9a-115">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="38f9a-116">**True**の場合は、ユニファイド メッセージングのメールボックスが有効になっていることを示します。</span><span class="sxs-lookup"><span data-stu-id="38f9a-116">A value of **true** indicates that the mailbox is enabled for Unified Messaging.</span></span> <span data-ttu-id="38f9a-117">**False**の値は、ユニファイド メッセージングのメールボックスが有効になっていないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="38f9a-117">A value of **false** means that the mailbox is not enabled for Unified Messaging.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="38f9a-118">備考</span><span class="sxs-lookup"><span data-stu-id="38f9a-118">Remarks</span></span>

<span data-ttu-id="38f9a-119">ユニファイド メッセージングのメールボックスが有効になっているかどうかを確認するのには、 [IsUMEnabled 操作 (UM web サービス)](isumenabled-operation-um-web-service.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="38f9a-119">To determine whether a mailbox is enabled for Unified Messaging, use the [IsUMEnabled operation (UM web service)](isumenabled-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38f9a-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="38f9a-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38f9a-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="38f9a-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="38f9a-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="38f9a-122">Schema Name</span></span>  <br/> |<span data-ttu-id="38f9a-123">メッセージ</span><span class="sxs-lookup"><span data-stu-id="38f9a-123">Messages</span></span>  <br/> |
|<span data-ttu-id="38f9a-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="38f9a-124">Validation File</span></span>  <br/> |<span data-ttu-id="38f9a-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="38f9a-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="38f9a-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="38f9a-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="38f9a-127">False</span><span class="sxs-lookup"><span data-stu-id="38f9a-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38f9a-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="38f9a-128">See also</span></span>



[<span data-ttu-id="38f9a-129">IsUMEnabled 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="38f9a-129">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)


[<span data-ttu-id="38f9a-130">ユニファイド メッセージング web サービスの XML 要素の交換</span><span class="sxs-lookup"><span data-stu-id="38f9a-130">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)

