---
title: AddImGroupResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2fca9474-f5f8-44e8-975d-145fc7696edf
description: AddImGroupResponse は、AddImGroup 要求に対する応答を定義します。
ms.openlocfilehash: 1c3873d46c6f55cee9b7ab10114f26e6fb322b30
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462774"
---
# <a name="addimgroupresponse"></a><span data-ttu-id="f6ad3-103">AddImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="f6ad3-103">AddImGroupResponse</span></span>

<span data-ttu-id="f6ad3-104">**AddImGroupResponse**は、 **addimgroup**要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="f6ad3-104">The **AddImGroupResponse** defines a response to an **AddImGroup** request.</span></span> 
  
```XML
<AddImGroupResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ImGroup/>
</AddImGroupResponse>
```

 <span data-ttu-id="f6ad3-105">**AddImContactToGroupResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f6ad3-105">**AddImContactToGroupResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6ad3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f6ad3-106">Attributes and elements</span></span>

<span data-ttu-id="f6ad3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f6ad3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6ad3-108">属性</span><span class="sxs-lookup"><span data-stu-id="f6ad3-108">Attributes</span></span>

<span data-ttu-id="f6ad3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f6ad3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6ad3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f6ad3-110">Child elements</span></span>

<span data-ttu-id="f6ad3-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Imgroup](imgroup.md)</span><span class="sxs-lookup"><span data-stu-id="f6ad3-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ImGroup](imgroup.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f6ad3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f6ad3-112">Parent elements</span></span>

<span data-ttu-id="f6ad3-113">なし。</span><span class="sxs-lookup"><span data-stu-id="f6ad3-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f6ad3-114">注釈</span><span class="sxs-lookup"><span data-stu-id="f6ad3-114">Remarks</span></span>

<span data-ttu-id="f6ad3-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f6ad3-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f6ad3-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f6ad3-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6ad3-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f6ad3-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6ad3-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="f6ad3-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f6ad3-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f6ad3-119">Schema name</span></span>  <br/> |<span data-ttu-id="f6ad3-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="f6ad3-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f6ad3-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f6ad3-121">Validation file</span></span>  <br/> |<span data-ttu-id="f6ad3-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f6ad3-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f6ad3-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f6ad3-123">Can be empty</span></span>  <br/> |<span data-ttu-id="f6ad3-124">false</span><span class="sxs-lookup"><span data-stu-id="f6ad3-124">false</span></span>  <br/> |
   

