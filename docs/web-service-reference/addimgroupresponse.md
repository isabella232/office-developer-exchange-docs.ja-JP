---
title: AddImGroupResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2fca9474-f5f8-44e8-975d-145fc7696edf
description: AddImGroupResponse は、AddImGroup 要求への応答を定義します。
ms.openlocfilehash: 1fc7a2cd8c86a6ac7ce1d23d4b62fc6b2ade9d70
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759287"
---
# <a name="addimgroupresponse"></a><span data-ttu-id="0ad6a-103">AddImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="0ad6a-103">AddImGroupResponse</span></span>

<span data-ttu-id="0ad6a-104">**AddImGroupResponse**は、 **AddImGroup**要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="0ad6a-104">The **AddImGroupResponse** defines a response to an **AddImGroup** request.</span></span> 
  
```XML
<AddImGroupResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ImGroup/>
</AddImGroupResponse>
```

 <span data-ttu-id="0ad6a-105">**AddImContactToGroupResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0ad6a-105">**AddImContactToGroupResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ad6a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0ad6a-106">Attributes and elements</span></span>

<span data-ttu-id="0ad6a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0ad6a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ad6a-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ad6a-108">Attributes</span></span>

<span data-ttu-id="0ad6a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0ad6a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ad6a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0ad6a-110">Child elements</span></span>

<span data-ttu-id="0ad6a-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ImGroup](imgroup.md)</span><span class="sxs-lookup"><span data-stu-id="0ad6a-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ImGroup](imgroup.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0ad6a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0ad6a-112">Parent elements</span></span>

<span data-ttu-id="0ad6a-113">なし。</span><span class="sxs-lookup"><span data-stu-id="0ad6a-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ad6a-114">備考</span><span class="sxs-lookup"><span data-stu-id="0ad6a-114">Remarks</span></span>

<span data-ttu-id="0ad6a-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0ad6a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0ad6a-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0ad6a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ad6a-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="0ad6a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ad6a-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="0ad6a-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0ad6a-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0ad6a-119">Schema name</span></span>  <br/> |<span data-ttu-id="0ad6a-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="0ad6a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0ad6a-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0ad6a-121">Validation file</span></span>  <br/> |<span data-ttu-id="0ad6a-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0ad6a-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0ad6a-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0ad6a-123">Can be empty</span></span>  <br/> |<span data-ttu-id="0ad6a-124">false</span><span class="sxs-lookup"><span data-stu-id="0ad6a-124">false</span></span>  <br/> |
   

