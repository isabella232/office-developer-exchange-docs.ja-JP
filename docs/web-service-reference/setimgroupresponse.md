---
title: SetImGroupResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5562b38-6a3e-49e0-b1db-ec8cd0683863
description: SetImGroupResponse 要素は、SetImGroup 要求への応答を表します。
ms.openlocfilehash: 9c5f6bb5c2a4ffe4626f242ec06b7e022ef21bbf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44438055"
---
# <a name="setimgroupresponse"></a><span data-ttu-id="ba819-103">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="ba819-103">SetImGroupResponse</span></span>

<span data-ttu-id="ba819-104">**SetImGroupResponse**要素は、 **setimgroup**要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="ba819-104">The **SetImGroupResponse** element represents a response to a **SetImGroup** request.</span></span> 
  
```XML
<SetImGroupResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SetImGroupResponse>
```

 <span data-ttu-id="ba819-105">**SetImGroupResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ba819-105">**SetImGroupResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba819-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ba819-106">Attributes and elements</span></span>

<span data-ttu-id="ba819-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ba819-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba819-108">属性</span><span class="sxs-lookup"><span data-stu-id="ba819-108">Attributes</span></span>

<span data-ttu-id="ba819-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ba819-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba819-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ba819-110">Child elements</span></span>

<span data-ttu-id="ba819-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="ba819-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ba819-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ba819-112">Parent elements</span></span>

<span data-ttu-id="ba819-113">なし。</span><span class="sxs-lookup"><span data-stu-id="ba819-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ba819-114">注釈</span><span class="sxs-lookup"><span data-stu-id="ba819-114">Remarks</span></span>

<span data-ttu-id="ba819-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ba819-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ba819-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ba819-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba819-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ba819-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba819-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="ba819-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ba819-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ba819-119">Schema name</span></span>  <br/> |<span data-ttu-id="ba819-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="ba819-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ba819-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ba819-121">Validation file</span></span>  <br/> |<span data-ttu-id="ba819-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="ba819-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ba819-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ba819-123">Can be empty</span></span>  <br/> |<span data-ttu-id="ba819-124">false</span><span class="sxs-lookup"><span data-stu-id="ba819-124">false</span></span>  <br/> |
   

