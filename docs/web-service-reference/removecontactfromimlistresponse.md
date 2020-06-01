---
title: RemoveContactFromImListResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f784c433-5f5f-4171-a973-04ee6215c6b8
description: RemoveContactFromImListResponse 要素は、RemoveContactFromImList 要求への応答を表します。
ms.openlocfilehash: 8fedcfbbc83246bc553c5e6adc0d9d780040ec2f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466606"
---
# <a name="removecontactfromimlistresponse"></a><span data-ttu-id="128d9-103">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="128d9-103">RemoveContactFromImListResponse</span></span>

<span data-ttu-id="128d9-104">**RemoveContactFromImListResponse**要素は、 **RemoveContactFromImList**要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="128d9-104">The **RemoveContactFromImListResponse** element represents a response to a **RemoveContactFromImList** request.</span></span> 
  
```XML
<RemoveContactFromImListResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RemoveContactFromImListResponse>
```

 <span data-ttu-id="128d9-105">**RemoveContactFromImListResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="128d9-105">**RemoveContactFromImListResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="128d9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="128d9-106">Attributes and elements</span></span>

<span data-ttu-id="128d9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="128d9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="128d9-108">属性</span><span class="sxs-lookup"><span data-stu-id="128d9-108">Attributes</span></span>

<span data-ttu-id="128d9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="128d9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="128d9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="128d9-110">Child elements</span></span>

<span data-ttu-id="128d9-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="128d9-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="128d9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="128d9-112">Parent elements</span></span>

<span data-ttu-id="128d9-113">なし。</span><span class="sxs-lookup"><span data-stu-id="128d9-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="128d9-114">注釈</span><span class="sxs-lookup"><span data-stu-id="128d9-114">Remarks</span></span>

<span data-ttu-id="128d9-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="128d9-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="128d9-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="128d9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="128d9-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="128d9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="128d9-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="128d9-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="128d9-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="128d9-119">Schema name</span></span>  <br/> |<span data-ttu-id="128d9-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="128d9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="128d9-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="128d9-121">Validation file</span></span>  <br/> |<span data-ttu-id="128d9-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="128d9-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="128d9-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="128d9-123">Can be empty</span></span>  <br/> |<span data-ttu-id="128d9-124">false</span><span class="sxs-lookup"><span data-stu-id="128d9-124">false</span></span>  <br/> |
   

