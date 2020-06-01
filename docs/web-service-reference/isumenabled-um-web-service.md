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
description: IsUMEnabled 要素は、メールボックスがユニファイドメッセージングに対して有効になっているかどうかを示します。
ms.openlocfilehash: ea5bde677c62664acad8afd5c8142e96d82b7a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458230"
---
# <a name="isumenabled-um-web-service"></a><span data-ttu-id="fd9b6-103">IsUMEnabled (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="fd9b6-103">IsUMEnabled (UM web service)</span></span>

<span data-ttu-id="fd9b6-104">**IsUMEnabled**要素は、メールボックスがユニファイドメッセージングに対して有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fd9b6-104">The **IsUMEnabled** element indicates whether a mailbox is enabled for Unified Messaging.</span></span> 
  
```xml
<IsUMEnabled/>
```

 <span data-ttu-id="fd9b6-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="fd9b6-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd9b6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fd9b6-106">Attributes and elements</span></span>

<span data-ttu-id="fd9b6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fd9b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd9b6-108">属性</span><span class="sxs-lookup"><span data-stu-id="fd9b6-108">Attributes</span></span>

<span data-ttu-id="fd9b6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fd9b6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd9b6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fd9b6-110">Child elements</span></span>

<span data-ttu-id="fd9b6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fd9b6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd9b6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fd9b6-112">Parent elements</span></span>

<span data-ttu-id="fd9b6-113">なし。</span><span class="sxs-lookup"><span data-stu-id="fd9b6-113">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="fd9b6-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fd9b6-114">Text value</span></span>

<span data-ttu-id="fd9b6-115">この要素が含まれている場合は、ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="fd9b6-115">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="fd9b6-116">値が**true**の場合は、メールボックスがユニファイドメッセージングに対して有効になっていることを示します。</span><span class="sxs-lookup"><span data-stu-id="fd9b6-116">A value of **true** indicates that the mailbox is enabled for Unified Messaging.</span></span> <span data-ttu-id="fd9b6-117">値が**false**の場合は、メールボックスがユニファイドメッセージングに対して有効になっていないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="fd9b6-117">A value of **false** means that the mailbox is not enabled for Unified Messaging.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fd9b6-118">注釈</span><span class="sxs-lookup"><span data-stu-id="fd9b6-118">Remarks</span></span>

<span data-ttu-id="fd9b6-119">メールボックスがユニファイドメッセージングに対して有効になっているかどうかを確認するには、 [IsUMEnabled 操作 (UM web サービス)](isumenabled-operation-um-web-service.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="fd9b6-119">To determine whether a mailbox is enabled for Unified Messaging, use the [IsUMEnabled operation (UM web service)](isumenabled-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd9b6-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fd9b6-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd9b6-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="fd9b6-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fd9b6-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fd9b6-122">Schema Name</span></span>  <br/> |<span data-ttu-id="fd9b6-123">メッセージ</span><span class="sxs-lookup"><span data-stu-id="fd9b6-123">Messages</span></span>  <br/> |
|<span data-ttu-id="fd9b6-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fd9b6-124">Validation File</span></span>  <br/> |<span data-ttu-id="fd9b6-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="fd9b6-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fd9b6-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fd9b6-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd9b6-127">正しくない</span><span class="sxs-lookup"><span data-stu-id="fd9b6-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd9b6-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="fd9b6-128">See also</span></span>



[<span data-ttu-id="fd9b6-129">IsUMEnabled 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="fd9b6-129">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)


[<span data-ttu-id="fd9b6-130">Exchange 用のユニファイドメッセージング web サービスの XML 要素</span><span class="sxs-lookup"><span data-stu-id="fd9b6-130">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)

