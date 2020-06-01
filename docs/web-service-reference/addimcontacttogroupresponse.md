---
title: AddImContactToGroupResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e75f8da2-d0a4-44f4-a597-1554757fdf55
description: AddImContactToGroupResponse 要素は、AddImContactToGroup 要求への応答を定義します。
ms.openlocfilehash: 1d186c89a7fdfd978fb8f713908a4f2ebfbddfa9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463686"
---
# <a name="addimcontacttogroupresponse"></a><span data-ttu-id="546fa-103">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="546fa-103">AddImContactToGroupResponse</span></span>

<span data-ttu-id="546fa-104">**AddImContactToGroupResponse**要素は、 **Addimcontacttogroup**要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="546fa-104">The **AddImContactToGroupResponse** element defines a response to an **AddImContactToGroup** request.</span></span> 
  
```XML
<AddImContactToGroupResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</AddImContactToGroupResponse>
```

 <span data-ttu-id="546fa-105">**AddImContactToGroupResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="546fa-105">**AddImContactToGroupResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="546fa-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="546fa-106">Attributes and elements</span></span>

<span data-ttu-id="546fa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="546fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="546fa-108">属性</span><span class="sxs-lookup"><span data-stu-id="546fa-108">Attributes</span></span>

<span data-ttu-id="546fa-109">なし。</span><span class="sxs-lookup"><span data-stu-id="546fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="546fa-110">子要素</span><span class="sxs-lookup"><span data-stu-id="546fa-110">Child elements</span></span>

<span data-ttu-id="546fa-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="546fa-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="546fa-112">親要素</span><span class="sxs-lookup"><span data-stu-id="546fa-112">Parent elements</span></span>

<span data-ttu-id="546fa-113">なし。</span><span class="sxs-lookup"><span data-stu-id="546fa-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="546fa-114">注釈</span><span class="sxs-lookup"><span data-stu-id="546fa-114">Remarks</span></span>

<span data-ttu-id="546fa-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="546fa-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="546fa-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="546fa-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="546fa-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="546fa-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="546fa-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="546fa-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="546fa-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="546fa-119">Schema name</span></span>  <br/> |<span data-ttu-id="546fa-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="546fa-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="546fa-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="546fa-121">Validation file</span></span>  <br/> |<span data-ttu-id="546fa-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="546fa-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="546fa-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="546fa-123">Can be empty</span></span>  <br/> |<span data-ttu-id="546fa-124">false</span><span class="sxs-lookup"><span data-stu-id="546fa-124">false</span></span>  <br/> |
   

