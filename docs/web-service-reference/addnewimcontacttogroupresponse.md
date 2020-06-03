---
title: AddNewImContactToGroupResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e1a1c5fa-9e1e-4ee7-bb19-77c29b47ecbb
description: AddNewImContactToGroupResponse 要素は、AddNewImContactToGroup 要求に対する応答を定義します。
ms.openlocfilehash: 6c8f0f2330e4394a7657ddeef0df93f1c75c7001
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467712"
---
# <a name="addnewimcontacttogroupresponse"></a><span data-ttu-id="6bb8e-103">AddNewImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="6bb8e-103">AddNewImContactToGroupResponse</span></span>

<span data-ttu-id="6bb8e-104">**AddNewImContactToGroupResponse**要素は、 **AddNewImContactToGroup**要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="6bb8e-104">The **AddNewImContactToGroupResponse** element defines a response to an **AddNewImContactToGroup** request.</span></span> 
  
```XML
<AddNewImContactToGroupResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Persona/>
</AddNewImContactToGroupResponse>
```

 <span data-ttu-id="6bb8e-105">**AddNewImContactToGroupResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6bb8e-105">**AddNewImContactToGroupResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6bb8e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6bb8e-106">Attributes and elements</span></span>

<span data-ttu-id="6bb8e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6bb8e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6bb8e-108">属性</span><span class="sxs-lookup"><span data-stu-id="6bb8e-108">Attributes</span></span>

<span data-ttu-id="6bb8e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6bb8e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6bb8e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6bb8e-110">Child elements</span></span>

<span data-ttu-id="6bb8e-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Persona](persona.md)</span><span class="sxs-lookup"><span data-stu-id="6bb8e-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Persona](persona.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6bb8e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6bb8e-112">Parent elements</span></span>

<span data-ttu-id="6bb8e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6bb8e-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6bb8e-114">注釈</span><span class="sxs-lookup"><span data-stu-id="6bb8e-114">Remarks</span></span>

<span data-ttu-id="6bb8e-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6bb8e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6bb8e-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6bb8e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6bb8e-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6bb8e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6bb8e-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="6bb8e-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6bb8e-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6bb8e-119">Schema name</span></span>  <br/> |<span data-ttu-id="6bb8e-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6bb8e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6bb8e-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6bb8e-121">Validation file</span></span>  <br/> |<span data-ttu-id="6bb8e-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6bb8e-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6bb8e-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6bb8e-123">Can be empty</span></span>  <br/> |<span data-ttu-id="6bb8e-124">false</span><span class="sxs-lookup"><span data-stu-id="6bb8e-124">false</span></span>  <br/> |
   

