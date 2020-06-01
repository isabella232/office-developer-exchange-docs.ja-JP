---
title: RemoveImGroupResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 55d6f802-a32c-45c6-b53c-b8b495d1e62f
description: RemoveImGroupResponse 要素は、RemoveImGroup 要求への応答を表します。
ms.openlocfilehash: 9cff2af802392a241f2257d42741cb2f5a0e277e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456004"
---
# <a name="removeimgroupresponse"></a><span data-ttu-id="d9c9e-103">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="d9c9e-103">RemoveImGroupResponse</span></span>

<span data-ttu-id="d9c9e-104">**RemoveImGroupResponse**要素は、 **removeimgroup**要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="d9c9e-104">The **RemoveImGroupResponse** element represents a response to a **RemoveImGroup** request.</span></span> 
  
```XML
<RemoveImGroupResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RemoveImGroupResponse>
```

 <span data-ttu-id="d9c9e-105">**RemoveImGroupResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d9c9e-105">**RemoveImGroupResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9c9e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d9c9e-106">Attributes and elements</span></span>

<span data-ttu-id="d9c9e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d9c9e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9c9e-108">属性</span><span class="sxs-lookup"><span data-stu-id="d9c9e-108">Attributes</span></span>

<span data-ttu-id="d9c9e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d9c9e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9c9e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d9c9e-110">Child elements</span></span>

<span data-ttu-id="d9c9e-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="d9c9e-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d9c9e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d9c9e-112">Parent elements</span></span>

<span data-ttu-id="d9c9e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d9c9e-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d9c9e-114">注釈</span><span class="sxs-lookup"><span data-stu-id="d9c9e-114">Remarks</span></span>

<span data-ttu-id="d9c9e-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d9c9e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d9c9e-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d9c9e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9c9e-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d9c9e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9c9e-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="d9c9e-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d9c9e-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d9c9e-119">Schema name</span></span>  <br/> |<span data-ttu-id="d9c9e-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d9c9e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d9c9e-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d9c9e-121">Validation file</span></span>  <br/> |<span data-ttu-id="d9c9e-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d9c9e-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d9c9e-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d9c9e-123">Can be empty</span></span>  <br/> |<span data-ttu-id="d9c9e-124">false</span><span class="sxs-lookup"><span data-stu-id="d9c9e-124">false</span></span>  <br/> |
   

