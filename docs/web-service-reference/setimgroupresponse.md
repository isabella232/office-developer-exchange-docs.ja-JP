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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44438055"
---
# <a name="setimgroupresponse"></a><span data-ttu-id="efa59-103">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="efa59-103">SetImGroupResponse</span></span>

<span data-ttu-id="efa59-104">**SetImGroupResponse**要素は、 **setimgroup**要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="efa59-104">The **SetImGroupResponse** element represents a response to a **SetImGroup** request.</span></span> 
  
```XML
<SetImGroupResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SetImGroupResponse>
```

 <span data-ttu-id="efa59-105">**SetImGroupResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="efa59-105">**SetImGroupResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="efa59-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="efa59-106">Attributes and elements</span></span>

<span data-ttu-id="efa59-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="efa59-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="efa59-108">属性</span><span class="sxs-lookup"><span data-stu-id="efa59-108">Attributes</span></span>

<span data-ttu-id="efa59-109">なし。</span><span class="sxs-lookup"><span data-stu-id="efa59-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="efa59-110">子要素</span><span class="sxs-lookup"><span data-stu-id="efa59-110">Child elements</span></span>

<span data-ttu-id="efa59-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="efa59-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="efa59-112">親要素</span><span class="sxs-lookup"><span data-stu-id="efa59-112">Parent elements</span></span>

<span data-ttu-id="efa59-113">なし。</span><span class="sxs-lookup"><span data-stu-id="efa59-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="efa59-114">注釈</span><span class="sxs-lookup"><span data-stu-id="efa59-114">Remarks</span></span>

<span data-ttu-id="efa59-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="efa59-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="efa59-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="efa59-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="efa59-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="efa59-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="efa59-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="efa59-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="efa59-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="efa59-119">Schema name</span></span>  <br/> |<span data-ttu-id="efa59-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="efa59-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="efa59-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="efa59-121">Validation file</span></span>  <br/> |<span data-ttu-id="efa59-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="efa59-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="efa59-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="efa59-123">Can be empty</span></span>  <br/> |<span data-ttu-id="efa59-124">false</span><span class="sxs-lookup"><span data-stu-id="efa59-124">false</span></span>  <br/> |
   

